# Gerar QRCode com C# fácil
Gera QRCodes em C# / Windows Forms com apenas 5 linhas de código.
Primeiramente crie um formulário com TextBox, um Button e uma PictureBox

## Instale a biblioteca QRCoder
Este projeto tem dependência com a bibliote QRCode.
Está disponível no NuGet - https://github.com/codebude/QRCoder
PAra instalar via NuGet acesse no Visual Studio o menu PROJETO > GERENCIADOR DE PACOTES DO NUGET


## Código para gerar o QRCode em C#

```
QRCodeGenerator qrGenerator = new QRCodeGenerator(); 
QRCodeData qrCodeData = qrGenerator.CreateQrCode(textBox1.Text, QRCodeGenerator.ECCLevel.Q); 
QRCode qrCode = new QRCode(qrCodeData); 
Bitmap qrCodeImage = qrCode.GetGraphic(20); 
pictureBox1.Image = qrCodeImage;
```

## Código completo para download
Este material está disponível no Blogson, leia o artigo - [Como gerar um QR Code com C# de forma simples, apenas 5 linhas](https://www.blogson.com.br/como-gerar-um-qr-code-com-c-de-forma-simples-apenas-5-linhas/)
