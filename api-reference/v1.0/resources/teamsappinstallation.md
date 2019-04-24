---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c98f1b927c319eb1d81573fd9dc43e1baad86a39
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462351"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="1da39-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1da39-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1da39-104">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="1da39-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="1da39-105">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe à qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="1da39-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="1da39-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1da39-106">Methods</span></span>

| <span data-ttu-id="1da39-107">Método</span><span class="sxs-lookup"><span data-stu-id="1da39-107">Method</span></span>       | <span data-ttu-id="1da39-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1da39-108">Return Type</span></span>  |<span data-ttu-id="1da39-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1da39-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1da39-110">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="1da39-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="1da39-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1da39-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="1da39-112">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="1da39-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="1da39-113">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="1da39-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="1da39-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1da39-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="1da39-115">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="1da39-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="1da39-116">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="1da39-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="1da39-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1da39-117">None</span></span> | <span data-ttu-id="1da39-118">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="1da39-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="1da39-119">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="1da39-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="1da39-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1da39-120">None</span></span> | <span data-ttu-id="1da39-121">Atualiza para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1da39-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="1da39-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1da39-122">Properties</span></span>

| <span data-ttu-id="1da39-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1da39-123">Property</span></span>            | <span data-ttu-id="1da39-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1da39-124">Type</span></span>     | <span data-ttu-id="1da39-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1da39-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1da39-126">id</span><span class="sxs-lookup"><span data-stu-id="1da39-126">id</span></span>                  | <span data-ttu-id="1da39-127">string</span><span class="sxs-lookup"><span data-stu-id="1da39-127">string</span></span>   | <span data-ttu-id="1da39-128">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="1da39-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="1da39-129">Relações</span><span class="sxs-lookup"><span data-stu-id="1da39-129">Relationships</span></span>

| <span data-ttu-id="1da39-130">Relação</span><span class="sxs-lookup"><span data-stu-id="1da39-130">Relationship</span></span>   | <span data-ttu-id="1da39-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1da39-131">Type</span></span>    | <span data-ttu-id="1da39-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1da39-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1da39-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1da39-133">teamsApp</span></span>|[<span data-ttu-id="1da39-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1da39-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="1da39-135">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="1da39-135">The app that is installed.</span></span> |
|<span data-ttu-id="1da39-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1da39-136">teamsAppDefinition</span></span>|[<span data-ttu-id="1da39-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1da39-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="1da39-138">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1da39-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1da39-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1da39-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="1da39-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="1da39-140">See also</span></span>

- [<span data-ttu-id="1da39-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1da39-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="1da39-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1da39-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="1da39-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1da39-143">teamsTab</span></span>](../resources/teamstab.md)


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

