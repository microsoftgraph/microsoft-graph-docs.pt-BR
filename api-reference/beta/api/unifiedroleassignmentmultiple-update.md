---
title: Atualizar unifiedRoleAssignmentMultiple
description: Atualize um novo objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: af1749b0def974fab47bfe3403f4e53e83f65b52
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978882"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="c614a-103">Atualizar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="c614a-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="c614a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c614a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c614a-105">Atualize um objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) existente.</span><span class="sxs-lookup"><span data-stu-id="c614a-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="c614a-106">Use esta atualização para atualizar as atribuições de função no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="c614a-106">Use this to update role assignments in Microsoft Intune.</span></span> <span data-ttu-id="c614a-107">Observe que o [unifiedRoleAssignment](../resources/unifiedroleassignment.md) não é compatível com a atualização.</span><span class="sxs-lookup"><span data-stu-id="c614a-107">Note that [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="c614a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c614a-108">Permissions</span></span>

<span data-ttu-id="c614a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c614a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c614a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c614a-111">Permission type</span></span> | <span data-ttu-id="c614a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c614a-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="c614a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c614a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c614a-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c614a-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="c614a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c614a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c614a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c614a-116">Not supported.</span></span> |
| <span data-ttu-id="c614a-117">Application</span><span class="sxs-lookup"><span data-stu-id="c614a-117">Application</span></span> | <span data-ttu-id="c614a-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c614a-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c614a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c614a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c614a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c614a-120">Request headers</span></span>

| <span data-ttu-id="c614a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c614a-121">Name</span></span> | <span data-ttu-id="c614a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c614a-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="c614a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c614a-123">Authorization</span></span> | <span data-ttu-id="c614a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c614a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c614a-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="c614a-126">Content-type</span></span> | <span data-ttu-id="c614a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c614a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c614a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c614a-129">Request body</span></span>

<span data-ttu-id="c614a-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c614a-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c614a-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c614a-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c614a-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c614a-132">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="c614a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c614a-133">Response</span></span>

<span data-ttu-id="c614a-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c614a-134">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c614a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c614a-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="c614a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c614a-136">Request</span></span>

<span data-ttu-id="c614a-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c614a-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c614a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c614a-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c614a-139">C#</span><span class="sxs-lookup"><span data-stu-id="c614a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c614a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c614a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c614a-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c614a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c614a-142">Java</span><span class="sxs-lookup"><span data-stu-id="c614a-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c614a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c614a-143">Response</span></span>

<span data-ttu-id="c614a-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c614a-144">The following is an example of the response.</span></span>
> <span data-ttu-id="c614a-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c614a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


