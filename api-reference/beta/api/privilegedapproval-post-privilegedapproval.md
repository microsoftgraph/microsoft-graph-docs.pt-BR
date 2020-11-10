---
title: Create privilegedApproval
description: Use esta API para criar um novo privilegedApproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 8d6bbd41b171f63914fb55f3ba4c2a8e8185ed3a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970462"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="2ff84-103">Create privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="2ff84-103">Create privilegedApproval</span></span>

<span data-ttu-id="2ff84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ff84-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ff84-105">Use esta API para criar um novo privilegedApproval.</span><span class="sxs-lookup"><span data-stu-id="2ff84-105">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ff84-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ff84-106">Permissions</span></span>
<span data-ttu-id="2ff84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ff84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2ff84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ff84-109">Permission type</span></span>      | <span data-ttu-id="2ff84-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ff84-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ff84-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ff84-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ff84-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ff84-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2ff84-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ff84-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ff84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ff84-114">Not supported.</span></span>    |
|<span data-ttu-id="2ff84-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ff84-115">Application</span></span> | <span data-ttu-id="2ff84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ff84-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ff84-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ff84-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="2ff84-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ff84-118">Request headers</span></span>
| <span data-ttu-id="2ff84-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2ff84-119">Name</span></span>       | <span data-ttu-id="2ff84-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ff84-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ff84-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ff84-121">Authorization</span></span>  | <span data-ttu-id="2ff84-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ff84-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ff84-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ff84-124">Request body</span></span>
<span data-ttu-id="2ff84-125">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedApproval](../resources/privilegedapproval.md) .</span><span class="sxs-lookup"><span data-stu-id="2ff84-125">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2ff84-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ff84-126">Response</span></span>

<span data-ttu-id="2ff84-127">Se bem-sucedido, este método retorna o `201 Created` código de resposta e o objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ff84-127">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="2ff84-128">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="2ff84-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2ff84-129">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="2ff84-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="2ff84-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ff84-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ff84-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ff84-131">Request</span></span>
<span data-ttu-id="2ff84-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ff84-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ff84-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ff84-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2ff84-134">C#</span><span class="sxs-lookup"><span data-stu-id="2ff84-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ff84-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ff84-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ff84-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ff84-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ff84-137">Java</span><span class="sxs-lookup"><span data-stu-id="2ff84-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedapproval-from-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2ff84-138">No corpo da solicitação, forneça uma representação JSON do objeto [privilegedApproval](../resources/privilegedapproval.md) .</span><span class="sxs-lookup"><span data-stu-id="2ff84-138">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2ff84-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ff84-139">Response</span></span>
<span data-ttu-id="2ff84-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ff84-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


