---
title: 'privilegedApproval: myrequests'
description: Receba solicitações de aprovação do solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 8be41edff2c2c9163f26238ef0dd23bb61ea5170
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218798"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="f1568-103">privilegedApproval: myrequests</span><span class="sxs-lookup"><span data-stu-id="f1568-103">privilegedApproval: myRequests</span></span>

<span data-ttu-id="f1568-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1568-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1568-105">Receba solicitações de aprovação do solicitante.</span><span class="sxs-lookup"><span data-stu-id="f1568-105">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1568-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1568-106">Permissions</span></span>
<span data-ttu-id="f1568-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f1568-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1568-109">Permission type</span></span>      | <span data-ttu-id="f1568-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1568-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1568-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1568-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f1568-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1568-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f1568-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1568-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1568-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1568-114">Not supported.</span></span>    |
|<span data-ttu-id="f1568-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1568-115">Application</span></span> | <span data-ttu-id="f1568-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1568-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1568-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1568-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="f1568-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1568-118">Request headers</span></span>
| <span data-ttu-id="f1568-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f1568-119">Name</span></span>       | <span data-ttu-id="f1568-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1568-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f1568-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1568-121">Authorization</span></span>  | <span data-ttu-id="f1568-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1568-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1568-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1568-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f1568-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1568-125">Response</span></span>

<span data-ttu-id="f1568-126">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1568-126">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="f1568-127">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="f1568-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f1568-128">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="f1568-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="f1568-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1568-129">Example</span></span>
<span data-ttu-id="f1568-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f1568-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f1568-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1568-131">Request</span></span>
<span data-ttu-id="f1568-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1568-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1568-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1568-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```
# <a name="c"></a>[<span data-ttu-id="f1568-134">C#</span><span class="sxs-lookup"><span data-stu-id="f1568-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedapproval-myrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1568-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1568-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedapproval-myrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1568-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1568-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedapproval-myrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f1568-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1568-137">Response</span></span>
<span data-ttu-id="f1568-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1568-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

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
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
