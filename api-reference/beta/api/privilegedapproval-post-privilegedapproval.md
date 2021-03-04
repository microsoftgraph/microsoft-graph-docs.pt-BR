---
title: Create privilegedApproval
description: Use essa API para criar um novo privilegedApproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: ef3581fef523f14d5f84bb0f1859795860624c45
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442240"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="4dfd6-103">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="4dfd6-103">Create privilegedApproval</span></span>

<span data-ttu-id="4dfd6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dfd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dfd6-105">Use essa API para criar um novo privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="4dfd6-105">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="4dfd6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4dfd6-106">Permissions</span></span>
<span data-ttu-id="4dfd6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dfd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4dfd6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dfd6-109">Permission type</span></span>      | <span data-ttu-id="4dfd6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4dfd6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dfd6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dfd6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4dfd6-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4dfd6-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4dfd6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dfd6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dfd6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dfd6-114">Not supported.</span></span>    |
|<span data-ttu-id="4dfd6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dfd6-115">Application</span></span> | <span data-ttu-id="4dfd6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dfd6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dfd6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dfd6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="4dfd6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dfd6-118">Request headers</span></span>
| <span data-ttu-id="4dfd6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4dfd6-119">Name</span></span>       | <span data-ttu-id="4dfd6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dfd6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4dfd6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dfd6-121">Authorization</span></span>  | <span data-ttu-id="4dfd6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dfd6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4dfd6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dfd6-124">Request body</span></span>
<span data-ttu-id="4dfd6-125">No corpo da solicitação, fornece uma representação JSON [do objeto privilegedApproval.](../resources/privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="4dfd6-125">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4dfd6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dfd6-126">Response</span></span>

<span data-ttu-id="4dfd6-127">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4dfd6-127">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="4dfd6-128">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="4dfd6-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4dfd6-129">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="4dfd6-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="4dfd6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dfd6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4dfd6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dfd6-131">Request</span></span>
<span data-ttu-id="4dfd6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dfd6-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4dfd6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4dfd6-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4dfd6-134">C#</span><span class="sxs-lookup"><span data-stu-id="4dfd6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4dfd6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4dfd6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4dfd6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4dfd6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4dfd6-137">Java</span><span class="sxs-lookup"><span data-stu-id="4dfd6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedapproval-from-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4dfd6-138">No corpo da solicitação, fornece uma representação JSON [do objeto privilegedApproval.](../resources/privilegedapproval.md)</span><span class="sxs-lookup"><span data-stu-id="4dfd6-138">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4dfd6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dfd6-139">Response</span></span>
<span data-ttu-id="4dfd6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4dfd6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


