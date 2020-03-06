---
title: 'workbookApplication: calcular'
description: Recalcula todas as pastas de trabalho abertas no Excel no momento.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0f6dfc1b77168b7b3c221b9c4ab147efb42a106b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508825"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="4881b-103">workbookApplication: calcular</span><span class="sxs-lookup"><span data-stu-id="4881b-103">workbookApplication: calculate</span></span>

<span data-ttu-id="4881b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4881b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4881b-105">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="4881b-105">Recalculate all currently opened workbooks in Excel.</span></span>

## <a name="permissions"></a><span data-ttu-id="4881b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4881b-106">Permissions</span></span>
<span data-ttu-id="4881b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4881b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4881b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4881b-109">Permission type</span></span>      | <span data-ttu-id="4881b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4881b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4881b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4881b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4881b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4881b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4881b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4881b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4881b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4881b-114">Not supported.</span></span>    |
|<span data-ttu-id="4881b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4881b-115">Application</span></span> | <span data-ttu-id="4881b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4881b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4881b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4881b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="4881b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4881b-118">Request headers</span></span>
| <span data-ttu-id="4881b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4881b-119">Name</span></span>       | <span data-ttu-id="4881b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4881b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4881b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4881b-121">Authorization</span></span>  | <span data-ttu-id="4881b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4881b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4881b-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="4881b-124">Content-type</span></span> | <span data-ttu-id="4881b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4881b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4881b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4881b-127">Request body</span></span>
<span data-ttu-id="4881b-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4881b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4881b-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4881b-129">Parameter</span></span>    | <span data-ttu-id="4881b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4881b-130">Type</span></span>   |<span data-ttu-id="4881b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4881b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4881b-132">Calculador de cálculo</span><span class="sxs-lookup"><span data-stu-id="4881b-132">calculationType</span></span>|<span data-ttu-id="4881b-133">string</span><span class="sxs-lookup"><span data-stu-id="4881b-133">string</span></span>|<span data-ttu-id="4881b-134">Especifica o tipo de cálculo a usar.</span><span class="sxs-lookup"><span data-stu-id="4881b-134">Specifies the calculation type to use.</span></span>  <span data-ttu-id="4881b-135">Os valores possíveis são: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="4881b-135">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="4881b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4881b-136">Response</span></span>

<span data-ttu-id="4881b-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4881b-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4881b-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4881b-139">Example</span></span>
<span data-ttu-id="4881b-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4881b-140">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="4881b-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4881b-141">Request</span></span>
<span data-ttu-id="4881b-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4881b-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4881b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4881b-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4881b-144">C#</span><span class="sxs-lookup"><span data-stu-id="4881b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4881b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4881b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4881b-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4881b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4881b-147">Java</span><span class="sxs-lookup"><span data-stu-id="4881b-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookapplication-calculate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4881b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4881b-148">Response</span></span>
<span data-ttu-id="4881b-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4881b-149">Here is an example of the response.</span></span> 
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
