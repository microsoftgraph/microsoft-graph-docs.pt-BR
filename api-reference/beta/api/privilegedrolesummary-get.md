---
title: Get privilegedRoleSummary
description: Recupere as propriedades e os relacionamentos do objeto privilegedRoleSummary.
localization_priority: Normal
ms.openlocfilehash: 3030a82c4cc8959eb515d02b2ecb665440f991ff
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455382"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="02d92-103">Get privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="02d92-103">Get privilegedRoleSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02d92-104">Recupere as propriedades e os relacionamentos do objeto [privilegedRoleSummary](../resources/privilegedrolesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="02d92-104">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="02d92-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="02d92-105">Permissions</span></span>
<span data-ttu-id="02d92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02d92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="02d92-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02d92-108">Permission type</span></span>      | <span data-ttu-id="02d92-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02d92-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02d92-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02d92-110">Delegated (work or school account)</span></span> | <span data-ttu-id="02d92-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02d92-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02d92-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02d92-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02d92-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02d92-113">Not supported.</span></span>    |
|<span data-ttu-id="02d92-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02d92-114">Application</span></span> | <span data-ttu-id="02d92-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02d92-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02d92-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02d92-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="02d92-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02d92-117">Optional query parameters</span></span>
<span data-ttu-id="02d92-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02d92-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02d92-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02d92-119">Request headers</span></span>
| <span data-ttu-id="02d92-120">Nome</span><span class="sxs-lookup"><span data-stu-id="02d92-120">Name</span></span>      |<span data-ttu-id="02d92-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d92-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02d92-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02d92-122">Authorization</span></span>  | <span data-ttu-id="02d92-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02d92-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02d92-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02d92-125">Request body</span></span>
<span data-ttu-id="02d92-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02d92-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02d92-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="02d92-127">Response</span></span>

<span data-ttu-id="02d92-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRoleSummary](../resources/privilegedrolesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02d92-128">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="02d92-129">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="02d92-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="02d92-130">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="02d92-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="02d92-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02d92-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02d92-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02d92-132">Request</span></span>
<span data-ttu-id="02d92-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02d92-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="02d92-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="02d92-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="02d92-135">C#</span><span class="sxs-lookup"><span data-stu-id="02d92-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02d92-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="02d92-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02d92-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="02d92-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="02d92-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="02d92-138">Response</span></span>
<span data-ttu-id="02d92-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02d92-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
