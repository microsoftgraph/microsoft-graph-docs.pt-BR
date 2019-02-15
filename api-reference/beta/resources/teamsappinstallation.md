---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f6ff72ab99d20eba9880630248e4b61fca5c2521
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057012"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="1aa01-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1aa01-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1aa01-104">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="1aa01-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="1aa01-105">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe à qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="1aa01-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="1aa01-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1aa01-106">Methods</span></span>

| <span data-ttu-id="1aa01-107">Método</span><span class="sxs-lookup"><span data-stu-id="1aa01-107">Method</span></span>       | <span data-ttu-id="1aa01-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1aa01-108">Return Type</span></span>  |<span data-ttu-id="1aa01-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aa01-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1aa01-110">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="1aa01-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="1aa01-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1aa01-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="1aa01-112">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="1aa01-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="1aa01-113">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="1aa01-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="1aa01-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1aa01-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="1aa01-115">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="1aa01-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="1aa01-116">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="1aa01-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="1aa01-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1aa01-117">None</span></span> | <span data-ttu-id="1aa01-118">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="1aa01-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="1aa01-119">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="1aa01-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="1aa01-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1aa01-120">None</span></span> | <span data-ttu-id="1aa01-121">Atualiza para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1aa01-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="1aa01-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1aa01-122">Properties</span></span>

| <span data-ttu-id="1aa01-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1aa01-123">Property</span></span>            | <span data-ttu-id="1aa01-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1aa01-124">Type</span></span>     | <span data-ttu-id="1aa01-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aa01-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1aa01-126">id</span><span class="sxs-lookup"><span data-stu-id="1aa01-126">id</span></span>                  | <span data-ttu-id="1aa01-127">string</span><span class="sxs-lookup"><span data-stu-id="1aa01-127">string</span></span>   | <span data-ttu-id="1aa01-128">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="1aa01-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="1aa01-129">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="1aa01-129">Relationships</span></span>

| <span data-ttu-id="1aa01-130">Relação</span><span class="sxs-lookup"><span data-stu-id="1aa01-130">Relationship</span></span>   | <span data-ttu-id="1aa01-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1aa01-131">Type</span></span>    | <span data-ttu-id="1aa01-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aa01-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1aa01-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1aa01-133">teamsApp</span></span>|[<span data-ttu-id="1aa01-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1aa01-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="1aa01-135">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="1aa01-135">The app that is installed.</span></span> |
|<span data-ttu-id="1aa01-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1aa01-136">teamsAppDefinition</span></span>|[<span data-ttu-id="1aa01-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1aa01-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="1aa01-138">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1aa01-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1aa01-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1aa01-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="1aa01-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="1aa01-140">See also</span></span>

- [<span data-ttu-id="1aa01-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1aa01-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="1aa01-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1aa01-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="1aa01-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1aa01-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstallation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

