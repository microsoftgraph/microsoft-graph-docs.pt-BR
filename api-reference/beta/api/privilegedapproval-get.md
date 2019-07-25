---
title: Get privilegedApproval
description: Recupere as propriedades e os relacionamentos do objeto privilegedapproval.
localization_priority: Normal
ms.openlocfilehash: a0704a970a93f40f316946aa193359b03f828573
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875955"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="abaa2-103">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="abaa2-103">Get privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abaa2-104">Recupere as propriedades e os relacionamentos do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="abaa2-104">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="abaa2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="abaa2-105">Permissions</span></span>
<span data-ttu-id="abaa2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abaa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="abaa2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abaa2-108">Permission type</span></span>      | <span data-ttu-id="abaa2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="abaa2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abaa2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abaa2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="abaa2-111">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="abaa2-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="abaa2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abaa2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abaa2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abaa2-113">Not supported.</span></span>    |
|<span data-ttu-id="abaa2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abaa2-114">Application</span></span> | <span data-ttu-id="abaa2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abaa2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="abaa2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abaa2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="abaa2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="abaa2-117">Optional query parameters</span></span>
<span data-ttu-id="abaa2-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="abaa2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abaa2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abaa2-119">Request headers</span></span>
| <span data-ttu-id="abaa2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="abaa2-120">Name</span></span>      |<span data-ttu-id="abaa2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="abaa2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="abaa2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="abaa2-122">Authorization</span></span>  | <span data-ttu-id="abaa2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abaa2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="abaa2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abaa2-125">Request body</span></span>
<span data-ttu-id="abaa2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="abaa2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abaa2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="abaa2-127">Response</span></span>

<span data-ttu-id="abaa2-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abaa2-128">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="abaa2-129">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="abaa2-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="abaa2-130">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="abaa2-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="abaa2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abaa2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="abaa2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abaa2-132">Request</span></span>
<span data-ttu-id="abaa2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abaa2-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="abaa2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="abaa2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="abaa2-135">C#</span><span class="sxs-lookup"><span data-stu-id="abaa2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="abaa2-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="abaa2-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="abaa2-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="abaa2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="abaa2-138">Java</span><span class="sxs-lookup"><span data-stu-id="abaa2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="abaa2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="abaa2-139">Response</span></span>
<span data-ttu-id="abaa2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abaa2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
