---
title: 'Range: OffsetRange'
description: Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.
ms.openlocfilehash: 301862e46a571754bcb4032c7c7bf87e3564268f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037873"
---
# <a name="range-offsetrange"></a><span data-ttu-id="053e6-105">Range: OffsetRange</span><span class="sxs-lookup"><span data-stu-id="053e6-105">Range: OffsetRange</span></span>

> <span data-ttu-id="053e6-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="053e6-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="053e6-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="053e6-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="053e6-p103">Obtém um objeto que representa um intervalo deslocado do intervalo especificado. A dimensão do intervalo retornado corresponde a esse intervalo. Se o intervalo resultante é imposto para fora dos limites da grade da planilha, o sistema gera uma exceção.</span><span class="sxs-lookup"><span data-stu-id="053e6-p103">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="053e6-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="053e6-111">Permissions</span></span>
<span data-ttu-id="053e6-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="053e6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="053e6-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="053e6-114">Permission type</span></span>      | <span data-ttu-id="053e6-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="053e6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="053e6-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="053e6-116">Delegated (work or school account)</span></span> | <span data-ttu-id="053e6-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="053e6-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="053e6-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="053e6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="053e6-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="053e6-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="053e6-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="053e6-120">Application</span></span> | <span data-ttu-id="053e6-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="053e6-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="053e6-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="053e6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="053e6-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="053e6-123">Request headers</span></span>
| <span data-ttu-id="053e6-124">Nome</span><span class="sxs-lookup"><span data-stu-id="053e6-124">Name</span></span>       | <span data-ttu-id="053e6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="053e6-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="053e6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="053e6-126">Authorization</span></span>  | <span data-ttu-id="053e6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="053e6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="053e6-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="053e6-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="053e6-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="053e6-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="053e6-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="053e6-132">Request body</span></span>
<span data-ttu-id="053e6-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="053e6-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="053e6-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="053e6-134">Parameter</span></span>    | <span data-ttu-id="053e6-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="053e6-135">Type</span></span>   |<span data-ttu-id="053e6-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="053e6-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="053e6-137">rowOffset</span><span class="sxs-lookup"><span data-stu-id="053e6-137">rowOffset</span></span>|<span data-ttu-id="053e6-138">número</span><span class="sxs-lookup"><span data-stu-id="053e6-138">number</span></span>|<span data-ttu-id="053e6-p107">O número de linhas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para baixo e os negativos, para cima.</span><span class="sxs-lookup"><span data-stu-id="053e6-p107">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="053e6-141">columnOffset</span><span class="sxs-lookup"><span data-stu-id="053e6-141">columnOffset</span></span>|<span data-ttu-id="053e6-142">número</span><span class="sxs-lookup"><span data-stu-id="053e6-142">number</span></span>|<span data-ttu-id="053e6-p108">O número de colunas (positivo, negativo ou 0) com base no qual o intervalo deve ser deslocado. Os valores positivos são deslocados para a direita e os negativos, para a esquerda.</span><span class="sxs-lookup"><span data-stu-id="053e6-p108">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="053e6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="053e6-145">Response</span></span>

<span data-ttu-id="053e6-146">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="053e6-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="053e6-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="053e6-147">Example</span></span>
<span data-ttu-id="053e6-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="053e6-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="053e6-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="053e6-149">Request</span></span>
<span data-ttu-id="053e6-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="053e6-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="053e6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="053e6-151">Response</span></span>
<span data-ttu-id="053e6-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="053e6-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->