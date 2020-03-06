---
title: 'usuário: reprocessLicenseAssignment'
description: Reprocessar todas as atribuições de licença baseadas em grupo para o usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c6b66a71f24799323eb2e85480856cd8d1fe8d1d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508937"
---
# <a name="user-reprocesslicenseassignment"></a><span data-ttu-id="22ea4-103">usuário: reprocessLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="22ea4-103">user: reprocessLicenseAssignment</span></span>

<span data-ttu-id="22ea4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22ea4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22ea4-105">Reprocessar todas as atribuições de licença baseadas em grupo para o usuário.</span><span class="sxs-lookup"><span data-stu-id="22ea4-105">Reprocess all group-based license assignments for the user.</span></span> <span data-ttu-id="22ea4-106">Para saber mais sobre licenciamento baseado em grupo, confira [o que é licenciamento baseado em grupo no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="22ea4-106">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span> <span data-ttu-id="22ea4-107">Além disso [, consulte identificar e resolver problemas de atribuição de licença para um grupo no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="22ea4-107">Also see [Identify and resolve license assignment problems for a group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) for more details.</span></span>


## <a name="permissions"></a><span data-ttu-id="22ea4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="22ea4-108">Permissions</span></span>
<span data-ttu-id="22ea4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22ea4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22ea4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22ea4-111">Permission type</span></span>      | <span data-ttu-id="22ea4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22ea4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22ea4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22ea4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="22ea4-114">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22ea4-114">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="22ea4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22ea4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22ea4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22ea4-116">Not supported.</span></span>    |
|<span data-ttu-id="22ea4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22ea4-117">Application</span></span> | <span data-ttu-id="22ea4-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22ea4-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22ea4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22ea4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/reprocessLicenseAssignment

```
## <a name="request-headers"></a><span data-ttu-id="22ea4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22ea4-120">Request headers</span></span>
| <span data-ttu-id="22ea4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22ea4-121">Header</span></span>       | <span data-ttu-id="22ea4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="22ea4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="22ea4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22ea4-123">Authorization</span></span>  | <span data-ttu-id="22ea4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22ea4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="22ea4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22ea4-126">Request body</span></span>
<span data-ttu-id="22ea4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22ea4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22ea4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="22ea4-128">Response</span></span>

<span data-ttu-id="22ea4-129">Se bem-sucedido, este método retorna `200 OK` o código de resposta e um objeto [User](../resources/user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22ea4-129">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22ea4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22ea4-130">Example</span></span>
<span data-ttu-id="22ea4-131">O exemplo a seguir mostra como reprocessar atribuições de licença para o usuário.</span><span class="sxs-lookup"><span data-stu-id="22ea4-131">The following example shows how to reprocess license assignments for the user.</span></span>
### <a name="request"></a><span data-ttu-id="22ea4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22ea4-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="22ea4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="22ea4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reprocessLicenseAssignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment

```
# <a name="c"></a>[<span data-ttu-id="22ea4-134">C#</span><span class="sxs-lookup"><span data-stu-id="22ea4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-reprocesslicenseassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22ea4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22ea4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-reprocesslicenseassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22ea4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22ea4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-reprocesslicenseassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22ea4-137">Java</span><span class="sxs-lookup"><span data-stu-id="22ea4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-reprocesslicenseassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22ea4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="22ea4-138">Response</span></span>

<span data-ttu-id="22ea4-139">A resposta é o objeto de usuário atualizado.</span><span class="sxs-lookup"><span data-stu-id="22ea4-139">The response is the updated user object.</span></span>

><span data-ttu-id="22ea4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22ea4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: reprocessLicenseAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
