---
title: 'privilegedRole: selfDeactivate'
description: Desative a função que é atribuída ao solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: ea2d8f9a34b2cf4defad6865518044d7908266d4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218742"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="235ab-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="235ab-103">privilegedRole: selfDeactivate</span></span>

<span data-ttu-id="235ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="235ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="235ab-105">Desative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="235ab-105">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="235ab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="235ab-106">Permissions</span></span>
<span data-ttu-id="235ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="235ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="235ab-109">O solicitante só pode chamar ```selfDeactivate``` a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="235ab-109">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="235ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="235ab-110">Permission type</span></span>      | <span data-ttu-id="235ab-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="235ab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="235ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="235ab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="235ab-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="235ab-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="235ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="235ab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="235ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="235ab-115">Not supported.</span></span>    |
|<span data-ttu-id="235ab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="235ab-116">Application</span></span> | <span data-ttu-id="235ab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="235ab-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="235ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="235ab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="235ab-119">Observe que ``{id}`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="235ab-119">Note that ``{id}`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="235ab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="235ab-120">Request headers</span></span>
| <span data-ttu-id="235ab-121">Nome</span><span class="sxs-lookup"><span data-stu-id="235ab-121">Name</span></span>       | <span data-ttu-id="235ab-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="235ab-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="235ab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="235ab-123">Authorization</span></span>  | <span data-ttu-id="235ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="235ab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="235ab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="235ab-126">Request body</span></span>
<span data-ttu-id="235ab-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="235ab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="235ab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="235ab-128">Response</span></span>

<span data-ttu-id="235ab-129">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="235ab-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="235ab-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="235ab-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="235ab-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="235ab-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="235ab-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="235ab-132">Example</span></span>
<span data-ttu-id="235ab-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="235ab-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="235ab-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="235ab-134">Request</span></span>
<span data-ttu-id="235ab-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="235ab-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="235ab-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="235ab-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="c"></a>[<span data-ttu-id="235ab-137">C#</span><span class="sxs-lookup"><span data-stu-id="235ab-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="235ab-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="235ab-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="235ab-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="235ab-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="235ab-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="235ab-140">Response</span></span>
<span data-ttu-id="235ab-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="235ab-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
