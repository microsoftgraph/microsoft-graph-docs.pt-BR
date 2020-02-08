---
title: 'usuário: reprocessLicenseAssignment'
description: Reprocessar todas as atribuições de licença baseadas em grupo para o usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9136931b08a2e86f582a0272a6be214740562e4b
ms.sourcegitcommit: cea768f767cf27a938b72bb26892d70e3dedaf2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2020
ms.locfileid: "41865764"
---
# <a name="user-reprocesslicenseassignment"></a><span data-ttu-id="90b3f-103">usuário: reprocessLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="90b3f-103">user: reprocessLicenseAssignment</span></span>

<span data-ttu-id="90b3f-104">Reprocessar todas as atribuições de licença baseadas em grupo para o usuário.</span><span class="sxs-lookup"><span data-stu-id="90b3f-104">Reprocess all group-based license assignments for the user.</span></span> <span data-ttu-id="90b3f-105">Para saber mais sobre licenciamento baseado em grupo, confira [o que é licenciamento baseado em grupo no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="90b3f-105">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span> <span data-ttu-id="90b3f-106">Além disso [, consulte identificar e resolver problemas de atribuição de licença para um grupo no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="90b3f-106">Also see [Identify and resolve license assignment problems for a group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) for more details.</span></span>


## <a name="permissions"></a><span data-ttu-id="90b3f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="90b3f-107">Permissions</span></span>
<span data-ttu-id="90b3f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90b3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90b3f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90b3f-110">Permission type</span></span>      | <span data-ttu-id="90b3f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90b3f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90b3f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90b3f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="90b3f-113">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90b3f-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="90b3f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90b3f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90b3f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90b3f-115">Not supported.</span></span>    |
|<span data-ttu-id="90b3f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90b3f-116">Application</span></span> | <span data-ttu-id="90b3f-117">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90b3f-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90b3f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90b3f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/reprocessLicenseAssignment

```
## <a name="request-headers"></a><span data-ttu-id="90b3f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90b3f-119">Request headers</span></span>
| <span data-ttu-id="90b3f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90b3f-120">Header</span></span>       | <span data-ttu-id="90b3f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="90b3f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90b3f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90b3f-122">Authorization</span></span>  | <span data-ttu-id="90b3f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90b3f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90b3f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90b3f-125">Request body</span></span>
<span data-ttu-id="90b3f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90b3f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90b3f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="90b3f-127">Response</span></span>

<span data-ttu-id="90b3f-128">Se bem-sucedido, este método retorna `200 OK` o código de resposta e um objeto [User](../resources/user.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90b3f-128">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90b3f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90b3f-129">Example</span></span>
<span data-ttu-id="90b3f-130">O exemplo a seguir mostra como reprocessar atribuições de licença para o usuário.</span><span class="sxs-lookup"><span data-stu-id="90b3f-130">The following example shows how to reprocess license assignments for the user.</span></span>
### <a name="request"></a><span data-ttu-id="90b3f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90b3f-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="90b3f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="90b3f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reprocessLicenseAssignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment

```

### <a name="response"></a><span data-ttu-id="90b3f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="90b3f-133">Response</span></span>

<span data-ttu-id="90b3f-134">A resposta é o objeto de usuário atualizado.</span><span class="sxs-lookup"><span data-stu-id="90b3f-134">The response is the updated user object.</span></span>

><span data-ttu-id="90b3f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90b3f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
