---
title: 'workbookRange: resizedRange'
description: Obtém um objeto range semelhante ao objeto range atual, mas com seu canto inferior direito expandido (ou recolhido) por um determinado número de linhas e colunas.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fc40c6053c64920226cb1d7b3d842ac13790d970
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578574"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="0079d-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="0079d-103">workbookRange: resizedRange</span></span>

<span data-ttu-id="0079d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0079d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0079d-105">Obtém um objeto range semelhante ao objeto range atual, mas com seu canto inferior direito expandido (ou recolhido) por um determinado número de linhas e colunas.</span><span class="sxs-lookup"><span data-stu-id="0079d-105">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="0079d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0079d-106">Permissions</span></span>
<span data-ttu-id="0079d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0079d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0079d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0079d-109">Permission type</span></span>      | <span data-ttu-id="0079d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0079d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0079d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0079d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0079d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0079d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0079d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0079d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0079d-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0079d-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0079d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0079d-115">Application</span></span> | <span data-ttu-id="0079d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0079d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0079d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0079d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="0079d-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0079d-118">Function parameters</span></span>

| <span data-ttu-id="0079d-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0079d-119">Parameter</span></span>    | <span data-ttu-id="0079d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0079d-120">Type</span></span>   |<span data-ttu-id="0079d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0079d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0079d-122">deltaRows</span><span class="sxs-lookup"><span data-stu-id="0079d-122">deltarows</span></span>|<span data-ttu-id="0079d-123">Int32</span><span class="sxs-lookup"><span data-stu-id="0079d-123">Int32</span></span>|<span data-ttu-id="0079d-p102">O número de linhas pelo qual expandir o canto inferior direito, referente ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo</span><span class="sxs-lookup"><span data-stu-id="0079d-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="0079d-126">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="0079d-126">deltaColumns</span></span>|<span data-ttu-id="0079d-127">Int32</span><span class="sxs-lookup"><span data-stu-id="0079d-127">Int32</span></span>|<span data-ttu-id="0079d-p103">O número de colunas pelo qual expandir o canto inferior direito, em relação ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo.</span><span class="sxs-lookup"><span data-stu-id="0079d-p103">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="0079d-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0079d-130">Request headers</span></span>
| <span data-ttu-id="0079d-131">Nome</span><span class="sxs-lookup"><span data-stu-id="0079d-131">Name</span></span>       | <span data-ttu-id="0079d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0079d-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0079d-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="0079d-133">Authorization</span></span>  | <span data-ttu-id="0079d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0079d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0079d-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0079d-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="0079d-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0079d-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0079d-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0079d-139">Request body</span></span>
<span data-ttu-id="0079d-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0079d-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0079d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0079d-141">Response</span></span>

<span data-ttu-id="0079d-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0079d-142">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0079d-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0079d-143">Example</span></span>
<span data-ttu-id="0079d-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0079d-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0079d-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0079d-145">Request</span></span>
<span data-ttu-id="0079d-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0079d-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="0079d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0079d-147">Response</span></span>
<span data-ttu-id="0079d-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0079d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


