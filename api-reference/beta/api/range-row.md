---
title: 'Range: Row'
description: Obtém uma linha contida no intervalo.
ms.openlocfilehash: d27d604444760d31f4abed9f1c3b9ae958a34aee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038708"
---
# <a name="range-row"></a><span data-ttu-id="f4f95-103">Range: Row</span><span class="sxs-lookup"><span data-stu-id="f4f95-103">Range: Row</span></span>

> <span data-ttu-id="f4f95-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f4f95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4f95-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f4f95-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f4f95-106">Obtém uma linha contida no intervalo.</span><span class="sxs-lookup"><span data-stu-id="f4f95-106">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="f4f95-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4f95-107">Permissions</span></span>
<span data-ttu-id="f4f95-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4f95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4f95-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4f95-110">Permission type</span></span>      | <span data-ttu-id="f4f95-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4f95-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4f95-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4f95-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f4f95-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4f95-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f4f95-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4f95-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4f95-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4f95-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f4f95-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4f95-116">Application</span></span> | <span data-ttu-id="f4f95-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4f95-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4f95-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4f95-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/Row
POST /workbook/worksheets/{id|name}/range(address='<address>')/Row
POST /workbook/tables/{id|name}/columns/{id|name}/range/Row

```
## <a name="request-headers"></a><span data-ttu-id="f4f95-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4f95-119">Request headers</span></span>
| <span data-ttu-id="f4f95-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f4f95-120">Name</span></span>       | <span data-ttu-id="f4f95-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4f95-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f4f95-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4f95-122">Authorization</span></span>  | <span data-ttu-id="f4f95-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4f95-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4f95-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f4f95-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f4f95-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f4f95-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4f95-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4f95-128">Request body</span></span>
<span data-ttu-id="f4f95-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4f95-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4f95-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f4f95-130">Parameter</span></span>    | <span data-ttu-id="f4f95-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4f95-131">Type</span></span>   |<span data-ttu-id="f4f95-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4f95-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4f95-133">row</span><span class="sxs-lookup"><span data-stu-id="f4f95-133">row</span></span>|<span data-ttu-id="f4f95-134">número</span><span class="sxs-lookup"><span data-stu-id="f4f95-134">number</span></span>|<span data-ttu-id="f4f95-p105">O número da linha do intervalo a ser recuperado. Indexados com zero.</span><span class="sxs-lookup"><span data-stu-id="f4f95-p105">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="f4f95-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4f95-137">Response</span></span>

<span data-ttu-id="f4f95-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4f95-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4f95-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4f95-139">Example</span></span>
<span data-ttu-id="f4f95-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f4f95-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f4f95-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4f95-141">Request</span></span>
<span data-ttu-id="f4f95-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4f95-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_row"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Row
Content-type: application/json
Content-length: 18

{
  "row": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="f4f95-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4f95-143">Response</span></span>
<span data-ttu-id="f4f95-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4f95-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->