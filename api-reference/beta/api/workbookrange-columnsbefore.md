---
title: 'workbookRange: columnsBefore'
description: Obtém um determinado número de colunas à esquerda do intervalo especificado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 677ee0d20031a9973644eec63e0a87e9c47440b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536086"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="e8957-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="e8957-103">workbookRange: columnsBefore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8957-104">Obtém um determinado número de colunas à esquerda do intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="e8957-104">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8957-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8957-105">Permissions</span></span>
<span data-ttu-id="e8957-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8957-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8957-108">Permission type</span></span>      | <span data-ttu-id="e8957-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8957-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8957-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8957-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8957-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8957-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e8957-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8957-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8957-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8957-113">Not supported.</span></span>    |
|<span data-ttu-id="e8957-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8957-114">Application</span></span> | <span data-ttu-id="e8957-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8957-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8957-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8957-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="e8957-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e8957-117">Function parameters</span></span>

| <span data-ttu-id="e8957-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e8957-118">Parameter</span></span>    | <span data-ttu-id="e8957-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8957-119">Type</span></span>   |<span data-ttu-id="e8957-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8957-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8957-121">Count</span><span class="sxs-lookup"><span data-stu-id="e8957-121">count</span></span>|<span data-ttu-id="e8957-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e8957-122">Int32</span></span>|<span data-ttu-id="e8957-123">O número de colunas a serem incluídas no intervalo resultante.</span><span class="sxs-lookup"><span data-stu-id="e8957-123">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="e8957-124">Em geral, use um número positivo para criar um intervalo fora do intervalo atual.</span><span class="sxs-lookup"><span data-stu-id="e8957-124">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="e8957-125">Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual.</span><span class="sxs-lookup"><span data-stu-id="e8957-125">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="e8957-126">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="e8957-126">The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e8957-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8957-127">Request headers</span></span>
| <span data-ttu-id="e8957-128">Nome</span><span class="sxs-lookup"><span data-stu-id="e8957-128">Name</span></span>       | <span data-ttu-id="e8957-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8957-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e8957-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8957-130">Authorization</span></span>  | <span data-ttu-id="e8957-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8957-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8957-133">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e8957-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="e8957-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e8957-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8957-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8957-136">Request body</span></span>
<span data-ttu-id="e8957-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8957-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8957-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8957-138">Response</span></span>
<span data-ttu-id="e8957-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8957-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8957-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8957-140">Example</span></span>
<span data-ttu-id="e8957-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e8957-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e8957-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8957-142">Request</span></span>
<span data-ttu-id="e8957-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8957-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="e8957-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8957-144">Response</span></span>
<span data-ttu-id="e8957-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8957-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/workbookrange-columnsbefore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
