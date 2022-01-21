---
title: 'contentType: addCopyFromContentTypeHub'
description: Adicione ou sincronize uma cópia de um tipo de conteúdo publicado do hub de tipo de conteúdo para um site de destino ou uma lista.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 39b147c1c75b535962eaa70d4120304b4e4634ca
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162197"
---
# <a name="contenttype-addcopyfromcontenttypehub"></a>contentType: addCopyFromContentTypeHub
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione ou sincronize uma cópia de um tipo de conteúdo publicado do hub de tipo de conteúdo para um site de [destino](../resources/site.md) ou uma [lista.](../resources/list.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) | Sites.Manage.All, Sites.FullControl.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | Sites.Manage.All, Sites.FullControl.All |


## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
POST /sites/{siteId}/contentTypes/addCopyFromContentTypeHub
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|contentTypeId|Cadeia de caracteres| ID do tipo de conteúdo no hub de tipo de conteúdo que deve ser adicionado ao site de destino ou a uma lista.|



## <a name="response"></a>Resposta

Se tiver êxito, essa ação retornará um código de resposta e um objeto contentType no corpo da resposta se o tipo de conteúdo for adicionado de forma síncrona ou um código de resposta se o tipo de conteúdo for sincronizado de forma `200 OK` [](../resources/contenttype.md) `202 Accepted` assíncrona. A resposta também conterá um header, que contém o local do `Location` [richLongRunningOperation](../resources/richLongRunningOperation.md) que foi criado para manipular a cópia/sincronização. No caso de uma operação assíncrona, pode levar até 70 minutos para sincronizar ou adicionar um tipo de conteúdo.

## <a name="examples"></a>Exemplos

### <a name="example-1-synchronous-pull"></a>Exemplo 1: pull síncrono

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "String"
}
```


#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.contentType",
    "id": "String (identifier)",
    "description": "String",
    "group": "String",
    "hidden": "Boolean",
    "isBuiltIn": "Boolean",
    "name": "String"
  }
}
```
### <a name="example-2-asynchronous-pull"></a>Exemplo 2: pull assíncrono

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "String"
}
```


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 202 Accepted
location: https://graph.microsoft.com/beta/sites/{siteId}/lists/{listId}/operations/{operationId}
```
