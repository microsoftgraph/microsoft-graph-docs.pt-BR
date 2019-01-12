---
title: 'workbookRange: columnsAfter'
description: Obtém um determinado número de colunas à direita do intervalo especificado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7b5a7625f6caa7bddbb21e23e670508e989f974a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982334"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="3be11-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="3be11-103">workbookRange: columnsAfter</span></span>

> <span data-ttu-id="3be11-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3be11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3be11-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3be11-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3be11-106">Obtém um determinado número de colunas à direita do intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="3be11-106">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="3be11-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3be11-107">Permissions</span></span>
<span data-ttu-id="3be11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3be11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3be11-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3be11-110">Permission type</span></span>      | <span data-ttu-id="3be11-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3be11-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3be11-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3be11-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3be11-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3be11-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3be11-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3be11-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3be11-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3be11-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3be11-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3be11-116">Application</span></span> | <span data-ttu-id="3be11-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3be11-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3be11-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3be11-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="3be11-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3be11-119">Function parameters</span></span>

| <span data-ttu-id="3be11-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3be11-120">Parameter</span></span>    | <span data-ttu-id="3be11-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3be11-121">Type</span></span>   |<span data-ttu-id="3be11-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be11-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3be11-123">Count</span><span class="sxs-lookup"><span data-stu-id="3be11-123">count</span></span>|<span data-ttu-id="3be11-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3be11-124">Int32</span></span>|<span data-ttu-id="3be11-p103">O número de colunas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1</span><span class="sxs-lookup"><span data-stu-id="3be11-p103">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3be11-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3be11-129">Request headers</span></span>
| <span data-ttu-id="3be11-130">Nome</span><span class="sxs-lookup"><span data-stu-id="3be11-130">Name</span></span>       | <span data-ttu-id="3be11-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be11-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3be11-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="3be11-132">Authorization</span></span>  | <span data-ttu-id="3be11-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3be11-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3be11-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3be11-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="3be11-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3be11-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3be11-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3be11-138">Request body</span></span>
<span data-ttu-id="3be11-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3be11-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3be11-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be11-140">Response</span></span>

<span data-ttu-id="3be11-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3be11-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3be11-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3be11-142">Example</span></span>
<span data-ttu-id="3be11-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3be11-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3be11-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3be11-144">Request</span></span>
<span data-ttu-id="3be11-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3be11-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="3be11-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be11-146">Response</span></span>
<span data-ttu-id="3be11-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3be11-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
