---
title: Excluir um canal
description: Exclua o canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 734df0a79881993f4e002562e5125305b624c4c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525329"
---
# <a name="delete-channel"></a><span data-ttu-id="ba4a1-103">Excluir um canal</span><span class="sxs-lookup"><span data-stu-id="ba4a1-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba4a1-104">Exclua o [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ba4a1-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="ba4a1-105">**Observação**: não há um problema conhecido com permissões de aplicativo e essa API.</span><span class="sxs-lookup"><span data-stu-id="ba4a1-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="ba4a1-106">Para obter detalhes, consulte a [lista de problemas conhecidos do](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="ba4a1-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba4a1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba4a1-107">Permissions</span></span>
<span data-ttu-id="ba4a1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba4a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba4a1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba4a1-110">Permission type</span></span>      | <span data-ttu-id="ba4a1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba4a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba4a1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba4a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba4a1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba4a1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba4a1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba4a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba4a1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba4a1-115">Not supported.</span></span>    |
|<span data-ttu-id="ba4a1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba4a1-116">Application</span></span> | <span data-ttu-id="ba4a1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba4a1-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="ba4a1-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="ba4a1-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ba4a1-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="ba4a1-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ba4a1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba4a1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ba4a1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba4a1-121">Request headers</span></span>
| <span data-ttu-id="ba4a1-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba4a1-122">Header</span></span>       | <span data-ttu-id="ba4a1-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ba4a1-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba4a1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba4a1-124">Authorization</span></span>  | <span data-ttu-id="ba4a1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba4a1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba4a1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba4a1-127">Request body</span></span>
<span data-ttu-id="ba4a1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba4a1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba4a1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba4a1-129">Response</span></span>

<span data-ttu-id="ba4a1-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba4a1-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba4a1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba4a1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba4a1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba4a1-133">Request</span></span>
<span data-ttu-id="ba4a1-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba4a1-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="ba4a1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba4a1-135">Response</span></span>

<span data-ttu-id="ba4a1-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba4a1-136">The following is an example of the response.</span></span> 
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
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
