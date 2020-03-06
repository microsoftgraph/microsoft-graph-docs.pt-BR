---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 70dfe86840bd908a2e626b7f965d89251b9221aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533501"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="d88a7-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d88a7-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="d88a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d88a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d88a7-105">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="d88a7-105">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="d88a7-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe à qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="d88a7-106">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="d88a7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d88a7-107">Methods</span></span>

| <span data-ttu-id="d88a7-108">Método</span><span class="sxs-lookup"><span data-stu-id="d88a7-108">Method</span></span>       | <span data-ttu-id="d88a7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d88a7-109">Return Type</span></span>  |<span data-ttu-id="d88a7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d88a7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d88a7-111">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="d88a7-111">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="d88a7-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d88a7-112">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="d88a7-113">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d88a7-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="d88a7-114">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="d88a7-114">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="d88a7-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d88a7-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="d88a7-116">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d88a7-116">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="d88a7-117">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="d88a7-117">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="d88a7-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d88a7-118">None</span></span> | <span data-ttu-id="d88a7-119">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d88a7-119">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="d88a7-120">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="d88a7-120">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="d88a7-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d88a7-121">None</span></span> | <span data-ttu-id="d88a7-122">Atualiza para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d88a7-122">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="d88a7-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d88a7-123">Properties</span></span>

| <span data-ttu-id="d88a7-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d88a7-124">Property</span></span>            | <span data-ttu-id="d88a7-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="d88a7-125">Type</span></span>     | <span data-ttu-id="d88a7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d88a7-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d88a7-127">id</span><span class="sxs-lookup"><span data-stu-id="d88a7-127">id</span></span>                  | <span data-ttu-id="d88a7-128">string</span><span class="sxs-lookup"><span data-stu-id="d88a7-128">string</span></span>   | <span data-ttu-id="d88a7-129">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="d88a7-129">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="d88a7-130">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="d88a7-130">Relationships</span></span>

| <span data-ttu-id="d88a7-131">Relação</span><span class="sxs-lookup"><span data-stu-id="d88a7-131">Relationship</span></span>   | <span data-ttu-id="d88a7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d88a7-132">Type</span></span>    | <span data-ttu-id="d88a7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d88a7-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d88a7-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d88a7-134">teamsApp</span></span>|[<span data-ttu-id="d88a7-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d88a7-135">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="d88a7-136">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="d88a7-136">The app that is installed.</span></span> |
|<span data-ttu-id="d88a7-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d88a7-137">teamsAppDefinition</span></span>|[<span data-ttu-id="d88a7-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d88a7-138">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="d88a7-139">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d88a7-139">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d88a7-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d88a7-140">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="d88a7-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="d88a7-141">See also</span></span>

- [<span data-ttu-id="d88a7-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d88a7-142">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="d88a7-143">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d88a7-143">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="d88a7-144">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d88a7-144">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
