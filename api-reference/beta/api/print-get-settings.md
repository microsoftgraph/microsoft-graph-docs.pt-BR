---
title: Obter configurações
description: Recupere configurações de todo o locatário para o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c8abf25bf95262813c354b8a54f50656af6c3a99
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948345"
---
# <a name="get-settings"></a><span data-ttu-id="94629-103">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="94629-103">Get settings</span></span>

<span data-ttu-id="94629-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94629-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94629-105">Recupere configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="94629-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="94629-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94629-106">Permissions</span></span>
<span data-ttu-id="94629-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94629-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94629-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94629-109">Permission type</span></span> | <span data-ttu-id="94629-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94629-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="94629-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94629-111">Delegated (work or school account)</span></span>| <span data-ttu-id="94629-112">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="94629-112">Users.Read.All</span></span> |
|<span data-ttu-id="94629-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94629-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94629-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94629-114">Not Supported.</span></span>|
|<span data-ttu-id="94629-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94629-115">Application</span></span>|<span data-ttu-id="94629-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94629-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94629-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94629-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94629-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94629-118">Optional query parameters</span></span>
<span data-ttu-id="94629-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94629-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="94629-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="94629-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="94629-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94629-121">Request headers</span></span>
| <span data-ttu-id="94629-122">Nome</span><span class="sxs-lookup"><span data-stu-id="94629-122">Name</span></span>      |<span data-ttu-id="94629-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="94629-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94629-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="94629-124">Authorization</span></span> | <span data-ttu-id="94629-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94629-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94629-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94629-127">Request body</span></span>
<span data-ttu-id="94629-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94629-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="94629-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="94629-129">Response</span></span>
<span data-ttu-id="94629-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printSettings](../resources/printsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94629-130">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94629-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94629-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94629-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94629-132">Request</span></span>
<span data-ttu-id="94629-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94629-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94629-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="94629-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/settings
```
# <a name="c"></a>[<span data-ttu-id="94629-135">C#</span><span class="sxs-lookup"><span data-stu-id="94629-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94629-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94629-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94629-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94629-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94629-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="94629-138">Response</span></span>
<span data-ttu-id="94629-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94629-139">The following is an example of the response.</span></span>
><span data-ttu-id="94629-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94629-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 144

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/settings",
  "documentConversionEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
