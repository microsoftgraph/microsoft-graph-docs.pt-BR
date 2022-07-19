---
title: Atualizar ediscoveryReviewSetQuery
description: Atualize as propriedades de um objeto ediscoveryReviewSetQuery.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 6b20bfe3f2d857e40a274cf0e4ec290cc8dc52c1
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838210"
---
# <a name="update-ediscoveryreviewsetquery"></a>Atualizar ediscoveryReviewSetQuery
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/queries/{queryId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da consulta. Obrigatório.|
|contentQuery|String|A consulta KQL para o conjunto de revisão. Para obter detalhes, [consulte Consultar e filtrar conteúdo em um conjunto de revisão](/microsoft-365/compliance/review-set-search).|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "update_ediscoveryreviewsetquery"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/cases/ediscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/63ef0fd7-0db2-45eb-a9d7-7d75c8239873/queries/5f426fdc-f027-40db-b7cc-453cf06dc996
Content-Type: application/json

{
    "displayName": "My Query 1 (update)",
    "contentQuery": "(Author=\"edisons\")"
}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No content.
```
