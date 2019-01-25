---
title: 'workbookRange: rowsBelow'
description: Obtém um determinado número de linhas abaixo de um determinado intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 42d53ce3aa9d26c7c499b19af3d5330259786520
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529471"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="9165c-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="9165c-103">workbookRange: rowsBelow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9165c-104">Obtém um determinado número de linhas abaixo de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="9165c-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="9165c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9165c-105">Permissions</span></span>
<span data-ttu-id="9165c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9165c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9165c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9165c-108">Permission type</span></span>      | <span data-ttu-id="9165c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9165c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9165c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9165c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9165c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9165c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9165c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9165c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9165c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9165c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9165c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9165c-114">Application</span></span> | <span data-ttu-id="9165c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9165c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9165c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9165c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="9165c-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9165c-117">Function parameters</span></span>

| <span data-ttu-id="9165c-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9165c-118">Parameter</span></span>    | <span data-ttu-id="9165c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9165c-119">Type</span></span>   |<span data-ttu-id="9165c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9165c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9165c-121">Count</span><span class="sxs-lookup"><span data-stu-id="9165c-121">count</span></span>|<span data-ttu-id="9165c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9165c-122">Int32</span></span>|<span data-ttu-id="9165c-p102">Opcional. O número de linhas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="9165c-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9165c-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9165c-128">Request headers</span></span>
| <span data-ttu-id="9165c-129">Nome</span><span class="sxs-lookup"><span data-stu-id="9165c-129">Name</span></span>       | <span data-ttu-id="9165c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9165c-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9165c-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="9165c-131">Authorization</span></span>  | <span data-ttu-id="9165c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9165c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9165c-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9165c-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="9165c-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9165c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9165c-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9165c-137">Request body</span></span>
<span data-ttu-id="9165c-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9165c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9165c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9165c-139">Response</span></span>

<span data-ttu-id="9165c-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9165c-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9165c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9165c-141">Example</span></span>
<span data-ttu-id="9165c-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9165c-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9165c-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9165c-143">Request</span></span>
<span data-ttu-id="9165c-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9165c-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="9165c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="9165c-145">Response</span></span>
<span data-ttu-id="9165c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9165c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrange-rowsbelow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
