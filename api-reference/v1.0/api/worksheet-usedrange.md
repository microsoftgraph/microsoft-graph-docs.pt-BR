---
title: 'Worksheet: UsedRange'
description: O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 444a88dfaad3983948a139f2a3db304c200a1153
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975299"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="77765-104">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="77765-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="77765-p102">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="77765-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="77765-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="77765-107">Permissions</span></span>
<span data-ttu-id="77765-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77765-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77765-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77765-110">Permission type</span></span>      | <span data-ttu-id="77765-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77765-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77765-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77765-112">Delegated (work or school account)</span></span> | <span data-ttu-id="77765-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77765-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="77765-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77765-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77765-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77765-115">Not supported.</span></span>    |
|<span data-ttu-id="77765-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77765-116">Application</span></span> | <span data-ttu-id="77765-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77765-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77765-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77765-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="77765-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="77765-119">Function parameters</span></span>
<span data-ttu-id="77765-120">Na URL da solicitação, você pode fornecer parâmetros opcionais.</span><span class="sxs-lookup"><span data-stu-id="77765-120">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="77765-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="77765-121">Parameter</span></span>    | <span data-ttu-id="77765-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="77765-122">Type</span></span>   |<span data-ttu-id="77765-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="77765-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77765-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="77765-124">valuesOnly</span></span>|<span data-ttu-id="77765-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="77765-125">Boolean</span></span>|<span data-ttu-id="77765-p104">Opcional. Considera apenas as células com valores como células usadas (ignora a formatação).</span><span class="sxs-lookup"><span data-stu-id="77765-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="77765-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77765-128">Request headers</span></span>
| <span data-ttu-id="77765-129">Nome</span><span class="sxs-lookup"><span data-stu-id="77765-129">Name</span></span>       | <span data-ttu-id="77765-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="77765-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="77765-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="77765-131">Authorization</span></span>  | <span data-ttu-id="77765-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77765-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77765-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="77765-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="77765-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="77765-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77765-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77765-137">Request body</span></span>
<span data-ttu-id="77765-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77765-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77765-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="77765-139">Response</span></span>

<span data-ttu-id="77765-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77765-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77765-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77765-141">Example</span></span>
<span data-ttu-id="77765-142">Aqui está um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="77765-142">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="77765-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77765-143">Request</span></span>
<span data-ttu-id="77765-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77765-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="77765-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="77765-145">Response</span></span>
<span data-ttu-id="77765-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77765-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="77765-149">Como alternativa, essa função pode ser chamada com o opcional `valuesOnly` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="77765-149">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="77765-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77765-150">Request</span></span>
<span data-ttu-id="77765-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77765-151">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="77765-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="77765-152">Response</span></span>
<span data-ttu-id="77765-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77765-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
