---
title: Atualizar tablerow
description: Atualize as propriedades do objeto tablerow.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c1a1cc51a6f148127a446dcbcfa8c9573db24ade
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868317"
---
# <a name="update-tablerow"></a><span data-ttu-id="f94ea-103">Atualizar tablerow</span><span class="sxs-lookup"><span data-stu-id="f94ea-103">Update tablerow</span></span>

> <span data-ttu-id="f94ea-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f94ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f94ea-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f94ea-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f94ea-106">Atualize as propriedades do objeto tablerow.</span><span class="sxs-lookup"><span data-stu-id="f94ea-106">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f94ea-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f94ea-107">Permissions</span></span>
<span data-ttu-id="f94ea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f94ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f94ea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f94ea-110">Permission type</span></span>      | <span data-ttu-id="f94ea-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f94ea-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f94ea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f94ea-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f94ea-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f94ea-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f94ea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f94ea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f94ea-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f94ea-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f94ea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f94ea-116">Application</span></span> | <span data-ttu-id="f94ea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f94ea-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f94ea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f94ea-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows(<index>)
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="f94ea-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f94ea-119">Optional request headers</span></span>
| <span data-ttu-id="f94ea-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f94ea-120">Name</span></span>       | <span data-ttu-id="f94ea-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f94ea-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f94ea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f94ea-122">Authorization</span></span>  | <span data-ttu-id="f94ea-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f94ea-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f94ea-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f94ea-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f94ea-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f94ea-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f94ea-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f94ea-128">Request body</span></span>
<span data-ttu-id="f94ea-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f94ea-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f94ea-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f94ea-132">Property</span></span>     | <span data-ttu-id="f94ea-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f94ea-133">Type</span></span>   |<span data-ttu-id="f94ea-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f94ea-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f94ea-135">values</span><span class="sxs-lookup"><span data-stu-id="f94ea-135">values</span></span>|<span data-ttu-id="f94ea-136">json</span><span class="sxs-lookup"><span data-stu-id="f94ea-136">json</span></span>|<span data-ttu-id="f94ea-p106">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="f94ea-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="f94ea-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f94ea-140">Response</span></span>

<span data-ttu-id="f94ea-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TableRow](../resources/tablerow.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f94ea-141">If successful, this method returns a `200 OK` response code and updated [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f94ea-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f94ea-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f94ea-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f94ea-143">Request</span></span>
<span data-ttu-id="f94ea-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f94ea-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="f94ea-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f94ea-145">Response</span></span>
<span data-ttu-id="f94ea-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f94ea-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
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
