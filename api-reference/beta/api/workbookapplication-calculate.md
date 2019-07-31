---
title: 'workbookApplication: calcular'
description: Recalcula todas as pastas de trabalho abertas no Excel no momento.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5a80666d13a1783d1f7deabd6b74f89fcae7e928
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987380"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="f536c-103">workbookApplication: calcular</span><span class="sxs-lookup"><span data-stu-id="f536c-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f536c-104">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="f536c-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="f536c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f536c-105">Permissions</span></span>
<span data-ttu-id="f536c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f536c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f536c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f536c-108">Permission type</span></span>      | <span data-ttu-id="f536c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f536c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f536c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f536c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f536c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f536c-111">Not supported.</span></span>    |
|<span data-ttu-id="f536c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f536c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f536c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f536c-113">Not supported.</span></span>    |
|<span data-ttu-id="f536c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f536c-114">Application</span></span> | <span data-ttu-id="f536c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f536c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f536c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f536c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="f536c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f536c-117">Request headers</span></span>
| <span data-ttu-id="f536c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f536c-118">Name</span></span>       | <span data-ttu-id="f536c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f536c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f536c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f536c-120">Authorization</span></span>  | <span data-ttu-id="f536c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f536c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f536c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f536c-123">Request body</span></span>
<span data-ttu-id="f536c-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f536c-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f536c-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f536c-125">Parameter</span></span>    | <span data-ttu-id="f536c-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="f536c-126">Type</span></span>   |<span data-ttu-id="f536c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f536c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f536c-128">Calculador de cálculo</span><span class="sxs-lookup"><span data-stu-id="f536c-128">calculationType</span></span>|<span data-ttu-id="f536c-129">string</span><span class="sxs-lookup"><span data-stu-id="f536c-129">string</span></span>|<span data-ttu-id="f536c-130">Especifica o tipo de cálculo a usar.</span><span class="sxs-lookup"><span data-stu-id="f536c-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="f536c-131">Os valores possíveis são: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="f536c-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="f536c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f536c-132">Response</span></span>

<span data-ttu-id="f536c-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f536c-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f536c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f536c-135">Example</span></span>
<span data-ttu-id="f536c-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f536c-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f536c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f536c-137">Request</span></span>
<span data-ttu-id="f536c-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f536c-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f536c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f536c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookApplication_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f536c-140">C#</span><span class="sxs-lookup"><span data-stu-id="f536c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f536c-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="f536c-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f536c-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f536c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f536c-143">Java</span><span class="sxs-lookup"><span data-stu-id="f536c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookapplication-calculate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f536c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f536c-144">Response</span></span>
<span data-ttu-id="f536c-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f536c-145">Here is an example of the response.</span></span> 
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
