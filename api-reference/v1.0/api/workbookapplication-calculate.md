---
title: 'workbookApplication: calculate'
description: Recalcula todas as pastas de trabalho abertas no Excel no momento.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 75a3888def2b292ffe4aed1aa178cd4c8709b4e3
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577685"
---
# <a name="workbookapplication-calculate"></a><span data-ttu-id="62747-103">workbookApplication: calculate</span><span class="sxs-lookup"><span data-stu-id="62747-103">workbookApplication: calculate</span></span>

<span data-ttu-id="62747-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62747-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62747-105">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="62747-105">Recalculate all currently opened workbooks in Excel.</span></span>

## <a name="permissions"></a><span data-ttu-id="62747-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="62747-106">Permissions</span></span>
<span data-ttu-id="62747-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62747-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62747-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62747-109">Permission type</span></span>      | <span data-ttu-id="62747-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62747-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62747-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62747-111">Delegated (work or school account)</span></span> | <span data-ttu-id="62747-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62747-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="62747-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62747-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62747-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62747-114">Not supported.</span></span>    |
|<span data-ttu-id="62747-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62747-115">Application</span></span> | <span data-ttu-id="62747-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62747-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62747-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62747-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/application/calculate
POST /me/drive/root:/{item-path}:/workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="62747-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62747-118">Request headers</span></span>
| <span data-ttu-id="62747-119">Nome</span><span class="sxs-lookup"><span data-stu-id="62747-119">Name</span></span>       | <span data-ttu-id="62747-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="62747-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="62747-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="62747-121">Authorization</span></span>  | <span data-ttu-id="62747-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62747-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="62747-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="62747-124">Content-type</span></span> | <span data-ttu-id="62747-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62747-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62747-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62747-127">Request body</span></span>
<span data-ttu-id="62747-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62747-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="62747-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="62747-129">Parameter</span></span>    | <span data-ttu-id="62747-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="62747-130">Type</span></span>   |<span data-ttu-id="62747-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="62747-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62747-132">calculationType</span><span class="sxs-lookup"><span data-stu-id="62747-132">calculationType</span></span>|<span data-ttu-id="62747-133">string</span><span class="sxs-lookup"><span data-stu-id="62747-133">string</span></span>|<span data-ttu-id="62747-134">Especifica o tipo de cálculo a usar.</span><span class="sxs-lookup"><span data-stu-id="62747-134">Specifies the calculation type to use.</span></span>  <span data-ttu-id="62747-135">Os valores possíveis são: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="62747-135">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="62747-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="62747-136">Response</span></span>

<span data-ttu-id="62747-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62747-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62747-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62747-139">Example</span></span>
<span data-ttu-id="62747-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="62747-140">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="62747-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62747-141">Request</span></span>
<span data-ttu-id="62747-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62747-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62747-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="62747-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="62747-144">C#</span><span class="sxs-lookup"><span data-stu-id="62747-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookapplication-calculate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62747-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62747-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookapplication-calculate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62747-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62747-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookapplication-calculate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62747-147">Java</span><span class="sxs-lookup"><span data-stu-id="62747-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookapplication-calculate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="62747-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="62747-148">Response</span></span>
<span data-ttu-id="62747-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62747-149">Here is an example of the response.</span></span> 
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

