---
title: 'Filter: clear'
description: Limpa o filtro na coluna determinada.
localization_priority: Normal
ms.openlocfilehash: 3567ee187a9b3becb1afa296c97cc7c3442bf667
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518034"
---
# <a name="filter-clear"></a><span data-ttu-id="6d872-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="6d872-103">Filter: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d872-104">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="6d872-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="6d872-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d872-105">Permissions</span></span>
<span data-ttu-id="6d872-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d872-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d872-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d872-108">Permission type</span></span>      | <span data-ttu-id="6d872-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d872-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d872-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d872-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d872-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d872-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6d872-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d872-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d872-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d872-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6d872-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d872-114">Application</span></span> | <span data-ttu-id="6d872-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d872-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d872-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d872-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="6d872-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d872-117">Request headers</span></span>
| <span data-ttu-id="6d872-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6d872-118">Name</span></span>       | <span data-ttu-id="6d872-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d872-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6d872-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d872-120">Authorization</span></span>  | <span data-ttu-id="6d872-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d872-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d872-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d872-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6d872-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d872-124">Response</span></span>

<span data-ttu-id="6d872-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d872-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d872-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d872-127">Example</span></span>
<span data-ttu-id="6d872-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6d872-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6d872-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d872-129">Request</span></span>
<span data-ttu-id="6d872-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d872-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="6d872-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d872-131">Response</span></span>
<span data-ttu-id="6d872-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d872-132">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/filter-clear.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
