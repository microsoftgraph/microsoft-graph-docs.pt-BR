---
title: 'workbookRange: rowsBelow'
description: Obtém um determinado número de linhas abaixo de um determinado intervalo.
ms.openlocfilehash: 530526a4a443d8a6d2985c9dea0724ed3f8c5b87
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034172"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="ddf44-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="ddf44-103">workbookRange: rowsBelow</span></span>

> <span data-ttu-id="ddf44-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ddf44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddf44-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ddf44-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ddf44-106">Obtém um determinado número de linhas abaixo de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="ddf44-106">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddf44-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddf44-107">Permissions</span></span>
<span data-ttu-id="ddf44-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddf44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddf44-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddf44-110">Permission type</span></span>      | <span data-ttu-id="ddf44-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddf44-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddf44-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddf44-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ddf44-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddf44-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ddf44-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddf44-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddf44-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddf44-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ddf44-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddf44-116">Application</span></span> | <span data-ttu-id="ddf44-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddf44-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddf44-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddf44-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="ddf44-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ddf44-119">Function parameters</span></span>

| <span data-ttu-id="ddf44-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ddf44-120">Parameter</span></span>    | <span data-ttu-id="ddf44-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddf44-121">Type</span></span>   |<span data-ttu-id="ddf44-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddf44-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddf44-123">Count</span><span class="sxs-lookup"><span data-stu-id="ddf44-123">count</span></span>|<span data-ttu-id="ddf44-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ddf44-124">Int32</span></span>|<span data-ttu-id="ddf44-p103">Opcional. O número de linhas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="ddf44-p103">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ddf44-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf44-130">Request headers</span></span>
| <span data-ttu-id="ddf44-131">Nome</span><span class="sxs-lookup"><span data-stu-id="ddf44-131">Name</span></span>       | <span data-ttu-id="ddf44-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddf44-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ddf44-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddf44-133">Authorization</span></span>  | <span data-ttu-id="ddf44-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddf44-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddf44-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ddf44-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="ddf44-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ddf44-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddf44-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf44-139">Request body</span></span>
<span data-ttu-id="ddf44-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddf44-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddf44-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf44-141">Response</span></span>

<span data-ttu-id="ddf44-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddf44-142">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddf44-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddf44-143">Example</span></span>
<span data-ttu-id="ddf44-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ddf44-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ddf44-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddf44-145">Request</span></span>
<span data-ttu-id="ddf44-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddf44-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="ddf44-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddf44-147">Response</span></span>
<span data-ttu-id="ddf44-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddf44-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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