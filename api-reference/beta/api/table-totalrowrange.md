---
title: 'Table: TotalRowRange'
description: Obtém o objeto de intervalo associado à linha de totais da tabela.
author: lumine2008
ms.openlocfilehash: 7e2526c8082aa495e507db6db77c2f96928b3525
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303469"
---
# <a name="table-totalrowrange"></a><span data-ttu-id="0e87a-103">Table: TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="0e87a-103">Table: TotalRowRange</span></span>

> <span data-ttu-id="0e87a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0e87a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e87a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0e87a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e87a-106">Obtém o objeto de intervalo associado à linha de totais da tabela.</span><span class="sxs-lookup"><span data-stu-id="0e87a-106">Gets the range object associated with totals row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e87a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e87a-107">Permissions</span></span>
<span data-ttu-id="0e87a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e87a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e87a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e87a-110">Permission type</span></span>      | <span data-ttu-id="0e87a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e87a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e87a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e87a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0e87a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e87a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e87a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e87a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e87a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e87a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e87a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e87a-116">Application</span></span> | <span data-ttu-id="0e87a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e87a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e87a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e87a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/TotalRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/TotalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="0e87a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e87a-119">Request headers</span></span>
| <span data-ttu-id="0e87a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0e87a-120">Name</span></span>       | <span data-ttu-id="0e87a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e87a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e87a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e87a-122">Authorization</span></span>  | <span data-ttu-id="0e87a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e87a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e87a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0e87a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e87a-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0e87a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e87a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e87a-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0e87a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e87a-129">Response</span></span>

<span data-ttu-id="0e87a-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e87a-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e87a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e87a-131">Example</span></span>
<span data-ttu-id="0e87a-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0e87a-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e87a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e87a-133">Request</span></span>
<span data-ttu-id="0e87a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e87a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_totalrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/TotalRowRange
```

##### <a name="response"></a><span data-ttu-id="0e87a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e87a-135">Response</span></span>
<span data-ttu-id="0e87a-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e87a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->