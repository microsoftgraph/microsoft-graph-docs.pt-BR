---
title: 'driveItem: visualização'
description: Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ae5140bf6164aedd051f04c2c43c361f16517e7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986072"
---
# <a name="driveitem-preview"></a>driveItem: visualização

Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.

Se você quiser obter links incorporável vida útil longa, use o [createLink][] API.

> **Observação:** Atualmente, a ação de **visualização** só está disponível no SharePoint e o OneDrive for Business.

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)
|:---------------------------------------|:-------------------------------------------
| Delegado (conta corporativa ou de estudante)     | Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All
| Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.ReadWrite.All
| Aplicativo                            | Sem suporte.

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

O corpo da solicitação define as propriedades da URL incorporável está solicitando o seu aplicativo.
A solicitação deve ser um objeto JSON com as seguintes propriedades.

|   Nome      |  Tipo         | Descrição
|:------------|:--------------|:-----------------------------------------------
| página        | número de sequência de caracteres / | Opcional. Número de página do documento para iniciar em, se aplicável. Especificado como cadeia de caracteres para uso futuro casos em torno de tipos de arquivo como ZIP.
| zoom        | number        | Opcional. Amplie o nível para iniciar em, se aplicável.

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
| getUrl         | string | URL adequada para incorporação usando HTTP GET (iframes, etc.)
| postUrl        | string | URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)
| postParameters | string | Parâmetros de POSTAGEM para incluir se usando postUrl

GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte de embed para as opções especificadas.

postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>Página/zoom

O 'página' e 'zoom' Opções podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização lhe fornecer apoio.
