---
title: 'educationUser: delta'
description: Obter usuários recém-criados ou atualizados sem precisar executar uma leitura completa de todo o conjunto de usuários.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7477bea6eeb01e74cb824a7d31b0cc5dba3161ef
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042923"
---
# <a name="educationuser-delta"></a><span data-ttu-id="c90d0-103">educationUser: delta</span><span class="sxs-lookup"><span data-stu-id="c90d0-103">educationUser: delta</span></span>

<span data-ttu-id="c90d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c90d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c90d0-105">Get newly created or [updated educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span><span class="sxs-lookup"><span data-stu-id="c90d0-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="c90d0-106">Consulte [Usar consulta delta para](/graph/delta-query-overview) obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="c90d0-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="c90d0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c90d0-107">Permissions</span></span>

<span data-ttu-id="c90d0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c90d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c90d0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c90d0-110">Permission type</span></span>                        | <span data-ttu-id="c90d0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c90d0-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="c90d0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c90d0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c90d0-113">EduRoster.ReadBasic, EduRoster.Read ou EduRoster.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c90d0-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="c90d0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c90d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c90d0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c90d0-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="c90d0-116">Application</span><span class="sxs-lookup"><span data-stu-id="c90d0-116">Application</span></span>                            | <span data-ttu-id="c90d0-117">EduRoster.ReadBasic.All, EduRoster.Read.All ou EduRoster.WriteWrite.All</span><span class="sxs-lookup"><span data-stu-id="c90d0-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c90d0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c90d0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/users/delta
```

## <a name="request-headers"></a><span data-ttu-id="c90d0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c90d0-119">Request headers</span></span>

| <span data-ttu-id="c90d0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c90d0-120">Name</span></span>          | <span data-ttu-id="c90d0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c90d0-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="c90d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c90d0-122">Authorization</span></span> | <span data-ttu-id="c90d0-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c90d0-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c90d0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c90d0-124">Request body</span></span>

<span data-ttu-id="c90d0-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c90d0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c90d0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c90d0-126">Response</span></span>

<span data-ttu-id="c90d0-127">Se tiver êxito, este método retornará um código de resposta e um objeto da coleção `200 OK` [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c90d0-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c90d0-128">educationUser deltas não incluem usuários excluídos.</span><span class="sxs-lookup"><span data-stu-id="c90d0-128">educationUser deltas do not include deleted users.</span></span>

## <a name="example"></a><span data-ttu-id="c90d0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c90d0-129">Example</span></span>

<span data-ttu-id="c90d0-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c90d0-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c90d0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c90d0-131">Request</span></span>

<span data-ttu-id="c90d0-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c90d0-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c90d0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c90d0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/delta
```
# <a name="c"></a>[<span data-ttu-id="c90d0-134">C#</span><span class="sxs-lookup"><span data-stu-id="c90d0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationuser-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c90d0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c90d0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationuser-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c90d0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c90d0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationuser-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c90d0-137">Java</span><span class="sxs-lookup"><span data-stu-id="c90d0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationuser-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c90d0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c90d0-138">Response</span></span>

<span data-ttu-id="c90d0-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c90d0-139">The following is an example of the response.</span></span>

> <span data-ttu-id="c90d0-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c90d0-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


