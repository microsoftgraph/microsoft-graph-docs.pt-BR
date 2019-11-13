---
title: 'workbookApplication: calcular'
description: Recalcula todas as pastas de trabalho abertas no Excel no momento.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 288476706d1569a71827dc1441e1ec362ac6ca89
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302273"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="c1d41-103">workbookApplication: calcular</span><span class="sxs-lookup"><span data-stu-id="c1d41-103">workbookApplication: calculate</span></span>

<span data-ttu-id="c1d41-104">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="c1d41-104">Recalculate all currently opened workbooks in Excel.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1d41-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1d41-105">Permissions</span></span>
<span data-ttu-id="c1d41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1d41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1d41-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1d41-108">Permission type</span></span>      | <span data-ttu-id="c1d41-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1d41-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1d41-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1d41-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1d41-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1d41-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c1d41-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1d41-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1d41-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1d41-113">Not supported.</span></span>    |
|<span data-ttu-id="c1d41-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1d41-114">Application</span></span> | <span data-ttu-id="c1d41-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1d41-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1d41-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1d41-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="c1d41-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1d41-117">Request headers</span></span>
| <span data-ttu-id="c1d41-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c1d41-118">Name</span></span>       | <span data-ttu-id="c1d41-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1d41-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c1d41-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1d41-120">Authorization</span></span>  | <span data-ttu-id="c1d41-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1d41-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1d41-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="c1d41-123">Content-type</span></span> | <span data-ttu-id="c1d41-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1d41-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1d41-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1d41-126">Request body</span></span>
<span data-ttu-id="c1d41-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1d41-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1d41-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c1d41-128">Parameter</span></span>    | <span data-ttu-id="c1d41-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1d41-129">Type</span></span>   |<span data-ttu-id="c1d41-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1d41-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1d41-131">Calculador de cálculo</span><span class="sxs-lookup"><span data-stu-id="c1d41-131">calculationType</span></span>|<span data-ttu-id="c1d41-132">string</span><span class="sxs-lookup"><span data-stu-id="c1d41-132">string</span></span>|<span data-ttu-id="c1d41-133">Especifica o tipo de cálculo a usar.</span><span class="sxs-lookup"><span data-stu-id="c1d41-133">Specifies the calculation type to use.</span></span>  <span data-ttu-id="c1d41-134">Os valores possíveis são: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="c1d41-134">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="c1d41-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1d41-135">Response</span></span>

<span data-ttu-id="c1d41-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1d41-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1d41-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1d41-138">Example</span></span>
<span data-ttu-id="c1d41-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c1d41-139">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="c1d41-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1d41-140">Request</span></span>
<span data-ttu-id="c1d41-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1d41-141">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c1d41-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1d41-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1d41-143">C#</span><span class="sxs-lookup"><span data-stu-id="c1d41-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1d41-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1d41-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1d41-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1d41-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c1d41-146">Java</span><span class="sxs-lookup"><span data-stu-id="c1d41-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookapplication-calculate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c1d41-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1d41-147">Response</span></span>
<span data-ttu-id="c1d41-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1d41-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
