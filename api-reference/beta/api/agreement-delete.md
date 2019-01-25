---
title: Excluir contrato
description: Exclua um objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: 95766f28e5456c1b4f410de65ae12dccd881727e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521317"
---
# <a name="delete-agreement"></a><span data-ttu-id="ebefb-103">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="ebefb-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebefb-104">Exclua um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="ebefb-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebefb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ebefb-105">Permissions</span></span>
<span data-ttu-id="ebefb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebefb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebefb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebefb-108">Permission type</span></span>                        | <span data-ttu-id="ebefb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebefb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebefb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebefb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ebefb-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebefb-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="ebefb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebefb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebefb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebefb-113">Not supported.</span></span> |
|<span data-ttu-id="ebefb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebefb-114">Application</span></span>                            | <span data-ttu-id="ebefb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebefb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebefb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebefb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="ebefb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebefb-117">Request headers</span></span>
| <span data-ttu-id="ebefb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ebefb-118">Name</span></span>         | <span data-ttu-id="ebefb-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebefb-119">Type</span></span>        | <span data-ttu-id="ebefb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebefb-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ebefb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebefb-121">Authorization</span></span> | <span data-ttu-id="ebefb-122">string</span><span class="sxs-lookup"><span data-stu-id="ebefb-122">string</span></span> | <span data-ttu-id="ebefb-123">Token de portador</span><span class="sxs-lookup"><span data-stu-id="ebefb-123">Bearer \{token\}.</span></span> <span data-ttu-id="ebefb-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebefb-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebefb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebefb-125">Request body</span></span>
<span data-ttu-id="ebefb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ebefb-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ebefb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebefb-127">Response</span></span>
<span data-ttu-id="ebefb-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebefb-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebefb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebefb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebefb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebefb-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/<id>
```
##### <a name="response"></a><span data-ttu-id="ebefb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebefb-132">Response</span></span>
><span data-ttu-id="ebefb-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebefb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
