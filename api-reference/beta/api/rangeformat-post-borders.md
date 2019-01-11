---
title: Criar RangeBorder
description: Use essa API para criar uma nova RangeBorder.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 3d6ed5337d3dc4c674739f7c3f70838757799566
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845462"
---
# <a name="create-rangeborder"></a><span data-ttu-id="e6a0a-103">Criar RangeBorder</span><span class="sxs-lookup"><span data-stu-id="e6a0a-103">Create RangeBorder</span></span>

> <span data-ttu-id="e6a0a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e6a0a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6a0a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e6a0a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6a0a-106">Use essa API para criar uma nova RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="e6a0a-106">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6a0a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6a0a-107">Permissions</span></span>
<span data-ttu-id="e6a0a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6a0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6a0a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6a0a-110">Permission type</span></span>      | <span data-ttu-id="e6a0a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6a0a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6a0a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6a0a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6a0a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6a0a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6a0a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6a0a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6a0a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6a0a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6a0a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6a0a-116">Application</span></span> | <span data-ttu-id="e6a0a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6a0a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6a0a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6a0a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="e6a0a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6a0a-119">Request headers</span></span>
| <span data-ttu-id="e6a0a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e6a0a-120">Name</span></span>       | <span data-ttu-id="e6a0a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6a0a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6a0a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6a0a-122">Authorization</span></span>  | <span data-ttu-id="e6a0a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6a0a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6a0a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e6a0a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e6a0a-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e6a0a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6a0a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6a0a-128">Request body</span></span>
<span data-ttu-id="e6a0a-129">No corpo da solicitação, forneça uma representação JSON do objeto [RangeBorder](../resources/rangeborder.md).</span><span class="sxs-lookup"><span data-stu-id="e6a0a-129">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e6a0a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6a0a-130">Response</span></span>

<span data-ttu-id="e6a0a-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [RangeBorder](../resources/rangeborder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6a0a-131">If successful, this method returns `201 Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6a0a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6a0a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6a0a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6a0a-133">Request</span></span>
<span data-ttu-id="e6a0a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6a0a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
<span data-ttu-id="e6a0a-135">No corpo da solicitação, forneça uma representação JSON do objeto [RangeBorder](../resources/rangeborder.md).</span><span class="sxs-lookup"><span data-stu-id="e6a0a-135">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e6a0a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6a0a-136">Response</span></span>
<span data-ttu-id="e6a0a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6a0a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
