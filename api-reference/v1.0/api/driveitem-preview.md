---
title: 'driveItem: visualização'
description: Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 5fea16ce14e2df4b87ddc2b3f9246dfe758ec5b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073261"
---
# <a name="driveitem-preview"></a>driveItem: visualização

Namespace: microsoft.graph

Esta ação permite que você obtenha uma URL incorporável de curta duração para um item a fim de renderizar uma visualização temporária.

Se você quiser obter links incorporáveis de longa duração, use a API [CreateLink][] em vez disso.

> **Observação:** No momento, a ação de **Visualização** só está disponível no SharePoint e no onedrive for Business.

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)
|:---------------------------------------|:-------------------------------------------
| Delegado (conta corporativa ou de estudante)     | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All
| Delegado (conta pessoal da Microsoft) | Sem suporte.
| Aplicativo                            | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a>Corpo da solicitação

O corpo da solicitação define as propriedades da URL incorporável que seu aplicativo está solicitando.
A solicitação deve ser um objeto JSON com as seguintes propriedades.

|   Nome      |  Tipo         | Descrição
|:------------|:--------------|:-----------------------------------------------
| page        | Cadeia de caracteres/número | Opcional. Número de página do documento para iniciar em, se aplicável. Especificado como cadeia de caracteres para casos de uso futuros em relação a tipos de arquivo como ZIP.
| zoom        | number        | Opcional. Nível de zoom para iniciar em, se aplicável.

## <a name="response"></a>Resposta

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

A resposta será um objeto JSON que contém as seguintes propriedades:

| Nome           | Tipo   | Descrição
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | URL adequada para incorporação usando HTTP GET (IFrames, etc.)
| postUrl        | string | URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)
| postparameters | string | LANÇAR parâmetros para incluir se estiver usando postUrl

GetUrl, postUrl ou ambos podem ser retornados, dependendo do estado atual do suporte de embed para as opções especificadas.

postparameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded` e, se estiver executando uma postagem no postUrl, o tipo de conteúdo deve ser definido de acordo. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>Página/zoom

As opções de ' página ' e ' Zoom ' podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização oferecer suporte a ele.

