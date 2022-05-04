---
title: 'contentType: getCompatibleHubContentTypes'
description: Obtenha uma lista de tipos de conteúdo compatíveis do hub de tipo de conteúdo que pode ser adicionado a um site de destino ou a uma lista.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 1d0f5d421e1f1f68298c555c8e7dad9dd81f294f
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191824"
---
# <a name="contenttype-getcompatiblehubcontenttypes"></a>contentType: getCompatibleHubContentTypes
Namespace: microsoft.graph

Obtenha uma lista de tipos de conteúdo compatíveis do hub de tipo de conteúdo que pode ser adicionado a um [site de destino](../resources/site.md) ou a uma [lista](../resources/list.md).

Esse método faz parte das alterações de publicação de tipo de conteúdo para otimizar a sincronização de tipos de conteúdo publicados para sites e listas, alternando efetivamente de uma abordagem "push everywhere" para "efetuar pull conforme necessário". O método permite que os usuários efetuem pull de tipos de conteúdo diretamente do hub de tipo de conteúdo para um site ou lista. Para obter mais informações, consulte [contentType: addCopyFromContentTypeHub](contenttype-addcopyfromcontenttypehub.md) e a postagem no blog [Syntex Product Updates – agosto de 2021](https://techcommunity.microsoft.com/t5/sharepoint-syntex-blog/syntex-product-updates-august-2021/ba-p/2606438).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) | Sites.Manage.All, Sites.FullControl.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{siteId}/lists/{listId}/contentTypes/getCompatibleHubContentTypes
GET /sites/{siteId}/contentTypes/getCompatibleHubContentTypes
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código `200 OK` de resposta e uma coleção de [objetos contentType](../resources/contenttype.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "name": "contenttype_getcompatiblehubcontenttypes"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/sites/root/lists/Documents/contentTypes/getCompatibleHubContentTypes
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.contentType",
      "id": "0x0101",
      "description": "Document content type",
      "group": "Document Content Types",
      "hidden": false,
      "isBuiltIn": true,
      "name": "Document"
    }
  ]
}
```

