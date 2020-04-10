---
title: Get privilegedApproval
description: Recupere as propriedades e os relacionamentos do objeto privilegedapproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: dbf8611e94e07b4f0a5bea1024a59779f72c53dc
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218812"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="e3794-103">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="e3794-103">Get privilegedApproval</span></span>

<span data-ttu-id="e3794-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3794-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3794-105">Recupere as propriedades e os relacionamentos do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="e3794-105">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3794-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3794-106">Permissions</span></span>
<span data-ttu-id="e3794-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3794-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e3794-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3794-109">Permission type</span></span>      | <span data-ttu-id="e3794-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3794-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3794-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3794-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e3794-112">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="e3794-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="e3794-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3794-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3794-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3794-114">Not supported.</span></span>    |
|<span data-ttu-id="e3794-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3794-115">Application</span></span> | <span data-ttu-id="e3794-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3794-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3794-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3794-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3794-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3794-118">Optional query parameters</span></span>
<span data-ttu-id="e3794-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3794-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3794-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3794-120">Request headers</span></span>
| <span data-ttu-id="e3794-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e3794-121">Name</span></span>      |<span data-ttu-id="e3794-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3794-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3794-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3794-123">Authorization</span></span>  | <span data-ttu-id="e3794-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3794-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3794-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3794-126">Request body</span></span>
<span data-ttu-id="e3794-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3794-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3794-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3794-128">Response</span></span>

<span data-ttu-id="e3794-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3794-129">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="e3794-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="e3794-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e3794-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="e3794-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="e3794-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3794-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3794-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3794-133">Request</span></span>
<span data-ttu-id="e3794-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3794-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3794-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3794-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/{id}
```
# <a name="c"></a>[<span data-ttu-id="e3794-136">C#</span><span class="sxs-lookup"><span data-stu-id="e3794-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3794-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3794-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3794-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3794-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e3794-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3794-139">Response</span></span>
<span data-ttu-id="e3794-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3794-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
