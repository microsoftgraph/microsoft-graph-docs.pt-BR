---
title: Definições de lista
description: Liste os objetos teamTemplateDefinition associados a um teamTemplate.
author: Charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 5e4b629399fa8e8e927028f4c212e8438ba1fa6f
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690100"
---
# <a name="list-definitions"></a>Definições de lista
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Liste [os objetos teamTemplateDefinition](../resources/teamstemplate.md) associados a um [teamTemplate](../resources/teamtemplate.md). 

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Team.Create|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|Team.Create|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/teamTemplates?$expand=definitions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte ao `$expand`parâmetro de consulta , `$filter`e `$skipToken` [OData](/graph/query-parameters) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de [objetos teamTemplateDefinition](../resources/teamtemplatedefinition.md) . 

## <a name="examples"></a>Exemplos

### <a name="example-1-use-extend-and-filter-to-get-teamtemplatedefinitions-for-en-us-locale"></a>Exemplo 1: usar $extend e $filter obter teamTemplateDefinitions para localidade en-US

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "name": "list_teamtemplatedefinitions"
}
-->
```http
GET https://graph.microsoft.com/beta/teamwork/teamTemplates?$expand=definitions&filter=definitions/any(a:a/languageTag eq 'en-US')
```

#### <a name="response"></a>Resposta
A seguir está um exemplo da resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamtemplatedefinition)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "id": "com.microsoft.teams.template.ManageAProject",
            "definitions": [
                {
                    "id": "Y29tLm1pY3Jvc29mdC50ZWFtcy50ZW1wbGF0ZS5NYW5hZ2VBUHJvamVjdCMjUHVibGljIyNlbi1VUw==",
                    "parentTemplateId": "com.microsoft.teams.template.ManageAProject",
                    "displayName": "Manage a Project",
                    "languageTag": "en-US",
                    "audience": "public",
                    "description": "Manage tasks, share documents, conduct project meetings and document risks and decisions with this template for general project management.",
                    "shortDescription": "Coordinate your project.",
                    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
                    "publisherName": "Microsoft",
                    "categories": [
                        "General"
                    ],
                    "lastModifiedBy": null
                }
            ]
        },
        {
            "id": "com.microsoft.teams.template.ManageAnEvent",
            "definitions": [
                {
                    "id": "Y29tLm1pY3Jvc29mdC50ZWFtcy50ZW1wbGF0ZS5NYW5hZ2VBbkV2ZW50IyNQdWJsaWMjI2VuLVVT",
                    "parentTemplateId": "com.microsoft.teams.template.ManageAnEvent",
                    "displayName": "Manage an Event",
                    "languageTag": "en-US",
                    "audience": "public",
                    "description": "Manage tasks, documents, and collaborate on everything you need to deliver a compelling event. Invite guest users to have a secure collaboration inside and outside of your company.",
                    "shortDescription": "Improve your event management and collaboration.",
                    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
                    "publisherName": "Microsoft",
                    "categories": [
                        "General"
                    ],
                    "lastModifiedBy": null
                }
            ]
        },
    ]
}
```
