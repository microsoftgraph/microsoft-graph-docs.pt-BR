---
title: Adicionar aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 35d2521d9bff37ea45f7496a825429762daaf8f7
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30056991"
---
# <a name="add-app-to-team"></a><span data-ttu-id="81147-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="81147-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81147-104">Instala um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="81147-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="81147-105">**Observação:** Se você estiver usando permissões de aplicativo, ocorrerá um problema conhecido.</span><span class="sxs-lookup"><span data-stu-id="81147-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="81147-106">Para saber mais, confira [problemas conhecidos](graph/concepts/known-issues.md).</span><span class="sxs-lookup"><span data-stu-id="81147-106">For details, see [known issues](graph/concepts/known-issues.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="81147-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="81147-107">Permissions</span></span>
<span data-ttu-id="81147-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81147-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81147-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81147-110">Permission type</span></span>      | <span data-ttu-id="81147-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81147-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81147-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81147-112">Delegated (work or school account)</span></span> | <span data-ttu-id="81147-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81147-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="81147-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81147-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81147-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81147-115">Not supported.</span></span>    |
|<span data-ttu-id="81147-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81147-116">Application</span></span> | <span data-ttu-id="81147-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81147-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81147-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81147-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="81147-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81147-119">Request headers</span></span>
| <span data-ttu-id="81147-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81147-120">Header</span></span>       | <span data-ttu-id="81147-121">Valor</span><span class="sxs-lookup"><span data-stu-id="81147-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="81147-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81147-122">Authorization</span></span>  | <span data-ttu-id="81147-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81147-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81147-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81147-125">Request body</span></span>

| <span data-ttu-id="81147-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81147-126">Property</span></span>     | <span data-ttu-id="81147-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="81147-127">Type</span></span>   |<span data-ttu-id="81147-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="81147-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81147-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="81147-129">teamsApp</span></span>|<span data-ttu-id="81147-130">String</span><span class="sxs-lookup"><span data-stu-id="81147-130">String</span></span>|<span data-ttu-id="81147-131">A ID do aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="81147-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="81147-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="81147-132">Response</span></span>

<span data-ttu-id="81147-133">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="81147-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="81147-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81147-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="81147-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81147-135">Request</span></span>
<span data-ttu-id="81147-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81147-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="81147-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="81147-137">Response</span></span>
<span data-ttu-id="81147-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81147-138">The following is an example of the response.</span></span> <span data-ttu-id="81147-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="81147-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="81147-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81147-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
}
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
    "Error: /api-reference/beta/api/teamsappinstallation-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="81147-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="81147-141">See also</span></span>

