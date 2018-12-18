---
title: 'workbookRange: rowsBelow'
description: Obtém um determinado número de linhas abaixo de um determinado intervalo.
author: lumine2008
ms.openlocfilehash: c6b7641dbc784c3c3fe7522308729877b7eb2ff9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337531"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="0a01f-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="0a01f-103">workbookRange: rowsBelow</span></span>

> <span data-ttu-id="0a01f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0a01f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a01f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0a01f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a01f-106">Obtém um determinado número de linhas abaixo de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="0a01f-106">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a01f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a01f-107">Permissions</span></span>
<span data-ttu-id="0a01f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a01f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a01f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a01f-110">Permission type</span></span>      | <span data-ttu-id="0a01f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a01f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a01f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a01f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0a01f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a01f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a01f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a01f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a01f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0a01f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0a01f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a01f-116">Application</span></span> | <span data-ttu-id="0a01f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a01f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a01f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a01f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="0a01f-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0a01f-119">Function parameters</span></span>

| <span data-ttu-id="0a01f-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0a01f-120">Parameter</span></span>    | <span data-ttu-id="0a01f-121">Type</span><span class="sxs-lookup"><span data-stu-id="0a01f-121">Type</span></span>   |<span data-ttu-id="0a01f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a01f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a01f-123">Count</span><span class="sxs-lookup"><span data-stu-id="0a01f-123">count</span></span>|<span data-ttu-id="0a01f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="0a01f-124">Int32</span></span>|<span data-ttu-id="0a01f-p103">Opcional. O número de linhas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="0a01f-p103">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="0a01f-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a01f-130">Request headers</span></span>
| <span data-ttu-id="0a01f-131">Nome</span><span class="sxs-lookup"><span data-stu-id="0a01f-131">Name</span></span>       | <span data-ttu-id="0a01f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a01f-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0a01f-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a01f-133">Authorization</span></span>  | <span data-ttu-id="0a01f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a01f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a01f-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0a01f-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="0a01f-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0a01f-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a01f-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a01f-139">Request body</span></span>
<span data-ttu-id="0a01f-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a01f-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a01f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a01f-141">Response</span></span>

<span data-ttu-id="0a01f-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a01f-142">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a01f-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a01f-143">Example</span></span>
<span data-ttu-id="0a01f-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0a01f-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0a01f-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a01f-145">Request</span></span>
<span data-ttu-id="0a01f-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a01f-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="0a01f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a01f-147">Response</span></span>
<span data-ttu-id="0a01f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a01f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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