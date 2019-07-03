---
title: 'privilegedRole: selfDeactivate'
description: Desative a função que é atribuída ao solicitante.
localization_priority: Normal
ms.openlocfilehash: 66c74f643e597bb8effae64d91159c3d3ac3a43d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445013"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="64cd5-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="64cd5-103">privilegedRole: selfDeactivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64cd5-104">Desative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="64cd5-104">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="64cd5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="64cd5-105">Permissions</span></span>
<span data-ttu-id="64cd5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64cd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="64cd5-108">O solicitante só pode chamar ```selfDeactivate``` a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="64cd5-108">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="64cd5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64cd5-109">Permission type</span></span>      | <span data-ttu-id="64cd5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64cd5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64cd5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64cd5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64cd5-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64cd5-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64cd5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64cd5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64cd5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64cd5-114">Not supported.</span></span>    |
|<span data-ttu-id="64cd5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64cd5-115">Application</span></span> | <span data-ttu-id="64cd5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64cd5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64cd5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64cd5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="64cd5-118">Observe que ``<id>`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="64cd5-118">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="64cd5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64cd5-119">Request headers</span></span>
| <span data-ttu-id="64cd5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="64cd5-120">Name</span></span>       | <span data-ttu-id="64cd5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="64cd5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64cd5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="64cd5-122">Authorization</span></span>  | <span data-ttu-id="64cd5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64cd5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64cd5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64cd5-125">Request body</span></span>
<span data-ttu-id="64cd5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64cd5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64cd5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="64cd5-127">Response</span></span>

<span data-ttu-id="64cd5-128">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64cd5-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="64cd5-129">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="64cd5-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="64cd5-130">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="64cd5-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="64cd5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64cd5-131">Example</span></span>
<span data-ttu-id="64cd5-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="64cd5-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="64cd5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64cd5-133">Request</span></span>
<span data-ttu-id="64cd5-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64cd5-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="64cd5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="64cd5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64cd5-136">C#</span><span class="sxs-lookup"><span data-stu-id="64cd5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64cd5-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="64cd5-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64cd5-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="64cd5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64cd5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="64cd5-139">Response</span></span>
<span data-ttu-id="64cd5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64cd5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
