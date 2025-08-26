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

  # Aplicação


## Instalação

```
# Criar projeto Laravel
composer create-project laravel/laravel .

# Copiar arquivo de configuração e gerar chave
copy .env.example .env
php artisan key:generate

```
## Verificar Instalação

```
php artisan --version
dir
```

## Banco de dados

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=mapslaravel
DB_USERNAME=root
DB_PASSWORD=senha
```

## Teste conexão:

```
php artisan tinker
DB::connection()->getPdo();
```


## Criação BD

```php artisan migrate```

## .env

```
APP_ENV=production
APP_DEBUG=false
APP_URL=https://seudominio.com
DB_USERNAME=usuario
DB_PASSWORD=senha
```

## Iniciar o projeto com laravel

```PHP artisan serve```


# O site

No desenvolvimento do website, não fiz um design muito elaborado ou inovador. Como o foco principal era fazer o backend e entender o laravel, foquei mais neles do que na estilização. Então, optei por trabalhar com uma paleta de cores inspirada na praia — remetendo ao mar, à areia e ao clima litorâneo. Essa escolha buscou transmitir uma sensação de leveza, tranquilidade e frescor, criando uma identidade visual simples, mas agradável e acolhedora para o usuário.

## 1 - Página Principal

Na página principal é exibido o **mapa interativo** (conectado ao JavaScript) e uma **lista de locais cadastrados**.  
Nessa tela, o usuário pode **visualizar uma localização por vez**, além de realizar operações de **CRUD** (editar e excluir locais já cadastrados).

<img width="1890" height="874" alt="Captura de tela 2025-08-26 131314" src="https://github.com/user-attachments/assets/298fa458-4e26-47fa-bc4f-bc91ec191f11" />

---

## 2 - Adicionar Localização

Ao clicar em **“Adicionar Local”** (seja no botão do header ou em outros pontos da página), o usuário é redirecionado para uma nova tela.  
No mapa interativo, basta clicar em um ponto para que a **latitude e longitude** sejam capturadas automaticamente.  
Depois, o usuário pode **inserir informações adicionais** sobre o local.

<img width="1899" height="880" alt="Captura de tela 2025-08-26 131442" src="https://github.com/user-attachments/assets/2050c6af-0f57-42b8-8cab-15c6dc3316e3" />

---

## 3 - Visualizar Informações

De volta à tela principal, é possível **selecionar uma localização específica** e **ampliar sua descrição**, visualizando os detalhes cadastrados.

<img width="1895" height="814" alt="Captura de tela 2025-08-26 131508" src="https://github.com/user-attachments/assets/e2c47b98-363b-4b9f-82d4-fc7f4f87a476" />

---

## 4 - Editar Localização

Se alguma informação tiver sido cadastrada incorretamente, é possível **editar os dados** e **salvar as alterações** diretamente no banco de dados.

<img width="1894" height="878" alt="Captura de tela 2025-08-26 131522" src="https://github.com/user-attachments/assets/f952f1da-68d3-4d3c-ab5b-234815ab0013" />
