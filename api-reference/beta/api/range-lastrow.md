---
title: 'Range: LastRow'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1a3f90c4962c2df11f959c23fccebb2fab289f90
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931418"
---
# <a name="range-lastrow"></a><span data-ttu-id="4ae55-103">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="4ae55-103">Range: LastRow</span></span>

> <span data-ttu-id="4ae55-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ae55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ae55-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ae55-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ae55-p102">Obtém a última linha do intervalo. Por exemplo, a última linha de "B2:D5" é "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="4ae55-p102">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="4ae55-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ae55-108">Permissions</span></span>
<span data-ttu-id="4ae55-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ae55-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ae55-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ae55-111">Permission type</span></span>      | <span data-ttu-id="4ae55-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ae55-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ae55-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ae55-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4ae55-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ae55-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4ae55-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ae55-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ae55-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ae55-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4ae55-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ae55-117">Application</span></span> | <span data-ttu-id="4ae55-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ae55-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ae55-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ae55-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="4ae55-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ae55-120">Request headers</span></span>
| <span data-ttu-id="4ae55-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4ae55-121">Name</span></span>       | <span data-ttu-id="4ae55-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ae55-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4ae55-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ae55-123">Authorization</span></span>  | <span data-ttu-id="4ae55-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ae55-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ae55-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4ae55-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="4ae55-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4ae55-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ae55-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ae55-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4ae55-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ae55-130">Response</span></span>

<span data-ttu-id="4ae55-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ae55-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ae55-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ae55-132">Example</span></span>
<span data-ttu-id="4ae55-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4ae55-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ae55-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ae55-134">Request</span></span>
<span data-ttu-id="4ae55-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ae55-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="4ae55-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ae55-136">Response</span></span>
<span data-ttu-id="4ae55-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ae55-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
