---
title: Get privilegedRoleSummary
description: Recupere as propriedades e os relacionamentos do objeto privilegedRoleSummary.
localization_priority: Normal
ms.openlocfilehash: 2261d4340d5c9feb29d81da195148047aa68ab88
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593705"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="d600c-103">Get privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="d600c-103">Get privilegedRoleSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d600c-104">Recupere as propriedades e os relacionamentos do objeto [privilegedRoleSummary](../resources/privilegedrolesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d600c-104">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d600c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d600c-105">Permissions</span></span>
<span data-ttu-id="d600c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d600c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d600c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d600c-108">Permission type</span></span>      | <span data-ttu-id="d600c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d600c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d600c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d600c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d600c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d600c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d600c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d600c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d600c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d600c-113">Not supported.</span></span>    |
|<span data-ttu-id="d600c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d600c-114">Application</span></span> | <span data-ttu-id="d600c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d600c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d600c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d600c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d600c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d600c-117">Optional query parameters</span></span>
<span data-ttu-id="d600c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d600c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d600c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d600c-119">Request headers</span></span>
| <span data-ttu-id="d600c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d600c-120">Name</span></span>      |<span data-ttu-id="d600c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d600c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d600c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d600c-122">Authorization</span></span>  | <span data-ttu-id="d600c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d600c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d600c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d600c-125">Request body</span></span>
<span data-ttu-id="d600c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d600c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d600c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d600c-127">Response</span></span>

<span data-ttu-id="d600c-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRoleSummary](../resources/privilegedrolesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d600c-128">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="d600c-129">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="d600c-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d600c-130">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="d600c-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="d600c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d600c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d600c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d600c-132">Request</span></span>
<span data-ttu-id="d600c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d600c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="d600c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d600c-134">Response</span></span>
<span data-ttu-id="d600c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d600c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d600c-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d600c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d600c-139">Basic</span><span class="sxs-lookup"><span data-stu-id="d600c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedrolesummary-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d600c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d600c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedrolesummary-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedrolesummary-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrolesummary-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
