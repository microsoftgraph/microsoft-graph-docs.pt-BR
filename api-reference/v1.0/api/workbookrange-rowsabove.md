---
title: 'workbookRange: rowsAbove'
description: Obtém um determinado número de linhas acima de um determinado intervalo.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 0eb7a9ec6539854d4148148e2d283df0eaa366d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875009"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="88687-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="88687-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="88687-104">Obtém um determinado número de linhas acima de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="88687-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="88687-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="88687-105">Permissions</span></span>
<span data-ttu-id="88687-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88687-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88687-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88687-108">Permission type</span></span>      | <span data-ttu-id="88687-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88687-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88687-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88687-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88687-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88687-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="88687-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88687-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88687-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88687-113">Not supported.</span></span>    |
|<span data-ttu-id="88687-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88687-114">Application</span></span> | <span data-ttu-id="88687-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88687-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88687-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88687-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="88687-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="88687-117">Function parameters</span></span>

| <span data-ttu-id="88687-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="88687-118">Parameter</span></span>    | <span data-ttu-id="88687-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="88687-119">Type</span></span>   |<span data-ttu-id="88687-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="88687-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88687-121">Count</span><span class="sxs-lookup"><span data-stu-id="88687-121">count</span></span>|<span data-ttu-id="88687-122">Int32</span><span class="sxs-lookup"><span data-stu-id="88687-122">Int32</span></span>|<span data-ttu-id="88687-p102">Opcional. O número de linhas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="88687-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="88687-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88687-128">Request headers</span></span>
| <span data-ttu-id="88687-129">Nome</span><span class="sxs-lookup"><span data-stu-id="88687-129">Name</span></span>       | <span data-ttu-id="88687-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="88687-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="88687-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="88687-131">Authorization</span></span>  | <span data-ttu-id="88687-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88687-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88687-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="88687-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="88687-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="88687-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88687-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88687-137">Request body</span></span>
<span data-ttu-id="88687-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88687-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88687-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="88687-139">Response</span></span>
<span data-ttu-id="88687-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88687-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88687-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88687-141">Example</span></span>
<span data-ttu-id="88687-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="88687-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="88687-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88687-143">Request</span></span>
<span data-ttu-id="88687-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88687-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="88687-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="88687-145">Response</span></span>
<span data-ttu-id="88687-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88687-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="88687-149">Se for chamado sem o opcional `count` parâmetro, essa função retornará a única linha acima do intervalo.</span><span class="sxs-lookup"><span data-stu-id="88687-149">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="88687-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88687-150">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="88687-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="88687-151">Response</span></span>
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
