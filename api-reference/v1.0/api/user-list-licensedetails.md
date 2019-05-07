---
title: Listar licenseDetails
description: Recupere uma lista de objetos licenseDetails.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b51b129977a2923646ec93479c0d8b888db2369e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601840"
---
# <a name="list-licensedetails"></a><span data-ttu-id="5477d-103">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="5477d-103">List licenseDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5477d-104">Recupere uma lista de objetos licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="5477d-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5477d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5477d-105">Permissions</span></span>
<span data-ttu-id="5477d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5477d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5477d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5477d-108">Permission type</span></span>      | <span data-ttu-id="5477d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5477d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5477d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5477d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5477d-111">User. Read, User. Read. All, User. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="5477d-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5477d-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5477d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5477d-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="5477d-113">User.Read</span></span>    |
|<span data-ttu-id="5477d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5477d-114">Application</span></span> | <span data-ttu-id="5477d-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5477d-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5477d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5477d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5477d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5477d-117">Optional query parameters</span></span>
<span data-ttu-id="5477d-118">Este método não \*\*\*\* oferece suporte a [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="5477d-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5477d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5477d-119">Request headers</span></span>
| <span data-ttu-id="5477d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5477d-120">Name</span></span>      |<span data-ttu-id="5477d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5477d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5477d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5477d-122">Authorization</span></span>  | <span data-ttu-id="5477d-123">&lt;Código do portador&gt;</span><span class="sxs-lookup"><span data-stu-id="5477d-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="5477d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5477d-124">Request body</span></span>
<span data-ttu-id="5477d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5477d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5477d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5477d-126">Response</span></span>

<span data-ttu-id="5477d-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [licenseDetails](../resources/licensedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5477d-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5477d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5477d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5477d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5477d-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="5477d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5477d-130">Response</span></span>
<span data-ttu-id="5477d-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5477d-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5477d-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5477d-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5477d-134">Basic</span><span class="sxs-lookup"><span data-stu-id="5477d-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_licensedetails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5477d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5477d-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_licensedetails-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-licensedetails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-licensedetails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
