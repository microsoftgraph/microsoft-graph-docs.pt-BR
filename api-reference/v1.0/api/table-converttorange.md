---
title: 'Table: convertToRange'
description: Converte a tabela em um intervalo de células normal. Todos os dados são preservados.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4528daab7cfde480e93d75cdcb5f9a969f583144
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825372"
---
# <a name="table-converttorange"></a><span data-ttu-id="de69e-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="de69e-104">Table: convertToRange</span></span>

<span data-ttu-id="de69e-p102">Converte a tabela em um intervalo de células normal. Todos os dados são preservados.</span><span class="sxs-lookup"><span data-stu-id="de69e-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="de69e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="de69e-107">Permissions</span></span>
<span data-ttu-id="de69e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de69e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de69e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de69e-110">Permission type</span></span>      | <span data-ttu-id="de69e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de69e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de69e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de69e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="de69e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de69e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="de69e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de69e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de69e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de69e-115">Not supported.</span></span>    |
|<span data-ttu-id="de69e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de69e-116">Application</span></span> | <span data-ttu-id="de69e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de69e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de69e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de69e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="de69e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de69e-119">Request headers</span></span>
| <span data-ttu-id="de69e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="de69e-120">Name</span></span>       | <span data-ttu-id="de69e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="de69e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="de69e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="de69e-122">Authorization</span></span>  | <span data-ttu-id="de69e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de69e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de69e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="de69e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="de69e-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="de69e-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de69e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de69e-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="de69e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="de69e-129">Response</span></span>

<span data-ttu-id="de69e-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de69e-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de69e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de69e-131">Example</span></span>
<span data-ttu-id="de69e-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="de69e-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="de69e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de69e-133">Request</span></span>
<span data-ttu-id="de69e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de69e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="de69e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="de69e-135">Response</span></span>
<span data-ttu-id="de69e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de69e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
