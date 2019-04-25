---
title: Adicionar aplicativo à equipe
description: Instala um aplicativo para a equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1a77d3b01c70273d0d93ca1e3b1b66d1de53f8f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544649"
---
# <a name="add-app-to-team"></a><span data-ttu-id="cfdeb-103">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="cfdeb-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfdeb-104">Instala um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="cfdeb-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cfdeb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cfdeb-105">Permissions</span></span>
<span data-ttu-id="cfdeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfdeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfdeb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfdeb-108">Permission type</span></span>      | <span data-ttu-id="cfdeb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfdeb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfdeb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfdeb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfdeb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdeb-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cfdeb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfdeb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfdeb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfdeb-113">Not supported.</span></span>    |
|<span data-ttu-id="cfdeb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfdeb-114">Application</span></span> | <span data-ttu-id="cfdeb-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdeb-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfdeb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfdeb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="cfdeb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdeb-117">Request headers</span></span>
| <span data-ttu-id="cfdeb-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfdeb-118">Header</span></span>       | <span data-ttu-id="cfdeb-119">Valor</span><span class="sxs-lookup"><span data-stu-id="cfdeb-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cfdeb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfdeb-120">Authorization</span></span>  | <span data-ttu-id="cfdeb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfdeb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cfdeb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdeb-123">Request body</span></span>

| <span data-ttu-id="cfdeb-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfdeb-124">Property</span></span>     | <span data-ttu-id="cfdeb-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfdeb-125">Type</span></span>   |<span data-ttu-id="cfdeb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfdeb-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfdeb-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cfdeb-127">teamsApp</span></span>|<span data-ttu-id="cfdeb-128">String</span><span class="sxs-lookup"><span data-stu-id="cfdeb-128">String</span></span>|<span data-ttu-id="cfdeb-129">A ID do aplicativo a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="cfdeb-129">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="cfdeb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfdeb-130">Response</span></span>

<span data-ttu-id="cfdeb-131">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="cfdeb-131">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="cfdeb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfdeb-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cfdeb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdeb-133">Request</span></span>
<span data-ttu-id="cfdeb-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfdeb-134">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="cfdeb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfdeb-135">Response</span></span>
<span data-ttu-id="cfdeb-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cfdeb-136">The following is an example of the response.</span></span> <span data-ttu-id="cfdeb-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="cfdeb-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cfdeb-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfdeb-138">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="cfdeb-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="cfdeb-139">See also</span></span>

