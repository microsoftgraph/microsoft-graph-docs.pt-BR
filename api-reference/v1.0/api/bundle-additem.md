---
author: JeremyKelley
title: Adicionar item a um pacote
description: Adicione item a um pacote de driveItems.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 88b8e8c5e93d746522979f4086adeae5d5212e00
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724253"
---
# <a name="add-item-to-a-bundle"></a>Adicionar item a um pacote

Namespace: microsoft.graph

Adicione um [driveItem][] adicional de uma unidade a um [pacote][].

[Agrupar]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte.                             |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All   |
|Aplicativo          | Sem suporte.                                           |

## <a name="http-request"></a>Solicitação HTTP

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição  |
|:------------- |:------------ |
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de um [objeto driveItem][] .

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Para obter informações sobre respostas a erros, consulte [Microsoft Graph respostas de erro e tipos de recursos][error-response].

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

A seguir está um exemplo de uma solicitação que adiciona um item existente ao pacote especificado.

<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/v1.0/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section&quot;: &quot;documentation"
} -->


