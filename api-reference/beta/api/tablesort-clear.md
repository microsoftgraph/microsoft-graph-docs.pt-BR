---
title: 'TableSort: clear'
description: Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5097498c1221a7cfd2e231232540cbef2d34a66e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521457"
---
# <a name="tablesort-clear"></a><span data-ttu-id="36629-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="36629-104">TableSort: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36629-p102">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="36629-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="36629-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="36629-107">Permissions</span></span>
<span data-ttu-id="36629-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36629-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36629-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36629-110">Permission type</span></span>      | <span data-ttu-id="36629-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36629-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36629-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36629-112">Delegated (work or school account)</span></span> | <span data-ttu-id="36629-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36629-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36629-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36629-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36629-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36629-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="36629-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36629-116">Application</span></span> | <span data-ttu-id="36629-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36629-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36629-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36629-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="36629-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36629-119">Request headers</span></span>
| <span data-ttu-id="36629-120">Nome</span><span class="sxs-lookup"><span data-stu-id="36629-120">Name</span></span>       | <span data-ttu-id="36629-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="36629-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="36629-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="36629-122">Authorization</span></span>  | <span data-ttu-id="36629-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36629-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36629-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="36629-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="36629-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="36629-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36629-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36629-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="36629-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="36629-129">Response</span></span>

<span data-ttu-id="36629-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36629-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36629-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36629-132">Example</span></span>
<span data-ttu-id="36629-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="36629-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="36629-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36629-134">Request</span></span>
<span data-ttu-id="36629-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36629-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="36629-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="36629-136">Response</span></span>
<span data-ttu-id="36629-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36629-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablesort-clear.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
