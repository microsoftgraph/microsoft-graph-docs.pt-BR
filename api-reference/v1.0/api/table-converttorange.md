---
title: 'Table: convertToRange'
description: Converte a tabela em um intervalo de células normal. Todos os dados são preservados.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2cda7e4eac082938cafb8328063658071eeb01d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560848"
---
# <a name="table-converttorange"></a><span data-ttu-id="584e1-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="584e1-104">Table: convertToRange</span></span>

<span data-ttu-id="584e1-p102">Converte a tabela em um intervalo de células normal. Todos os dados são preservados.</span><span class="sxs-lookup"><span data-stu-id="584e1-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="584e1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="584e1-107">Permissions</span></span>
<span data-ttu-id="584e1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="584e1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="584e1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="584e1-110">Permission type</span></span>      | <span data-ttu-id="584e1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="584e1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="584e1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="584e1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="584e1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="584e1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="584e1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="584e1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="584e1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="584e1-115">Not supported.</span></span>    |
|<span data-ttu-id="584e1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="584e1-116">Application</span></span> | <span data-ttu-id="584e1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="584e1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="584e1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="584e1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="584e1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="584e1-119">Request headers</span></span>
| <span data-ttu-id="584e1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="584e1-120">Name</span></span>       | <span data-ttu-id="584e1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="584e1-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="584e1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="584e1-122">Authorization</span></span>  | <span data-ttu-id="584e1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="584e1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="584e1-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="584e1-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="584e1-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="584e1-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="584e1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="584e1-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="584e1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="584e1-129">Response</span></span>

<span data-ttu-id="584e1-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="584e1-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="584e1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="584e1-131">Example</span></span>
<span data-ttu-id="584e1-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="584e1-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="584e1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="584e1-133">Request</span></span>
<span data-ttu-id="584e1-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="584e1-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="584e1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="584e1-135">Response</span></span>
<span data-ttu-id="584e1-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="584e1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
