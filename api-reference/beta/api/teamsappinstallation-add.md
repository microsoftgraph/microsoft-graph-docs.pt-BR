---
title: Adicionar o aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 353298dc43479057e689f43e3a7274523468caee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516823"
---
# <a name="add-app-to-team"></a><span data-ttu-id="42326-103">Adicionar o aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="42326-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42326-104">Instala um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="42326-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="42326-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="42326-105">Permissions</span></span>
<span data-ttu-id="42326-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42326-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42326-108">Permission type</span></span>      | <span data-ttu-id="42326-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42326-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42326-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42326-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42326-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42326-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="42326-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42326-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42326-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42326-113">Not supported.</span></span>    |
|<span data-ttu-id="42326-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42326-114">Application</span></span> | <span data-ttu-id="42326-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42326-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42326-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42326-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="42326-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42326-117">Request headers</span></span>
| <span data-ttu-id="42326-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42326-118">Header</span></span>       | <span data-ttu-id="42326-119">Valor</span><span class="sxs-lookup"><span data-stu-id="42326-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42326-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="42326-120">Authorization</span></span>  | <span data-ttu-id="42326-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42326-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="42326-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42326-123">Request body</span></span>

| <span data-ttu-id="42326-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42326-124">Property</span></span>     | <span data-ttu-id="42326-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="42326-125">Type</span></span>   |<span data-ttu-id="42326-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="42326-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42326-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="42326-127">teamsApp</span></span>|<span data-ttu-id="42326-128">String</span><span class="sxs-lookup"><span data-stu-id="42326-128">String</span></span>|<span data-ttu-id="42326-129">A id do aplicativo para adicionar.</span><span class="sxs-lookup"><span data-stu-id="42326-129">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="42326-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="42326-130">Response</span></span>

<span data-ttu-id="42326-131">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="42326-131">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="42326-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42326-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="42326-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42326-133">Request</span></span>
<span data-ttu-id="42326-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42326-134">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="42326-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="42326-135">Response</span></span>
<span data-ttu-id="42326-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42326-136">The following is an example of the response.</span></span> <span data-ttu-id="42326-137">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="42326-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="42326-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42326-138">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="42326-139">Veja também</span><span class="sxs-lookup"><span data-stu-id="42326-139">See also</span></span>

