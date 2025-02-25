---
id: 639f2a72-3578-468c-9c9a-81b28496af66
blueprint: page
title: 'Grupos de Investigación'
titulo_pagina: 'Grupos de Investigación'
texto_bienvenida: 'Grupos de Investigación'
author: 06ac68ab-d29f-41e9-9b9a-dd4da3996484
template: home
template_imagen_fondo:
  code: |-
    <!--<div class="page-header header-filter clear-filter purple-filter header-small" data-parallax="true" style="background-image: url('assets/a_home_otros/font-grupos.jpeg');">
        <div class="container">
          <div class="row">
            <div class="col-md-8 ml-auto mr-auto ">
             <h1 class="title">{{texto_bienvenida}}</h1>
            </div>
          </div>
        </div>
      </div>-->
  mode: htmlmixed
modal:
  code: null
  mode: htmlmixed
updated_by: 06ac68ab-d29f-41e9-9b9a-dd4da3996484
updated_at: 1692976578
block_types:
  -
    id: ll8y8w9d
    template:
      code: |-
        <style>
        /* Estilo para el contenedor del título */
        .title-container {
            display: inline-block;
            padding: 10px 20px;
            border: 2px solid #2980b9;
            border-radius: 10px;
            background: #f0f8ff;
            color: #2c3e50;
            font-weight: bold;
            font-size: 1.25rem;
            text-align: center;
            margin: 0 auto 25px auto;
        }

        /* Estilo para las tarjetas de los grupos */
        .card {
            border: 1px solid #ddd;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            background-color: #ffffff;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .contenido-card {
            padding: 15px;
            text-align: center;
        }

        .contenido-card h4 {
            font-size: 1.2rem;
            color: #2c3e50;
            margin-bottom: 10px;
        }

        .contenido-card p {
            font-size: 0.9rem;
            color: #7f8c8d;
            margin: 5px 0;
        }

        .contenido-card a {
            display: inline-block;
            margin-top: 10px;
            padding: 8px 15px;
            background-color: #2980b9;
            color: #ffffff;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .contenido-card a:hover {
            background-color: #1a5e85;
        }

        /* Estilo para el footer */
        footer {
            background-color: #2c3e50;
            color: #ffffff;
            padding: 20px 0;
            text-align: center;
        }

        footer a {
            color: #1abc9c;
            text-decoration: none;
        }

        footer a:hover {
            text-decoration: underline;
        }
        </style>

        <div class="row">
            <div class="col-md-12 text-center">
                <h1 class="title-container">
                    En este espacio encontrarás a los docentes investigadores reconocidos por su aporte al desarrollo académico y científico. Conoce a quienes, desde su especialidad, contribuyen al progreso de nuestra región y del país.
                </h1>
            </div>
        </div>

        <div class="section justify-content-center" style="margin-top: -100px;">
            <div class="section col-md-12 ml-auto mr-auto">
                <div class="row">
                    {{collection:grupos_inv}}
                    <div class="col-md-3">
                        <br>
                        <div class="card">
                            <figure>
                                <img src="./assets/grupos-investigacion/grupo2.jpeg" alt="Imagen del grupo">
                            </figure>
                            <div class="contenido-card">
                                <h4><b>{{nombre_grupo}}</b></h4>
                                <p><strong>Coordinador:</strong> {{jefe_grupo}}</p>
                                <p><strong>Integrantes:</strong></p>
                                <a href="#">{{integrantes}}</a>
                            </div>
                        </div>
                    </div>
                    {{/collection:grupos_inv}}
                    <div class="col-md-1"></div>
                </div>
            </div>
        </div>

      mode: htmlmixed
    type: template
    enabled: true
---
