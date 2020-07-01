---
title: 'educationUser: Delta'
description: Obter usuários recém-criados ou atualizados sem ter que realizar uma leitura completa de toda a coleção de usuários.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3d96334c4a7f3fd6974fdf08c2eb86809e89326d
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006825"
---
# <a name="educationuser-delta"></a><span data-ttu-id="75705-103">educationUser: Delta</span><span class="sxs-lookup"><span data-stu-id="75705-103">educationUser: delta</span></span>

<span data-ttu-id="75705-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75705-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75705-105">Obter [educationUser](../resources/educationuser.md) recentemente criados ou atualizados sem ter que realizar uma leitura completa de toda a coleção.</span><span class="sxs-lookup"><span data-stu-id="75705-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="75705-106">Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="75705-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="75705-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="75705-107">Permissions</span></span>

<span data-ttu-id="75705-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="75705-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="75705-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75705-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75705-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75705-110">Permission type</span></span>                        | <span data-ttu-id="75705-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75705-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="75705-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75705-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="75705-113">EduRoster. ReadBasic, EduRoster. Read ou EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75705-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="75705-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75705-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75705-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75705-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="75705-116">Application</span><span class="sxs-lookup"><span data-stu-id="75705-116">Application</span></span>                            | <span data-ttu-id="75705-117">EduRoster. ReadBasic. All, EduRoster. Read. All ou EduRoster. WriteWrite. All</span><span class="sxs-lookup"><span data-stu-id="75705-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75705-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75705-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/users/delta
```

## <a name="request-headers"></a><span data-ttu-id="75705-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75705-119">Request headers</span></span>

| <span data-ttu-id="75705-120">Nome</span><span class="sxs-lookup"><span data-stu-id="75705-120">Name</span></span>          | <span data-ttu-id="75705-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="75705-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="75705-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75705-122">Authorization</span></span> | <span data-ttu-id="75705-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="75705-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="75705-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75705-124">Request body</span></span>

<span data-ttu-id="75705-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75705-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75705-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="75705-126">Response</span></span>

<span data-ttu-id="75705-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75705-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="75705-128">educationUser deltas não incluem usuários excluídos.</span><span class="sxs-lookup"><span data-stu-id="75705-128">educationUser deltas do not include deleted users.</span></span>

## <a name="example"></a><span data-ttu-id="75705-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75705-129">Example</span></span>

<span data-ttu-id="75705-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="75705-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="75705-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75705-131">Request</span></span>

<span data-ttu-id="75705-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="75705-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
GET https://graph.microsoft.com/beta/education/users/delta
```

### <a name="response"></a><span data-ttu-id="75705-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="75705-133">Response</span></span>

<span data-ttu-id="75705-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="75705-134">The following is an example of the response.</span></span>

> <span data-ttu-id="75705-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="75705-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="75705-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="75705-136">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1039

{
  "value": [
    {
      "accountEnabled": true,
      "assignedLicenses": [{ "@odata.type": "microsoft.graph.assignedLicense" }],
      "assignedPlans": [{ "@odata.type": "microsoft.graph.assignedPlan" }],
      "businessPhones": ["String"],
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "department": "String",
      "displayName": "String",
      "externalSource": "string",
      "givenName": "String",
      "id": "String (identifier)",
      "mail": "String",
      "mailNickname": "String",
      "mailingAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
      "middleName": "String",
      "mobilePhone": "String",
      "officeLocation": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      },
      "passwordPolicies": "String",
      "passwordProfile": { "@odata.type": "microsoft.graph.passwordProfile" },
      "preferredLanguage": "String",
      "primaryRole": "string",
      "provisionedPlans": [{ "@odata.type": "microsoft.graph.provisionedPlan" }],
      "residenceAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
      "student": { "@odata.type": "microsoft.graph.educationStudent" },
      "surname": "String",
      "teacher": { "@odata.type": "microsoft.graph.educationTeacher" },
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
