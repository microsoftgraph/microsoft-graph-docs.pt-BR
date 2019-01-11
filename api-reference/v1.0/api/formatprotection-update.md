---
title: Atualizar formatprotection
description: Atualiza as propriedades do objeto formatprotection.
localization_priority: Normal
ms.openlocfilehash: 26e51babc4610c331563923c464db341d4517c51
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847639"
---
# <a name="update-formatprotection"></a><span data-ttu-id="c8d2a-103">Atualizar formatprotection</span><span class="sxs-lookup"><span data-stu-id="c8d2a-103">Update formatprotection</span></span>

<span data-ttu-id="c8d2a-104">Atualiza as propriedades do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="c8d2a-104">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8d2a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8d2a-105">Permissions</span></span>
<span data-ttu-id="c8d2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8d2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8d2a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8d2a-108">Permission type</span></span>      | <span data-ttu-id="c8d2a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8d2a-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c8d2a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8d2a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8d2a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8d2a-111">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="c8d2a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8d2a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8d2a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8d2a-113">Not supported.</span></span>    | 
|<span data-ttu-id="c8d2a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8d2a-114">Application</span></span> | <span data-ttu-id="c8d2a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8d2a-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c8d2a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8d2a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="c8d2a-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c8d2a-117">Optional request headers</span></span>
| <span data-ttu-id="c8d2a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c8d2a-118">Name</span></span>       | <span data-ttu-id="c8d2a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8d2a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c8d2a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8d2a-120">Authorization</span></span>  | <span data-ttu-id="c8d2a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8d2a-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c8d2a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8d2a-123">Request body</span></span>
<span data-ttu-id="c8d2a-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c8d2a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c8d2a-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8d2a-127">Property</span></span>     | <span data-ttu-id="c8d2a-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8d2a-128">Type</span></span>   |<span data-ttu-id="c8d2a-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8d2a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8d2a-130">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="c8d2a-130">formulaHidden</span></span>|<span data-ttu-id="c8d2a-131">booliano</span><span class="sxs-lookup"><span data-stu-id="c8d2a-131">boolean</span></span>|<span data-ttu-id="c8d2a-p104">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="c8d2a-p104">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="c8d2a-134">locked</span><span class="sxs-lookup"><span data-stu-id="c8d2a-134">locked</span></span>|<span data-ttu-id="c8d2a-135">booliano</span><span class="sxs-lookup"><span data-stu-id="c8d2a-135">boolean</span></span>|<span data-ttu-id="c8d2a-p105">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="c8d2a-p105">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="c8d2a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8d2a-138">Response</span></span>

<span data-ttu-id="c8d2a-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8d2a-139">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8d2a-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8d2a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8d2a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8d2a-141">Request</span></span>
<span data-ttu-id="c8d2a-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8d2a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="c8d2a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8d2a-143">Response</span></span>
<span data-ttu-id="c8d2a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8d2a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookFormatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
