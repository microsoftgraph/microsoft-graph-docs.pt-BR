---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b180cae4c700eea31a5d5d9b1504f09ca12c3ae0
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908345"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="862b5-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="862b5-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="862b5-104">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="862b5-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="862b5-105">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe à qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="862b5-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="862b5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="862b5-106">Methods</span></span>

| <span data-ttu-id="862b5-107">Método</span><span class="sxs-lookup"><span data-stu-id="862b5-107">Method</span></span>       | <span data-ttu-id="862b5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="862b5-108">Return Type</span></span>  |<span data-ttu-id="862b5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="862b5-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="862b5-110">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="862b5-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="862b5-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="862b5-111">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="862b5-112">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="862b5-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="862b5-113">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="862b5-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="862b5-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="862b5-114">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="862b5-115">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="862b5-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="862b5-116">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="862b5-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="862b5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="862b5-117">None</span></span> | <span data-ttu-id="862b5-118">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="862b5-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="862b5-119">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="862b5-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="862b5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="862b5-120">None</span></span> | <span data-ttu-id="862b5-121">Atualiza para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="862b5-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="862b5-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="862b5-122">Properties</span></span>

| <span data-ttu-id="862b5-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="862b5-123">Property</span></span>            | <span data-ttu-id="862b5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="862b5-124">Type</span></span>     | <span data-ttu-id="862b5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="862b5-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="862b5-126">id</span><span class="sxs-lookup"><span data-stu-id="862b5-126">id</span></span>                  | <span data-ttu-id="862b5-127">string</span><span class="sxs-lookup"><span data-stu-id="862b5-127">string</span></span>   | <span data-ttu-id="862b5-128">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="862b5-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="862b5-129">Relações</span><span class="sxs-lookup"><span data-stu-id="862b5-129">Relationships</span></span>

| <span data-ttu-id="862b5-130">Relação</span><span class="sxs-lookup"><span data-stu-id="862b5-130">Relationship</span></span>   | <span data-ttu-id="862b5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="862b5-131">Type</span></span>    | <span data-ttu-id="862b5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="862b5-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="862b5-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="862b5-133">teamsApp</span></span>|[<span data-ttu-id="862b5-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="862b5-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="862b5-135">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="862b5-135">The app that is installed.</span></span> |
|<span data-ttu-id="862b5-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="862b5-136">teamsAppDefinition</span></span>|[<span data-ttu-id="862b5-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="862b5-137">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="862b5-138">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="862b5-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="862b5-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="862b5-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a><span data-ttu-id="862b5-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="862b5-140">See also</span></span>

- [<span data-ttu-id="862b5-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="862b5-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="862b5-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="862b5-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="862b5-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="862b5-143">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
