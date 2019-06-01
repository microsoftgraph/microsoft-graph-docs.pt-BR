---
title: Obter directoryRole
description: Recupere as propriedades de um objeto directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aba5f7fc9773e9f8e49e1346ecadbd690c62c0a2
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655954"
---
# <a name="get-directoryrole"></a><span data-ttu-id="caf5a-103">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="caf5a-103">Get directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caf5a-104">Recupere as propriedades de um objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="caf5a-104">Retrieve the properties of a directoryRole object.</span></span>
## <a name="permissions"></a><span data-ttu-id="caf5a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="caf5a-105">Permissions</span></span>
<span data-ttu-id="caf5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caf5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caf5a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caf5a-108">Permission type</span></span>      | <span data-ttu-id="caf5a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="caf5a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="caf5a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caf5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="caf5a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="caf5a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="caf5a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caf5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caf5a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caf5a-113">Not supported.</span></span>    |
|<span data-ttu-id="caf5a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caf5a-114">Application</span></span> | <span data-ttu-id="caf5a-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caf5a-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="caf5a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="caf5a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="caf5a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="caf5a-117">Optional query parameters</span></span>
<span data-ttu-id="caf5a-118">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="caf5a-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="caf5a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="caf5a-119">Request headers</span></span>
| <span data-ttu-id="caf5a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="caf5a-120">Name</span></span>       | <span data-ttu-id="caf5a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="caf5a-121">Type</span></span> | <span data-ttu-id="caf5a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="caf5a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="caf5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="caf5a-123">Authorization</span></span>  | <span data-ttu-id="caf5a-124">string</span><span class="sxs-lookup"><span data-stu-id="caf5a-124">string</span></span>  | <span data-ttu-id="caf5a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caf5a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="caf5a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="caf5a-127">Request body</span></span>
<span data-ttu-id="caf5a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="caf5a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="caf5a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="caf5a-129">Response</span></span>

<span data-ttu-id="caf5a-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caf5a-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="caf5a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="caf5a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="caf5a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="caf5a-132">Request</span></span>
<span data-ttu-id="caf5a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="caf5a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="caf5a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="caf5a-134">Response</span></span>
<span data-ttu-id="caf5a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="caf5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 142

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="caf5a-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="caf5a-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="caf5a-139">C#</span><span class="sxs-lookup"><span data-stu-id="caf5a-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="caf5a-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="caf5a-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryrole-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
