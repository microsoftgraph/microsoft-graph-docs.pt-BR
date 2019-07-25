---
title: Create privilegedApproval
description: Use esta API para criar um novo privilegedApproval.
localization_priority: Normal
ms.openlocfilehash: 82e265e5b76c9649445b3e6d4edaf035cbddbc82
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875885"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="afb14-103">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="afb14-103">Create privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afb14-104">Use esta API para criar um novo privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="afb14-104">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="afb14-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="afb14-105">Permissions</span></span>
<span data-ttu-id="afb14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afb14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="afb14-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afb14-108">Permission type</span></span>      | <span data-ttu-id="afb14-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="afb14-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afb14-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afb14-110">Delegated (work or school account)</span></span> | <span data-ttu-id="afb14-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="afb14-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="afb14-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afb14-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afb14-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afb14-113">Not supported.</span></span>    |
|<span data-ttu-id="afb14-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afb14-114">Application</span></span> | <span data-ttu-id="afb14-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afb14-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="afb14-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afb14-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="afb14-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afb14-117">Request headers</span></span>
| <span data-ttu-id="afb14-118">Nome</span><span class="sxs-lookup"><span data-stu-id="afb14-118">Name</span></span>       | <span data-ttu-id="afb14-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="afb14-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="afb14-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="afb14-120">Authorization</span></span>  | <span data-ttu-id="afb14-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afb14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afb14-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afb14-123">Request body</span></span>
<span data-ttu-id="afb14-124">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedApproval](../resources/privilegedapproval.md) .</span><span class="sxs-lookup"><span data-stu-id="afb14-124">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="afb14-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="afb14-125">Response</span></span>

<span data-ttu-id="afb14-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afb14-126">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="afb14-127">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="afb14-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="afb14-128">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="afb14-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="afb14-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afb14-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afb14-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afb14-130">Request</span></span>
<span data-ttu-id="afb14-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afb14-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="afb14-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="afb14-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="afb14-133">C#</span><span class="sxs-lookup"><span data-stu-id="afb14-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="afb14-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="afb14-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="afb14-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="afb14-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="afb14-136">Java</span><span class="sxs-lookup"><span data-stu-id="afb14-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedapproval-from-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="afb14-137">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedApproval](../resources/privilegedapproval.md) .</span><span class="sxs-lookup"><span data-stu-id="afb14-137">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="afb14-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="afb14-138">Response</span></span>
<span data-ttu-id="afb14-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afb14-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
