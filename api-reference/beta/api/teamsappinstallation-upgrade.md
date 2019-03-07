---
title: Atualizar um aplicativo em uma equipe
description: Atualiza uma instalação de aplicativo em uma equipe
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1000bcbb8aeaa26cd1b580bd4c11a4018a3a82f9
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458642"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="66461-103">Atualizar um aplicativo em uma equipe</span><span class="sxs-lookup"><span data-stu-id="66461-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66461-104">Atualiza uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66461-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="66461-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="66461-105">Permissions</span></span>

<span data-ttu-id="66461-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66461-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66461-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66461-108">Permission type</span></span>      | <span data-ttu-id="66461-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66461-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66461-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66461-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66461-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66461-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="66461-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66461-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66461-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66461-113">Not supported.</span></span>    |
|<span data-ttu-id="66461-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66461-114">Application</span></span> | <span data-ttu-id="66461-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66461-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66461-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66461-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="66461-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66461-117">Request headers</span></span>
| <span data-ttu-id="66461-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66461-118">Header</span></span>       | <span data-ttu-id="66461-119">Valor</span><span class="sxs-lookup"><span data-stu-id="66461-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="66461-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="66461-120">Authorization</span></span>  | <span data-ttu-id="66461-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66461-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="66461-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66461-123">Request body</span></span>
<span data-ttu-id="66461-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66461-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66461-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="66461-125">Response</span></span>

<span data-ttu-id="66461-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66461-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66461-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66461-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="66461-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66461-129">Request</span></span>
<span data-ttu-id="66461-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66461-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="66461-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="66461-131">Response</span></span>
<span data-ttu-id="66461-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66461-132">The following is an example of the response.</span></span> 

><span data-ttu-id="66461-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66461-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsappinstallation-upgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
