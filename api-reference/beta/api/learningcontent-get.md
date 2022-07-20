---
title: Obter learningContent
description: Leia as propriedades e as relações de um objeto learningContent.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: 563c33930f596f362965899b14a4fc6cc37022a8
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883264"
---
# <a name="get-learningcontent"></a>Obter learningContent
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha o recurso [learningContent](../resources/learningcontent.md) especificado que representa os metadados do conteúdo ingerido do provedor especificado.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|LearningContent.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|LearningContent.Read.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /employeeExperience/learningProviders/{learningProviderId}/learningContents/{externalId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e um [objeto learningContent](../resources/learningcontent.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "get_learningcontent"
}
-->
``` http 
GET /employeeExperience/learningProviders/13727311-e7bb-470d-8b20-6a23d9030d70/learningContents(externalId='LP4471') 
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.learningContent"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#learningProviders('13727311-e7bb-470d-8b20-6a23d9030d70')/learningContents/$entity",
    "externalId": "LP4471",
    "title": "Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle",
    "description": "A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.",
    "contentWebUrl": "https://docs.microsoft.com/en-us/learn/modules/manage-classes-resources-assessment-planning-beedle/",
    "sourceName": "MSLibrary",
    "thumbnailWebUrl": "https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF",
    "languageTag": "en-us",
    "numberOfPages": 10,
    "duration": "PT20M",
    "format": "Book",
    "createdDateTime": "2018-01-01T00:00:00",
    "lastModifiedDateTime": "2021-04-01T04:26:06.1995367Z",
    "contributor": "Scott Simpson",
    "additionalTags": [
        "Create private or public teams",
        "Add members to teams"
    ],
    "skillTags": [
        "Create teams",
        "Teams channels",
        "Teams members"
    ],
    "isActive": true,
    "isPremium": false,
    "isSearchable": true
}
```

