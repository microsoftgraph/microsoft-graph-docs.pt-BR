---
title: 'workbookRange: resizedRange'
description: Obtém um objeto range semelhante ao objeto range atual, mas com seu canto inferior direito expandido (ou recolhido) por um determinado número de linhas e colunas.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 31a7cf1b88f54309bb43c1a021673bd29f290dae
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573583"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="2a855-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="2a855-103">workbookRange: resizedRange</span></span>

<span data-ttu-id="2a855-104">Namespace: microsoft.graph Obtém um objeto de intervalo semelhante ao objeto de intervalo atual, mas com seu canto inferior direito expandido (ou contratado) por algum número de linhas e colunas.</span><span class="sxs-lookup"><span data-stu-id="2a855-104">Namespace: microsoft.graph Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a855-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a855-105">Permissions</span></span>
<span data-ttu-id="2a855-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a855-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a855-108">Permission type</span></span>      | <span data-ttu-id="2a855-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a855-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a855-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a855-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2a855-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a855-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2a855-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a855-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a855-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a855-113">Not supported.</span></span>    |
|<span data-ttu-id="2a855-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a855-114">Application</span></span> | <span data-ttu-id="2a855-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a855-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a855-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a855-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="2a855-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2a855-117">Function parameters</span></span>

| <span data-ttu-id="2a855-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2a855-118">Parameter</span></span>    | <span data-ttu-id="2a855-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a855-119">Type</span></span>   |<span data-ttu-id="2a855-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a855-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a855-121">deltaRows</span><span class="sxs-lookup"><span data-stu-id="2a855-121">deltaRows</span></span>|<span data-ttu-id="2a855-122">Int32</span><span class="sxs-lookup"><span data-stu-id="2a855-122">Int32</span></span>|<span data-ttu-id="2a855-p102">O número de linhas pelo qual expandir o canto inferior direito, referente ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo</span><span class="sxs-lookup"><span data-stu-id="2a855-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="2a855-125">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="2a855-125">deltaColumns</span></span>|<span data-ttu-id="2a855-126">Int32</span><span class="sxs-lookup"><span data-stu-id="2a855-126">Int32</span></span>|<span data-ttu-id="2a855-127">O número de colunas pelas quais expandir o canto inferior direito, em relação ao intervalo atual.</span><span class="sxs-lookup"><span data-stu-id="2a855-127">The number of columns by which to expand the bottom-right corner, relative to the current range.</span></span> <span data-ttu-id="2a855-128">Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo.</span><span class="sxs-lookup"><span data-stu-id="2a855-128">Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2a855-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a855-129">Request headers</span></span>
| <span data-ttu-id="2a855-130">Nome</span><span class="sxs-lookup"><span data-stu-id="2a855-130">Name</span></span>       | <span data-ttu-id="2a855-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a855-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2a855-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a855-132">Authorization</span></span>  | <span data-ttu-id="2a855-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a855-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a855-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2a855-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="2a855-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2a855-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a855-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a855-138">Request body</span></span>
<span data-ttu-id="2a855-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a855-139">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="2a855-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a855-140">Response</span></span>
<span data-ttu-id="2a855-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a855-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a855-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a855-142">Example</span></span>
<span data-ttu-id="2a855-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2a855-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2a855-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a855-144">Request</span></span>
<span data-ttu-id="2a855-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a855-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="2a855-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a855-146">Response</span></span>
<span data-ttu-id="2a855-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a855-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

