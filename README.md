# `mpv_crop_script.lua`

### A Lua script to take cropped screenshots in mpv, sans external dependencies | Show preview thumbnails in mpv's OSC seekbar | Um Lua script para fazer previsão de tela na barra de progresso do mpv, sem dependências externas

[![](docs/sintel_crop_guides_crosshair.jpg "Cropping Sintel (2010) with mpv_crop_script.lua")](https://youtu.be/Eis0Ipu7yw0)
[*Click the image or here to see the script in action*](https://youtu.be/Eis0Ipu7yw0)

*(You might also be interested in [`mpv_thumbnail_script.lua`](https://github.com/TheAMM/mpv_thumbnail_script))*

----

## What is it? | O que é isso?

`mpv_crop_script.lua` is a script for making cropped screenshots from within [mpv](https://github.com/mpv-player/mpv), without any external dependencies[<sup>1</sup>](#footnotes), cross-platform-ly [<sup>2</sup>](#footnotes)!

----

`mpv_crop_script.lua` é um script para fazer capturas de tela recortadas de dentro de [mpv](https://github.com/mpv-player/mpv), sem quaisquer dependências externas [<sup>1</sup>](#footnotes), plataforma-cruzada-ly [<sup>2</sup>](#footnotes)!

## How? | Como?

mpv by itself doesn't support cropped screenshots, but can be told to save a full screenshot at a specified location.
This full-sized image can then be cropped down to size, but this requires a tool to edit the image (like ImageMagick). Bothersome!

However, we can forget external ependencies by calling on mpv itself to use the the built-in [encoding features](https://mpv.io/manual/master/#encoding). Bam!

----

mpv por si só não suporta capturas de tela cortadas, mas pode ser instruído a salvar uma captura de tela completa em um local especificado.
Esta imagem em tamanho real pode então ser cortada no tamanho certo, mas isso requer uma ferramenta para editar a imagem (como ImageMagick). Incomodador!

No entanto, podemos esquecer as dependências externas chamando o próprio mpv para usar os [recursos de codificação integrados](https://mpv.io/manual/master/#encoding). Pronto!

## Configuration | Configuração

Create a file called `mpv_crop_script.conf` or `mpv_thumbnail_script.conf` inside your mpv's `lua-settings` directory.

For example:
  * Linux/Unix/Mac: `~/.config/mpv/lua-settings/mpv_crop_script.conf`
  * Windows: `%APPDATA%\Roaming\mpv\lua-settings\mpv_crop_script.conf`

You can grab an example config [from HERE](https://raw.githubusercontent.com/TheAMM/mpv_sort_script/build/mpv_sort_script.conf).

See the [Files section](https://mpv.io/manual/master/#files) in mpv's manual for more info.

----

Crie um arquivo chamado `mpv_thumbnail_script.conf` dentro do diretório `lua-settings` em seu diretório `mpv`.

Por exemplo:
  * Linux/Unix/Mac:  `~/.config/mpv/lua-settings/mpv_thumbnail_script.conf`
  * Windows: `%APPDATA%\Roaming\mpv\lua-settings\mpv_thumbnail_script.conf`

Você pode pegar um exemplo de configuração [AQUI](https://raw.githubusercontent.com/felipefacundes/mpv_crop_script/main/mpv/lua-settings/mpv_thumbnail_script.conf).

Veja a [Seção Arquivos](https://mpv.io/manual/master/#files) no manual do mpv para mais informações.

----

## Script installation and practical use | Instalação e uso prático do script

You can use the template. Already ready. Just clone the repository:
  `git clone https://github.com/felipefacundes/mpv_crop_script`

  * Linux/Unix/Mac: After cloning just copy the entire `mpv` folder into `~/.config` folder:
  `cd mpv_crop_script && cp -rf mpv ~/.config`

  * Windows: copy the mpv folder to `%APPDATA%\Roaming\`

----

Você poderá usar o modelo. Já pronto. Basta clonar o repositório:
  `git clone https://github.com/felipefacundes/mpv_crop_script`

  * Linux/Unix/Mac: Após a clonagem, basta copiar toda a pasta `mpv` para a pasta`~/.config`:
  `cd mpv_crop_script && cp -rf mpv ~/.config`

  * Windows: copie a pasta mpv em `%APPDATA%\Roaming\`

## Change the Lua script (optional) | Alterar o Lua script (opcional)

You can change the script in Lua by following these guidelines [`string.format()`](http://www.lua.org/manual/5.1/manual.html#pdf-string.format)

----

Você pode alterar o script em Lua seguindo essas orientações [`string.format()`](http://www.lua.org/manual/5.1/manual.html#pdf-string.format)

----

#### Footnotes | Notas de rodapé

<sup>1</sup>You *may* need to add `mpv[.exe]` to your `PATH`.

<sup>2</sup>Developed & tested on Windows and Linux (Ubuntu), but it *should* work on Mac and whatnot as well, if <sup>1</sup> has been taken care of.

----

<sup>1</sup>Você *pode* precisar adicionar `mpv [.exe]` ao seu `PATH`.

<sup>2</sup>Desenvolvido e testado no Windows e Linux (ArchLinux), mas *deve* funcionar no Mac e outros sistemas, se o <sup>1</sup> tiver sido cuidado.

# Doação

Se você realmente gosta disso, pode me doar via [`PayPal`](https://www.paypal.com/donate/?hosted_button_id=REU2UNGXLQQPG).

# Donation

If you really like it, you can pay me with [`PayPal`](https://www.paypal.com/donate/?hosted_button_id=REU2UNGXLQQPG).
