---
title: Atualizar um aplicativo em uma equipe
description: Atualiza uma instalação de aplicativo em uma equipe
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9ef5c41c8b09512b0ee6ebb888be1df1166cf9c5
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30056977"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="ca00a-103">Atualizar um aplicativo em uma equipe</span><span class="sxs-lookup"><span data-stu-id="ca00a-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca00a-104">Atualiza uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca00a-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

><span data-ttu-id="ca00a-105">**Observação:** Se você estiver usando permissões de aplicativo, ocorrerá um problema conhecido.</span><span class="sxs-lookup"><span data-stu-id="ca00a-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="ca00a-106">Para saber mais, confira [problemas conhecidos](graph/concepts/known-issues.md).</span><span class="sxs-lookup"><span data-stu-id="ca00a-106">For details, see [known issues](graph/concepts/known-issues.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca00a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca00a-107">Permissions</span></span>

<span data-ttu-id="ca00a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca00a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca00a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca00a-110">Permission type</span></span>      | <span data-ttu-id="ca00a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca00a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca00a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca00a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ca00a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca00a-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca00a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca00a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca00a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca00a-115">Not supported.</span></span>    |
|<span data-ttu-id="ca00a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca00a-116">Application</span></span> | <span data-ttu-id="ca00a-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca00a-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca00a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca00a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="ca00a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca00a-119">Request headers</span></span>
| <span data-ttu-id="ca00a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca00a-120">Header</span></span>       | <span data-ttu-id="ca00a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ca00a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ca00a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca00a-122">Authorization</span></span>  | <span data-ttu-id="ca00a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca00a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ca00a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca00a-125">Request body</span></span>
<span data-ttu-id="ca00a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca00a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca00a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca00a-127">Response</span></span>

<span data-ttu-id="ca00a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca00a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca00a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca00a-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ca00a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca00a-131">Request</span></span>
<span data-ttu-id="ca00a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca00a-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="ca00a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca00a-133">Response</span></span>
<span data-ttu-id="ca00a-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ca00a-134">The following is an example of the response.</span></span> 

><span data-ttu-id="ca00a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca00a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
