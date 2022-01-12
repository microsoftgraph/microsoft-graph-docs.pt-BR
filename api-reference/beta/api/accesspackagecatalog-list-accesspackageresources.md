---
title: Listar accessPackageResources
description: Recupere uma lista de objetos accesspackageresource.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 03592aeb434ba077efb88d83fcc768eb28f7ed05
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791907"
---
# <a name="list-accesspackageresources"></a>Listar accessPackageResources

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recuperar uma lista de [objetos accessPackageResource](../resources/accesspackageresource.md) em [um accessPackageCatalog](../resources/accesspackagecatalog.md).  Para solicitar para adicionar ou remover [um accessPackageResource,](../resources/accesspackageresource.md)use [criar accessPackageResourceRequest](entitlementmanagement-post-accesspackageresourcerequests.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta. Por exemplo, para recuperar os escopos e ambientes de recursos do pacote de acesso para cada recurso, `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` inclua na consulta. Para recuperar as funções disponíveis de um recurso, inclua `$expand=accessPackageResourceRoles` . Para recuperar apenas recursos para aplicativos e não grupos ou sites, `$filter=resourceType eq 'Application'` inclua na consulta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos accessPackageResource](../resources/accesspackageresource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

A seguir está um exemplo da solicitação, usando um filtro para selecionar recursos de um tipo específico e para retornar escopos de `$expand` recurso de cada recurso.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources?$filter=resourceType eq 'Application'&$expand=accessPackageResourceScopes
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accesspackageresources-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
      "accessPackageResourceScopes": [
          {
              "id": "452d78a7-69a5-482d-a82f-859a5169c55e",
              "displayName": "Root",
              "description": "Root Scope",
              "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
              "originSystem": "AadApplication",
              "isRootScope": true
          }
      ],
      "attributes": [
          {
              "id": "4f28e638-93de-4152-b631-2135da14c94a",
              "attributeName": "country",
              "attributeDefaultValue": null,
              "isEditable": true,
              "isPersistedOnAssignmentRemoval": false,
              "attributeSource": {
                  "@odata.type": "#microsoft.graph.resourceAttributeQuestion",
                  "question": {
                      "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
                      "id": "6c797e12-e608-4ac9-90da-a8f18df37a94",
                      "isRequired": false,
                      "isAnswerEditable": null,
                      "sequence": 0,
                      "allowsMultipleSelection": false,
                      "text": {
                          "defaultText": "Enter your country",
                          "localizedTexts": []
                      },
                      "choices": [
                          {
                              "actualValue": "USA",
                              "displayValue": {
                                  "defaultText": "USA",
                                  "localizedTexts": [
                                      {
                                          "text": "USA",
                                          "languageCode": "en-US"
                                      }
                                  ]
                              }
                          },
                          {
                              "actualValue": "Canada",
                              "displayValue": {
                                  "defaultText": "Canada",
                                  "localizedTexts": [
                                      {
                                          "text": "Canada",
                                          "languageCode": "en-US"
                                      }
                                  ]
                              }
                          },
                          {
                              "actualValue": "India",
                              "displayValue": {
                                  "defaultText": "India",
                                  "localizedTexts": [
                                      {
                                          "text": "English",
                                          "languageCode": "en-US"
                                      }
                                  ]
                              }
                          }
                      ]
                  }
              },
              "attributeDestination": {
                  "@odata.type": "#microsoft.graph.userDirectoryAttributeStore"
              }
          }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
