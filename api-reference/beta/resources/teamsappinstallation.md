---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8d8770a21b11c9ba1042c9a0f59d9405dce96f9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345798"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="f46bf-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f46bf-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f46bf-104">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="f46bf-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="f46bf-105">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe à qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="f46bf-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="f46bf-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f46bf-106">Methods</span></span>

| <span data-ttu-id="f46bf-107">Método</span><span class="sxs-lookup"><span data-stu-id="f46bf-107">Method</span></span>       | <span data-ttu-id="f46bf-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f46bf-108">Return Type</span></span>  |<span data-ttu-id="f46bf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f46bf-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f46bf-110">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="f46bf-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="f46bf-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f46bf-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="f46bf-112">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="f46bf-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="f46bf-113">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="f46bf-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="f46bf-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f46bf-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="f46bf-115">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="f46bf-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="f46bf-116">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="f46bf-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="f46bf-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f46bf-117">None</span></span> | <span data-ttu-id="f46bf-118">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="f46bf-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="f46bf-119">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="f46bf-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="f46bf-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f46bf-120">None</span></span> | <span data-ttu-id="f46bf-121">Atualiza para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f46bf-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="f46bf-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f46bf-122">Properties</span></span>

| <span data-ttu-id="f46bf-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f46bf-123">Property</span></span>            | <span data-ttu-id="f46bf-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f46bf-124">Type</span></span>     | <span data-ttu-id="f46bf-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f46bf-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="f46bf-126">id</span><span class="sxs-lookup"><span data-stu-id="f46bf-126">id</span></span>                  | <span data-ttu-id="f46bf-127">string</span><span class="sxs-lookup"><span data-stu-id="f46bf-127">string</span></span>   | <span data-ttu-id="f46bf-128">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="f46bf-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="f46bf-129">Relações</span><span class="sxs-lookup"><span data-stu-id="f46bf-129">Relationships</span></span>

| <span data-ttu-id="f46bf-130">Relação</span><span class="sxs-lookup"><span data-stu-id="f46bf-130">Relationship</span></span>   | <span data-ttu-id="f46bf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f46bf-131">Type</span></span>    | <span data-ttu-id="f46bf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f46bf-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f46bf-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f46bf-133">teamsApp</span></span>|[<span data-ttu-id="f46bf-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f46bf-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="f46bf-135">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="f46bf-135">The app that is installed.</span></span> |
|<span data-ttu-id="f46bf-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="f46bf-136">teamsAppDefinition</span></span>|[<span data-ttu-id="f46bf-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="f46bf-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="f46bf-138">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f46bf-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f46bf-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f46bf-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="f46bf-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="f46bf-140">See also</span></span>

- [<span data-ttu-id="f46bf-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f46bf-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="f46bf-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="f46bf-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="f46bf-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f46bf-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

