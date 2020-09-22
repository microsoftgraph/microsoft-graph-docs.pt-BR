---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a10872d45a53c60af75179acfd2e1ece793b7c4a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036923"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="75782-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="75782-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="75782-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75782-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75782-105">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="75782-105">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="75782-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe à qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="75782-106">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="75782-107">Methods</span><span class="sxs-lookup"><span data-stu-id="75782-107">Methods</span></span>

| <span data-ttu-id="75782-108">Método</span><span class="sxs-lookup"><span data-stu-id="75782-108">Method</span></span>       | <span data-ttu-id="75782-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="75782-109">Return Type</span></span>  |<span data-ttu-id="75782-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="75782-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75782-111">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="75782-111">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="75782-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="75782-112">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="75782-113">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="75782-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="75782-114">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="75782-114">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="75782-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="75782-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="75782-116">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="75782-116">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="75782-117">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="75782-117">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="75782-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75782-118">None</span></span> | <span data-ttu-id="75782-119">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="75782-119">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="75782-120">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="75782-120">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="75782-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75782-121">None</span></span> | <span data-ttu-id="75782-122">Atualiza para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75782-122">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="75782-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75782-123">Properties</span></span>

| <span data-ttu-id="75782-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75782-124">Property</span></span>            | <span data-ttu-id="75782-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="75782-125">Type</span></span>     | <span data-ttu-id="75782-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="75782-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="75782-127">id</span><span class="sxs-lookup"><span data-stu-id="75782-127">id</span></span>                  | <span data-ttu-id="75782-128">string</span><span class="sxs-lookup"><span data-stu-id="75782-128">string</span></span>   | <span data-ttu-id="75782-129">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="75782-129">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="75782-130">Relações</span><span class="sxs-lookup"><span data-stu-id="75782-130">Relationships</span></span>

| <span data-ttu-id="75782-131">Relação</span><span class="sxs-lookup"><span data-stu-id="75782-131">Relationship</span></span>   | <span data-ttu-id="75782-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="75782-132">Type</span></span>    | <span data-ttu-id="75782-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="75782-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="75782-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="75782-134">teamsApp</span></span>|[<span data-ttu-id="75782-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="75782-135">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="75782-136">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="75782-136">The app that is installed.</span></span> |
|<span data-ttu-id="75782-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="75782-137">teamsAppDefinition</span></span>|[<span data-ttu-id="75782-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="75782-138">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="75782-139">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75782-139">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="75782-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75782-140">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="75782-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="75782-141">See also</span></span>

- [<span data-ttu-id="75782-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="75782-142">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="75782-143">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="75782-143">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="75782-144">teamsTab</span><span class="sxs-lookup"><span data-stu-id="75782-144">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

