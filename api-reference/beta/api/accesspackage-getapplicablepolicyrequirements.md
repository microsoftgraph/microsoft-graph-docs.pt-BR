---
title: 'accessPackage: getApplicablePolicyRequirements'
description: Permitir que os chamadores encontrem requisitos para solicitar uma atribuição para um accessPackage específico.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b158fcfee76d583bd2b44baa1216badf4494f8a9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791914"
---
# <a name="accesspackage-getapplicablepolicyrequirements"></a>accessPackage: getApplicablePolicyRequirements
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-overview.md)essa ação recupera uma lista de objetos [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) que o usuário atualmente está assinado pode usar para criar um [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).  Cada objeto de requisito corresponde a uma política de atribuição de pacote de acesso para a que o usuário atualmente está autorizado a solicitar uma atribuição.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/getApplicablePolicyRequirements
```

## <a name="function-parameters"></a>Parâmetros de função

Nenhum.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não fornece um corpo de solicitação para esse método se quiser recuperar uma lista de requisitos de pacote de acesso, como no exemplo 1. Se você quiser obter requisitos de política para o escopo do usuário, como no exemplo 2, deverá fornecer um corpo da solicitação.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) no corpo da resposta, um objeto para cada política para a qual o usuário é **um allowedRequestor**. Se houver uma política sem requisitos, **o accessPackageAssignmentRequestRequirements** terá `false` e `null` valores. Se não houver políticas em que o usuário seja **um allowedRequestor**, uma coleção vazia será retornada.

## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-a-list-of-access-package-requirements-to-create-an-access-package"></a>Exemplo 1: recuperar uma lista de requisitos de pacote de acesso para criar um pacote de acesso

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackage_getapplicablepolicyrequirements"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/fb449cf8-3a59-4d86-bdfd-a1b7299681de/getApplicablePolicyRequirements
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackage-getapplicablepolicyrequirements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackage-getapplicablepolicyrequirements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackage-getapplicablepolicyrequirements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackage-getapplicablepolicyrequirements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accesspackage-getapplicablepolicyrequirements-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequestRequirements)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "policyId": "d6322c23-04d6-eb11-b22b-c8d9d21f4e9a",
            "policyDisplayName": "Initial Policy",
            "policyDescription": "Initial Policy",
            "isApprovalRequired": false,
            "isApprovalRequiredForExtension": false,
            "isRequestorJustificationRequired": false,
            "questions": [
                {
                    "@odata.type": "#microsoft.graph.textInputQuestion",
                    "id": "0fd349e2-a3a7-4712-af08-660f29c12b90",
                    "isRequired": true,
                    "isAnswerEditable": null,
                    "sequence": 0,
                    "isSingleLineQuestion": true,
                    "text": {
                        "defaultText": "What is your display name",
                        "localizedTexts": []
                    }
                }
            ],
            "existingAnswers": [],
            "schedule": []
        }
    ]
}
``` 

### <a name="example-2-get-policy-requirements-for-a-given-user-scope"></a>Exemplo 2: Obter requisitos de política para um determinado escopo de usuário

#### <a name="request"></a>Solicitação

<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/entitlementManagement/accessPackages(‘b15419bb-5ffc-ea11-b207-c8d9d21f4e9a’)/getApplicablePolicyRequirements

{
        "subject": {
            "objectId": "5acd375c-8acb-45de-a958-fa0dd89259ad"
        }
    }
```



#### <a name="response"></a>Resposta

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "policyId": "d6322c23-04d6-eb11-b22b-c8d9d21f4e9a",
            "policyDisplayName": "Initial Policy",
            "policyDescription": "Initial Policy",
            "isApprovalRequired": false,
            "isApprovalRequiredForExtension": false,
            "isRequestorJustificationRequired": false,
            "questions": [
                {
                    "@odata.type": "#microsoft.graph.textInputQuestion",
                    "id": "5a7f2a8f-b802-4438-bec6-09599bc43e13",
                    "isRequired": false,
                    "isAnswerEditable": true,
                    "sequence": 0,
                    "isSingleLineQuestion": true,
                    "text": {
                        "defaultText": "Enter your mail",
                        "localizedTexts": []
                    }
                }
            ],
            "existingAnswers": [
                {
                    "@odata.type": "#microsoft.graph.answerString",
                    "displayValue": "admin@contoso.com",
                    "value": "admin@contoso.com",
                    "answeredQuestion": {
                        "@odata.type": "#microsoft.graph.textInputQuestion",
                        "id": "5a7f2a8f-b802-4438-bec6-09599bc43e13",
                        "isRequired": false,
                        "isAnswerEditable": true,
                        "sequence": 0,
                        "isSingleLineQuestion": true,
                        "text": {
                            "defaultText": "Enter your mail",
                            "localizedTexts": []
                        }
                    }
                }
            ],
            "schedule": []
        }
    ]
}
```
