---
title: Atualizar tablecolumn
description: Atualize as propriedades do objeto tablecolumn.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: e3e6bc61f66af286e348610c2463b6aad611f49c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806129"
---
# <a name="update-tablecolumn"></a><span data-ttu-id="181b7-103">Atualizar tablecolumn</span><span class="sxs-lookup"><span data-stu-id="181b7-103">Update tablecolumn</span></span>

> <span data-ttu-id="181b7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="181b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="181b7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="181b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="181b7-106">Atualize as propriedades do objeto tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="181b7-106">Update the properties of tablecolumn object.</span></span>
## <a name="permissions"></a><span data-ttu-id="181b7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="181b7-107">Permissions</span></span>
<span data-ttu-id="181b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="181b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="181b7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="181b7-110">Permission type</span></span>      | <span data-ttu-id="181b7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="181b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="181b7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="181b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="181b7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="181b7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="181b7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="181b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="181b7-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="181b7-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="181b7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="181b7-116">Application</span></span> | <span data-ttu-id="181b7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="181b7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="181b7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="181b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/columns/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="181b7-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="181b7-119">Optional request headers</span></span>
| <span data-ttu-id="181b7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="181b7-120">Name</span></span>       | <span data-ttu-id="181b7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="181b7-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="181b7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="181b7-122">Authorization</span></span>  | <span data-ttu-id="181b7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="181b7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="181b7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="181b7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="181b7-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="181b7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="181b7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="181b7-128">Request body</span></span>
<span data-ttu-id="181b7-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="181b7-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="181b7-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="181b7-132">Property</span></span>     | <span data-ttu-id="181b7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="181b7-133">Type</span></span>   |<span data-ttu-id="181b7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="181b7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="181b7-135">values</span><span class="sxs-lookup"><span data-stu-id="181b7-135">values</span></span>|<span data-ttu-id="181b7-136">json</span><span class="sxs-lookup"><span data-stu-id="181b7-136">json</span></span>|<span data-ttu-id="181b7-p106">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="181b7-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="181b7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="181b7-140">Response</span></span>

<span data-ttu-id="181b7-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TableColumn](../resources/tablecolumn.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="181b7-141">If successful, this method returns a `200 OK` response code and updated [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="181b7-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="181b7-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="181b7-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="181b7-143">Request</span></span>
<span data-ttu-id="181b7-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="181b7-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablecolumn"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
Content-type: application/json
Content-length: 81

{
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="181b7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="181b7-145">Response</span></span>
<span data-ttu-id="181b7-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="181b7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablecolumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
