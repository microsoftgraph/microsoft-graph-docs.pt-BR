---
title: Create privilegedRoleAssignment
description: Use esta API para criar um novo privilegedRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 21f5c2822ccc9396e9130c6ad94c65e3df002a36
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268079"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="5c87f-103">Create privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5c87f-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c87f-104">Use esta API para criar um novo [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5c87f-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5c87f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c87f-105">Permissions</span></span>
<span data-ttu-id="5c87f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c87f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5c87f-108">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="5c87f-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="5c87f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c87f-109">Permission type</span></span>      | <span data-ttu-id="5c87f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c87f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c87f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c87f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c87f-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c87f-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c87f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c87f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c87f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c87f-114">Not supported.</span></span>    |
|<span data-ttu-id="5c87f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c87f-115">Application</span></span> | <span data-ttu-id="5c87f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c87f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c87f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c87f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="5c87f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c87f-118">Request headers</span></span>
| <span data-ttu-id="5c87f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5c87f-119">Name</span></span>       | <span data-ttu-id="5c87f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c87f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5c87f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c87f-121">Authorization</span></span>  | <span data-ttu-id="5c87f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c87f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c87f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c87f-124">Request body</span></span>
<span data-ttu-id="5c87f-125">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5c87f-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5c87f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c87f-126">Response</span></span>

<span data-ttu-id="5c87f-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c87f-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="5c87f-128">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="5c87f-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="5c87f-129">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="5c87f-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="5c87f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c87f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c87f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c87f-131">Request</span></span>
<span data-ttu-id="5c87f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c87f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
<span data-ttu-id="5c87f-133">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5c87f-133">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5c87f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c87f-134">Response</span></span>
<span data-ttu-id="5c87f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c87f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5c87f-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5c87f-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5c87f-139">C#</span><span class="sxs-lookup"><span data-stu-id="5c87f-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_privilegedroleassignment_from_privilegedroleassignments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c87f-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="5c87f-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_privilegedroleassignment_from_privilegedroleassignments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5c87f-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5c87f-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_privilegedroleassignment_from_privilegedroleassignments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
