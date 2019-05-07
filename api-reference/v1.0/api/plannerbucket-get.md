---
title: Obter plannerBucket
description: Recupere as propriedades e os relacionamentos do objeto **plannerBucket** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d30483be99ddcdac67334a6f62692b7322f8556d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33609395"
---
# <a name="get-plannerbucket"></a><span data-ttu-id="38b9e-103">Obter plannerBucket</span><span class="sxs-lookup"><span data-stu-id="38b9e-103">Get plannerBucket</span></span>

<span data-ttu-id="38b9e-104">Recupere as propriedades e os relacionamentos do objeto **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="38b9e-104">Retrieve the properties and relationships of **plannerBucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="38b9e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="38b9e-105">Permissions</span></span>
<span data-ttu-id="38b9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38b9e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38b9e-108">Permission type</span></span>      | <span data-ttu-id="38b9e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38b9e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38b9e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38b9e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38b9e-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38b9e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="38b9e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38b9e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38b9e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38b9e-113">Not supported.</span></span>    |
|<span data-ttu-id="38b9e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38b9e-114">Application</span></span> | <span data-ttu-id="38b9e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38b9e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38b9e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38b9e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="38b9e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38b9e-117">Request headers</span></span>
| <span data-ttu-id="38b9e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="38b9e-118">Name</span></span>      |<span data-ttu-id="38b9e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="38b9e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38b9e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="38b9e-120">Authorization</span></span>  | <span data-ttu-id="38b9e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38b9e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38b9e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38b9e-123">Request body</span></span>
<span data-ttu-id="38b9e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38b9e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38b9e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="38b9e-125">Response</span></span>

<span data-ttu-id="38b9e-126">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38b9e-126">If successful, this method returns a `200 OK` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="38b9e-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="38b9e-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="38b9e-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="38b9e-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="38b9e-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="38b9e-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="38b9e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38b9e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38b9e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38b9e-131">Request</span></span>
<span data-ttu-id="38b9e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38b9e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbucket"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets/{bucket-id}
```
##### <a name="response"></a><span data-ttu-id="38b9e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="38b9e-133">Response</span></span>
<span data-ttu-id="38b9e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38b9e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="38b9e-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="38b9e-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38b9e-138">Basic</span><span class="sxs-lookup"><span data-stu-id="38b9e-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_plannerbucket-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38b9e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38b9e-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_plannerbucket-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerbucket-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerbucket-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
