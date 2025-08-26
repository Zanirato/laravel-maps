# Laravel Maps App

O **Laravel Maps App** é uma aplicação web desenvolvida em **Laravel 12** que permite adicionar e editar locais com suas informações detalhadas, desde endereço ate latitude e longitude, e visualizá-los em um mapa interativo.

## Funcionalidades

- **CRUD de locais**: Criar, visualizar, atualizar e excluir locais.
- **Mapas interativos**: Cada local possui uma posição no mapa, que pode ser atualizada ao clicar no mapa.
- **Informações completas**: Cada local possui nome, descrição, endereço e coordenadas.
- **Categorias**: Permite classificar os locais em categorias como Restaurante, Hotel, Shopping, Parque, Museu, Teatro, Hospital, Escola e Outro.
- **Interface responsiva**: Desenvolvido com Bootstrap e css, é adaptável a dispositivos móveis e desktop.

## Estrutura de Páginas

1. **Index (`index.blade.php`)**
   - Lista todos os locais cadastrados.
   - Permite acessar as páginas de detalhes, edição ou exclusão.

2. **Show (`show.blade.php`)**
   - Exibe detalhes de um local específico.
   - Exibe o mapa com marcador da localização do local.
   - Mostra informações como nome, categoria, descrição, endereço, coordenadas e datas.

3. **Create (`create.blade.php`)**
   - Permite criar um novo local.
   - Seleção de coordenadas diretamente no mapa.
   - Formulário com validação.

4. **Edit (`edit.blade.php`)**
   - Permite atualizar informações de um local existente.
   - Atualiza a localização clicando no mapa.
   - Formulário com validação e preenchimento automático dos campos existentes.

## Tecnologias Utilizadas

- **Backend**: Laravel 12
- **Frontend**: Blade Templates + Bootstrap 5
- **Mapas**: Leaflet.js + OpenStreetMap
- **Banco de Dados**: MySQL

# O site

Eu não consegui pensar em um designe criativ
