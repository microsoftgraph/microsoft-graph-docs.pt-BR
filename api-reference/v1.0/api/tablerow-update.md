---
title: Atualizar tablerow
description: Atualize as propriedades do objeto tablerow.
author: lumine2008
ms.openlocfilehash: 3990885ac237ccfe5e7a01c71353b0ec44d1a14d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314256"
---
# <a name="update-tablerow"></a><span data-ttu-id="fdb91-103">Atualizar tablerow</span><span class="sxs-lookup"><span data-stu-id="fdb91-103">Update tablerow</span></span>

<span data-ttu-id="fdb91-104">Atualize as propriedades do objeto tablerow.</span><span class="sxs-lookup"><span data-stu-id="fdb91-104">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fdb91-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdb91-105">Permissions</span></span>
<span data-ttu-id="fdb91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdb91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdb91-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdb91-108">Permission type</span></span>      | <span data-ttu-id="fdb91-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdb91-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdb91-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdb91-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fdb91-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdb91-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fdb91-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdb91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdb91-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdb91-113">Not supported.</span></span>    |
|<span data-ttu-id="fdb91-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdb91-114">Application</span></span> | <span data-ttu-id="fdb91-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdb91-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdb91-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdb91-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows/{index}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-request-headers"></a><span data-ttu-id="fdb91-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="fdb91-117">Optional request headers</span></span>
| <span data-ttu-id="fdb91-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fdb91-118">Name</span></span>       | <span data-ttu-id="fdb91-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdb91-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fdb91-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdb91-120">Authorization</span></span>  | <span data-ttu-id="fdb91-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdb91-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fdb91-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fdb91-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fdb91-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fdb91-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdb91-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb91-126">Request body</span></span>
<span data-ttu-id="fdb91-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="fdb91-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fdb91-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdb91-130">Property</span></span>     | <span data-ttu-id="fdb91-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdb91-131">Type</span></span>   |<span data-ttu-id="fdb91-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdb91-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdb91-133">values</span><span class="sxs-lookup"><span data-stu-id="fdb91-133">values</span></span>|<span data-ttu-id="fdb91-134">Json</span><span class="sxs-lookup"><span data-stu-id="fdb91-134">Json</span></span>|<span data-ttu-id="fdb91-p105">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="fdb91-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="fdb91-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdb91-138">Response</span></span>

<span data-ttu-id="fdb91-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [WorkbookTableRow](../resources/tablerow.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdb91-139">If successful, this method returns a `200 OK` response code and updated [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fdb91-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdb91-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fdb91-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb91-141">Request</span></span>
<span data-ttu-id="fdb91-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdb91-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="fdb91-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdb91-143">Response</span></span>
<span data-ttu-id="fdb91-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdb91-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->