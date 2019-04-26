---
title: 'Table: convertToRange'
description: Converte a tabela em um intervalo de células normal. Todos os dados são preservados.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8ecd7dfddbfabc893663e9297b7aed05c1c30358
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330569"
---
# <a name="table-converttorange"></a><span data-ttu-id="fc718-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="fc718-104">Table: convertToRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc718-p102">Converte a tabela em um intervalo de células normal. Todos os dados são preservados.</span><span class="sxs-lookup"><span data-stu-id="fc718-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc718-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc718-107">Permissions</span></span>
<span data-ttu-id="fc718-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc718-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc718-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc718-110">Permission type</span></span>      | <span data-ttu-id="fc718-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc718-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc718-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc718-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc718-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc718-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc718-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc718-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc718-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc718-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc718-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc718-116">Application</span></span> | <span data-ttu-id="fc718-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc718-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc718-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc718-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="fc718-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc718-119">Request headers</span></span>
| <span data-ttu-id="fc718-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fc718-120">Name</span></span>       | <span data-ttu-id="fc718-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc718-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc718-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc718-122">Authorization</span></span>  | <span data-ttu-id="fc718-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc718-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc718-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fc718-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc718-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fc718-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc718-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc718-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="fc718-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc718-129">Response</span></span>

<span data-ttu-id="fc718-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc718-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc718-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc718-131">Example</span></span>
<span data-ttu-id="fc718-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fc718-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc718-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc718-133">Request</span></span>
<span data-ttu-id="fc718-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc718-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="fc718-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc718-135">Response</span></span>
<span data-ttu-id="fc718-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc718-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
