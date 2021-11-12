---
title: 'reviewSet: addToReviewSet'
description: Inicie o processo de adição de uma coleção Microsoft 365 serviços a um conjunto de revisão.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: bc489619c25b6bc58a60fe898f7e0275365ee5ac
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60943497"
---
# <a name="reviewset-addtoreviewset"></a>reviewSet: addToReviewSet

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Inicie o processo de adição de uma coleção Microsoft 365 serviços a um conjunto de revisão. Depois que a operação for criada, você poderá obter o status da operação recuperando o parâmetro `Location` dos headers de resposta. O local fornece uma URL que retornará [caseExportOperation](../resources/ediscovery-caseexportoperation.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reviewSets/{reviewsetId}/addToReviewSet
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
|sourceCollection|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|A ID da **sourceCollection**.|
|additionalData|[microsoft.graph.ediscovery.dataCollectionScope](../resources/ediscovery-addtoreviewsetoperation.md#datacollectionscope-values)|O **dataCollectionScope** que será incluído na coleção.|

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reviewset_addtoreviewset"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/080e8cad-f21f-4452-8826-0ddf7e949fdd/reviewSets/6fe25d32-8167-4625-b75c-c4181ccbd9d5/addToReviewSet
Content-Type: application/json

{
    "sourceCollection": {
        "id": "1a9b4145d8f84e39bc45a7f68c5c5119"
    },
    "additionalData": "linkedFiles"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reviewset-addtoreviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reviewset-addtoreviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reviewset-addtoreviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reviewset-addtoreviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]



### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
```
