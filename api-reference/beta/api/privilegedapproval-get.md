---
title: Get privilegedApproval
description: Recupere as propriedades e os relacionamentos do objeto privilegedapproval.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d996c70936dab216b036ba9f218383d4284420c3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361283"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="d082c-103">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="d082c-103">Get privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d082c-104">Recupere as propriedades e os relacionamentos do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="d082c-104">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d082c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d082c-105">Permissions</span></span>
<span data-ttu-id="d082c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d082c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d082c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d082c-108">Permission type</span></span>      | <span data-ttu-id="d082c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d082c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d082c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d082c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d082c-111">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="d082c-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="d082c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d082c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d082c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d082c-113">Not supported.</span></span>    |
|<span data-ttu-id="d082c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d082c-114">Application</span></span> | <span data-ttu-id="d082c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d082c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d082c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d082c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d082c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d082c-117">Optional query parameters</span></span>
<span data-ttu-id="d082c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d082c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d082c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d082c-119">Request headers</span></span>
| <span data-ttu-id="d082c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d082c-120">Name</span></span>      |<span data-ttu-id="d082c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d082c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d082c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d082c-122">Authorization</span></span>  | <span data-ttu-id="d082c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d082c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d082c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d082c-125">Request body</span></span>
<span data-ttu-id="d082c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d082c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d082c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d082c-127">Response</span></span>

<span data-ttu-id="d082c-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d082c-128">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="d082c-129">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="d082c-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d082c-130">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="d082c-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="d082c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d082c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d082c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d082c-132">Request</span></span>
<span data-ttu-id="d082c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d082c-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d082c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d082c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d082c-135">C#</span><span class="sxs-lookup"><span data-stu-id="d082c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d082c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d082c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d082c-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d082c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d082c-138">Java</span><span class="sxs-lookup"><span data-stu-id="d082c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d082c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d082c-139">Response</span></span>
<span data-ttu-id="d082c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d082c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
