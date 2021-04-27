---
title: Atualizar unifiedRoleAssignmentMultiple
description: Atualize um novo objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5bd8485a9b01890420d47e95d976b84b0807b488
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054746"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="7e00b-103">Atualizar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="7e00b-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="7e00b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e00b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e00b-105">Atualize um [objeto unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) existente.</span><span class="sxs-lookup"><span data-stu-id="7e00b-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="7e00b-106">Use isso para atualizar as atribuições de função Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="7e00b-106">Use this to update role assignments in Microsoft Intune.</span></span> <span data-ttu-id="7e00b-107">Observe que [unifiedRoleAssignment](../resources/unifiedroleassignment.md) não dá suporte à atualização.</span><span class="sxs-lookup"><span data-stu-id="7e00b-107">Note that [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e00b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e00b-108">Permissions</span></span>

<span data-ttu-id="7e00b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e00b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e00b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e00b-111">Permission type</span></span> | <span data-ttu-id="7e00b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e00b-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="7e00b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e00b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7e00b-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e00b-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="7e00b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e00b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e00b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e00b-116">Not supported.</span></span> |
| <span data-ttu-id="7e00b-117">Application</span><span class="sxs-lookup"><span data-stu-id="7e00b-117">Application</span></span> | <span data-ttu-id="7e00b-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e00b-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e00b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e00b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="7e00b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e00b-120">Request headers</span></span>

| <span data-ttu-id="7e00b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7e00b-121">Name</span></span> | <span data-ttu-id="7e00b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e00b-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="7e00b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e00b-123">Authorization</span></span> | <span data-ttu-id="7e00b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e00b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e00b-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="7e00b-126">Content-type</span></span> | <span data-ttu-id="7e00b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e00b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e00b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e00b-129">Request body</span></span>

<span data-ttu-id="7e00b-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7e00b-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7e00b-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="7e00b-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7e00b-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7e00b-132">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="7e00b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e00b-133">Response</span></span>

<span data-ttu-id="7e00b-134">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e00b-134">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e00b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e00b-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e00b-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e00b-136">Request</span></span>

<span data-ttu-id="7e00b-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e00b-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7e00b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e00b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
Content-type: application/json

{ 
    "principalIds": ["0aeec2c1-fee7-4e02-b534-6f920d25b300", "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"]
}
```
# <a name="c"></a>[<span data-ttu-id="7e00b-139">C#</span><span class="sxs-lookup"><span data-stu-id="7e00b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e00b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e00b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e00b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e00b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e00b-142">Java</span><span class="sxs-lookup"><span data-stu-id="7e00b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7e00b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e00b-143">Response</span></span>

<span data-ttu-id="7e00b-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7e00b-144">The following is an example of the response.</span></span>
> <span data-ttu-id="7e00b-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7e00b-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 204 OK

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


