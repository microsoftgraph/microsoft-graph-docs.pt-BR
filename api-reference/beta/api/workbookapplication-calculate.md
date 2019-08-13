---
title: 'workbookApplication: calcular'
description: Recalcula todas as pastas de trabalho abertas no Excel no momento.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a89bd864f0c145acf37a0caef64a42ebddd51eff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361958"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="0c558-103">workbookApplication: calcular</span><span class="sxs-lookup"><span data-stu-id="0c558-103">workbookApplication: calculate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c558-104">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="0c558-104">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c558-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c558-105">Permissions</span></span>
<span data-ttu-id="0c558-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c558-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c558-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c558-108">Permission type</span></span>      | <span data-ttu-id="0c558-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c558-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c558-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c558-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0c558-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c558-111">Not supported.</span></span>    |
|<span data-ttu-id="0c558-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c558-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c558-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c558-113">Not supported.</span></span>    |
|<span data-ttu-id="0c558-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c558-114">Application</span></span> | <span data-ttu-id="0c558-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c558-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c558-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c558-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="0c558-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c558-117">Request headers</span></span>
| <span data-ttu-id="0c558-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0c558-118">Name</span></span>       | <span data-ttu-id="0c558-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c558-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c558-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c558-120">Authorization</span></span>  | <span data-ttu-id="0c558-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c558-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c558-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c558-123">Request body</span></span>
<span data-ttu-id="0c558-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c558-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c558-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0c558-125">Parameter</span></span>    | <span data-ttu-id="0c558-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c558-126">Type</span></span>   |<span data-ttu-id="0c558-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c558-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c558-128">Calculador de cálculo</span><span class="sxs-lookup"><span data-stu-id="0c558-128">calculationType</span></span>|<span data-ttu-id="0c558-129">string</span><span class="sxs-lookup"><span data-stu-id="0c558-129">string</span></span>|<span data-ttu-id="0c558-130">Especifica o tipo de cálculo a usar.</span><span class="sxs-lookup"><span data-stu-id="0c558-130">Specifies the calculation type to use.</span></span>  <span data-ttu-id="0c558-131">Os valores possíveis são: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="0c558-131">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="0c558-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c558-132">Response</span></span>

<span data-ttu-id="0c558-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c558-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c558-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c558-135">Example</span></span>
<span data-ttu-id="0c558-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0c558-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c558-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c558-137">Request</span></span>
<span data-ttu-id="0c558-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c558-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c558-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c558-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c558-140">C#</span><span class="sxs-lookup"><span data-stu-id="0c558-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c558-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c558-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c558-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0c558-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c558-143">Java</span><span class="sxs-lookup"><span data-stu-id="0c558-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookapplication-calculate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0c558-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c558-144">Response</span></span>
<span data-ttu-id="0c558-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c558-145">Here is an example of the response.</span></span> 
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
