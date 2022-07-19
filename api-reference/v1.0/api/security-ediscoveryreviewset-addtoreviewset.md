---
title: 'ediscoveryReviewSet: addToReviewSet'
description: Inicie o processo de adição de uma coleção de serviços do Microsoft 365 a um conjunto de revisão.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 30d4093704cc683f97f9dfb4334b193341bf4fad
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839104"
---
# <a name="ediscoveryreviewset-addtoreviewset"></a>ediscoveryReviewSet: addToReviewSet
Namespace: microsoft.graph.security



Inicie o processo de adição de uma coleção de serviços do Microsoft 365 a um [conjunto de revisão](../resources/security-ediscoveryreviewset.md). Depois que a operação for criada, você poderá obter o status `Location` da operação recuperando o parâmetro dos cabeçalhos de resposta. O local fornece uma URL que retornará uma operação [Adicionar ao conjunto de revisão](../resources/security-ediscoveryaddtoreviewsetoperation.md).


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
POST /security/cases/ediscoverycases/{eDiscoveryCaseId}/reviewSets/{eDiscoveryReviewSetId}/addToReviewSet
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|search|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|A ID da pesquisa de Descoberta Eletrônica que você deseja adicionar ao conjunto de revisão.|
|additionalDataOptions|additionalDataOptions|As opções para adicionar itens ao reviewSet.|

### <a name="additionaldataoptions-values"></a>valores additionalDataOptions
|Nome|Descrição|
|:---|:---|
|allVersions|incluem todas as versões de um documento do SharePoint correspondentes à consulta de coleção de origem. Cuidado: as versões do SharePoint podem aumentar significativamente o volume de itens |
|linkedFiles|incluem arquivos vinculados que foram compartilhados no Outlook, equipes ou mensagens do Yammer anexando um link ao arquivo.|

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetthis.addtoreviewset"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/ediscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/63ef0fd7-0db2-45eb-a9d7-7d75c8239873/addToReviewSet
Content-Type: application/json

{
    "search": {
        "id": "c17e91d6-6bc0-4ecb-b388-269ea3d4ffb7"
    },
    "additionalDataOptions": "linkedFiles"
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
HTTP/1.1 202 Accepted
```