---
title: tipo de recurso de teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 153b131cd24709995d7215b1cf568a8565f42a80
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929477"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="2c1fd-103">tipo de recurso de teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2c1fd-103">teamsAppInstallation resource type</span></span>



<span data-ttu-id="2c1fd-104">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="2c1fd-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="2c1fd-105">Qualquer bots que fazem parte do aplicativo se tornará parte de qualquer aplicativo é adicionado de equipe.</span><span class="sxs-lookup"><span data-stu-id="2c1fd-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="2c1fd-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2c1fd-106">Methods</span></span>

| <span data-ttu-id="2c1fd-107">Método</span><span class="sxs-lookup"><span data-stu-id="2c1fd-107">Method</span></span>       | <span data-ttu-id="2c1fd-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2c1fd-108">Return Type</span></span>  |<span data-ttu-id="2c1fd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c1fd-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c1fd-110">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="2c1fd-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="2c1fd-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2c1fd-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="2c1fd-112">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="2c1fd-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="2c1fd-113">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c1fd-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="2c1fd-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2c1fd-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="2c1fd-115">Adiciona (instala) um aplicativo para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="2c1fd-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="2c1fd-116">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c1fd-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="2c1fd-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c1fd-117">None</span></span> | <span data-ttu-id="2c1fd-118">Remove (desinstala) um aplicativo da equipe.</span><span class="sxs-lookup"><span data-stu-id="2c1fd-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="2c1fd-119">Atualizar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c1fd-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="2c1fd-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c1fd-120">None</span></span> | <span data-ttu-id="2c1fd-121">Atualizações para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c1fd-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c1fd-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c1fd-122">Properties</span></span>

| <span data-ttu-id="2c1fd-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c1fd-123">Property</span></span>            | <span data-ttu-id="2c1fd-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c1fd-124">Type</span></span>     | <span data-ttu-id="2c1fd-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c1fd-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="2c1fd-126">id</span><span class="sxs-lookup"><span data-stu-id="2c1fd-126">id</span></span>                  | <span data-ttu-id="2c1fd-127">string</span><span class="sxs-lookup"><span data-stu-id="2c1fd-127">string</span></span>   | <span data-ttu-id="2c1fd-128">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="2c1fd-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="2c1fd-129">Relações</span><span class="sxs-lookup"><span data-stu-id="2c1fd-129">Relationships</span></span>

| <span data-ttu-id="2c1fd-130">Relação</span><span class="sxs-lookup"><span data-stu-id="2c1fd-130">Relationship</span></span>   | <span data-ttu-id="2c1fd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c1fd-131">Type</span></span>    | <span data-ttu-id="2c1fd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c1fd-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2c1fd-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2c1fd-133">teamsApp</span></span>|[<span data-ttu-id="2c1fd-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2c1fd-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="2c1fd-135">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="2c1fd-135">The app that is installed.</span></span> |
|<span data-ttu-id="2c1fd-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2c1fd-136">teamsAppDefinition</span></span>|[<span data-ttu-id="2c1fd-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2c1fd-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="2c1fd-138">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c1fd-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c1fd-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c1fd-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="2c1fd-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="2c1fd-140">See also</span></span>

- [<span data-ttu-id="2c1fd-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2c1fd-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="2c1fd-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2c1fd-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="2c1fd-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2c1fd-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

