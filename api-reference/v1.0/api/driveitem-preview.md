---
title: 'driveItem: visualização'
description: Essa ação permite que você obtenha URLs inbeddáveis de curta duração para um item para renderizar uma visualização temporária.
ms.localizationpriority: medium
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: fecbdba30948dc89e0344a90574fe932562058fd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022762"
---
# <a name="driveitem-preview"></a>driveItem: visualização

Namespace: microsoft.graph

Essa ação permite que você obtenha uma URL in-loca de curta duração para um item para renderizar uma visualização temporária.

Se você quiser obter links inbeddáveis de longa duração, use a API [createLink][] em vez disso.

> **Observação:** No **momento,** a ação de visualização só está disponível SharePoint e OneDrive for Business.

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

O corpo da solicitação define propriedades da URL inbeddable que seu aplicativo está solicitando.
A solicitação deve ser um objeto JSON com as seguintes propriedades.

|   Nome      |  Tipo         | Descrição
|:------------|:--------------|:-----------------------------------------------
| page        | string/number | Opcional. Número da página do documento a ser inicial, se aplicável. Especificado como cadeia de caracteres para casos futuros de uso em torno de tipos de arquivo, como ZIP.
| zoom        | number        | Opcional. Nível de zoom para começar em, se aplicável.

## <a name="response"></a>Resposta

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

A resposta será um objeto JSON contendo as seguintes propriedades:

| Name           | Tipo   | Descrição
|:---------------|:-------|:---------------------------------------------------
| getUrl         | cadeia de caracteres | URL adequada para a incorporação usando HTTP GET (iframes, etc.)
| postUrl        | cadeia de caracteres | URL adequada para a incorporação usando HTTP POST (postagem de formulário, JS, etc.)
| postParameters | cadeia de caracteres | Parâmetros POST a incluir se estiver usando postUrl

GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte de incorporar para as opções especificadas.

postParameters é uma cadeia de caracteres formatada como , e se executar um POST para o postUrl o tipo de conteúdo deve ser `application/x-www-form-urlencoded` definido de acordo. Por exemplo:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a>Página/zoom

As opções 'page' e 'zoom' podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização for compatível com ele.

