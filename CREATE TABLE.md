# SQL
CREATE DATABASE MUSIC;

USE MUSIC;

CREATE TABLE GENEROS (
    generoId INT PRIMARY KEY,
    Descricao NVARCHAR(255)
);

CREATE TABLE musicas (
    MusicaId INT PRIMARY KEY,
    Nome NVARCHAR(255),
    Duracao TIME(3),
    GeneroId INT,
    ArtistaId INT,
    CONSTRAINT FK_musicas_generos FOREIGN KEY (GeneroId) REFERENCES GENEROS(generoId),
    CONSTRAINT FK_musicas_artistas FOREIGN KEY (ArtistaId) REFERENCES artistas(ArtistaId)
);

CREATE TABLE artistas (
    ArtistaId INT PRIMARY KEY,
    Nome NVARCHAR(255)
);
