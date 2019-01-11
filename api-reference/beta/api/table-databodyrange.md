---
title: 'Table: DataBodyRange'
description: Obtém o objeto de intervalo associado ao corpo de dados da tabela.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: e8b9c6464c3e4878466a097c3d0e2399fb92e39d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820780"
---
# <a name="table-databodyrange"></a><span data-ttu-id="e78f8-103">Table: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="e78f8-103">Table: DataBodyRange</span></span>

> <span data-ttu-id="e78f8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e78f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e78f8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e78f8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e78f8-106">Obtém o objeto de intervalo associado ao corpo de dados da tabela.</span><span class="sxs-lookup"><span data-stu-id="e78f8-106">Gets the range object associated with the data body of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="e78f8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e78f8-107">Permissions</span></span>
<span data-ttu-id="e78f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e78f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e78f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e78f8-110">Permission type</span></span>      | <span data-ttu-id="e78f8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e78f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e78f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e78f8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e78f8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e78f8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e78f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e78f8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e78f8-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e78f8-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e78f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e78f8-116">Application</span></span> | <span data-ttu-id="e78f8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e78f8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e78f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e78f8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/DataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/DataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="e78f8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e78f8-119">Request headers</span></span>
| <span data-ttu-id="e78f8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e78f8-120">Name</span></span>       | <span data-ttu-id="e78f8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e78f8-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e78f8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e78f8-122">Authorization</span></span>  | <span data-ttu-id="e78f8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e78f8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e78f8-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e78f8-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e78f8-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e78f8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e78f8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e78f8-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e78f8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e78f8-129">Response</span></span>

<span data-ttu-id="e78f8-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e78f8-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e78f8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e78f8-131">Example</span></span>
<span data-ttu-id="e78f8-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e78f8-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e78f8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e78f8-133">Request</span></span>
<span data-ttu-id="e78f8-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e78f8-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_databodyrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/DataBodyRange
```

##### <a name="response"></a><span data-ttu-id="e78f8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e78f8-135">Response</span></span>
<span data-ttu-id="e78f8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e78f8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
