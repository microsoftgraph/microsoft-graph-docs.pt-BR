---
title: 'privilegedRole: selfDeactivate'
description: Desative a função que é atribuída ao solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a50f74e928d95ba5bce5e39dc61febb30f9d67b7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441281"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="40395-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="40395-103">privilegedRole: selfDeactivate</span></span>

<span data-ttu-id="40395-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40395-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40395-105">Desative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="40395-105">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="40395-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="40395-106">Permissions</span></span>
<span data-ttu-id="40395-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="40395-109">O solicitante só pode ```selfDeactivate``` chamar a função atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="40395-109">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="40395-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40395-110">Permission type</span></span>      | <span data-ttu-id="40395-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40395-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40395-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40395-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40395-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40395-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="40395-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40395-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40395-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40395-115">Not supported.</span></span>    |
|<span data-ttu-id="40395-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40395-116">Application</span></span> | <span data-ttu-id="40395-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40395-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40395-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40395-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="40395-119">Observe que ``{id}`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="40395-119">Note that ``{id}`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="40395-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40395-120">Request headers</span></span>
| <span data-ttu-id="40395-121">Nome</span><span class="sxs-lookup"><span data-stu-id="40395-121">Name</span></span>       | <span data-ttu-id="40395-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="40395-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="40395-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="40395-123">Authorization</span></span>  | <span data-ttu-id="40395-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40395-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40395-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40395-126">Request body</span></span>
<span data-ttu-id="40395-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40395-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40395-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="40395-128">Response</span></span>

<span data-ttu-id="40395-129">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40395-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="40395-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="40395-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="40395-131">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="40395-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="40395-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40395-132">Example</span></span>
<span data-ttu-id="40395-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="40395-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="40395-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40395-134">Request</span></span>
<span data-ttu-id="40395-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40395-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40395-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="40395-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="c"></a>[<span data-ttu-id="40395-137">C#</span><span class="sxs-lookup"><span data-stu-id="40395-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40395-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40395-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40395-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40395-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40395-140">Java</span><span class="sxs-lookup"><span data-stu-id="40395-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfdeactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="40395-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="40395-141">Response</span></span>
<span data-ttu-id="40395-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40395-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


