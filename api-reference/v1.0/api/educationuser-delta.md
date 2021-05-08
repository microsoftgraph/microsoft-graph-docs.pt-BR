---
title: 'educationUser: delta'
description: Obter usuários recém-criados ou atualizados sem precisar executar uma leitura completa de todo o conjunto de usuários.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eddf1656a9f1366276b89fd5b101768b45e2cca1
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232120"
---
# <a name="educationuser-delta"></a><span data-ttu-id="a3103-103">educationUser: delta</span><span class="sxs-lookup"><span data-stu-id="a3103-103">educationUser: delta</span></span>

<span data-ttu-id="a3103-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3103-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a3103-105">Get newly created or [updated educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span><span class="sxs-lookup"><span data-stu-id="a3103-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="a3103-106">Consulte [Usar consulta delta para](/graph/delta-query-overview) obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="a3103-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3103-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3103-107">Permissions</span></span>

<span data-ttu-id="a3103-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3103-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3103-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3103-110">Permission type</span></span>                        | <span data-ttu-id="a3103-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3103-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a3103-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3103-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3103-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a3103-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="a3103-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3103-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3103-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3103-115">Not supported.</span></span>                              |
| <span data-ttu-id="a3103-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3103-116">Application</span></span>                            | <span data-ttu-id="a3103-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3103-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3103-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3103-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/users/delta
```

## <a name="request-headers"></a><span data-ttu-id="a3103-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3103-119">Request headers</span></span>

| <span data-ttu-id="a3103-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a3103-120">Name</span></span>          | <span data-ttu-id="a3103-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3103-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a3103-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3103-122">Authorization</span></span> | <span data-ttu-id="a3103-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3103-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3103-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3103-125">Request body</span></span>

<span data-ttu-id="a3103-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3103-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3103-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3103-127">Response</span></span>

<span data-ttu-id="a3103-128">Se tiver êxito, essa função retornará um código de resposta e uma coleção `200 OK` [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3103-128">If successful, this function returns a `200 OK` response code and a [educationUser](../resources/educationuser.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3103-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a3103-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3103-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3103-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/users/delta
```

### <a name="response"></a><span data-ttu-id="a3103-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3103-131">Response</span></span>

> <span data-ttu-id="a3103-132">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a3103-132">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationUser)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationUser)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/users/delta?$skiptoken=VwhMSQw1l1O5v2F1ZPm...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationUser",
      "id": "String (identifier)",
      "primaryRole": "String",
      "middleName": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "residenceAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "mailingAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "student": {
        "@odata.type": "microsoft.graph.educationStudent"
      },
      "teacher": {
        "@odata.type": "microsoft.graph.educationTeacher"
      },
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "accountEnabled": "Boolean",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan"
        }
      ],
      "businessPhones": [
        "String"
      ],
      "department": "String",
      "displayName": "String",
      "givenName": "String",
      "mail": "String",
      "mailNickname": "String",
      "mobilePhone": "String",
      "passwordPolicies": "String",
      "passwordProfile": {
        "@odata.type": "microsoft.graph.passwordProfile"
      },
      "officeLocation": "String",
      "preferredLanguage": "String",
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan"
        }
      ],
      "refreshTokensValidFromDateTime": "String (timestamp)",
      "showInAddressList": "Boolean",
      "surname": "String",
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      }
    }
  ]
}
```
