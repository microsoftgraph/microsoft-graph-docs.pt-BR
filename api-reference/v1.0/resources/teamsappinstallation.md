---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1a76d11472b3faef95e87ed4724f1397ebe467a6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033779"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="f273d-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f273d-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="f273d-104">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="f273d-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="f273d-105">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe à qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="f273d-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="f273d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f273d-106">Methods</span></span>

| <span data-ttu-id="f273d-107">Método</span><span class="sxs-lookup"><span data-stu-id="f273d-107">Method</span></span>       | <span data-ttu-id="f273d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f273d-108">Return Type</span></span>  |<span data-ttu-id="f273d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f273d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f273d-110">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="f273d-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="f273d-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f273d-111">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="f273d-112">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="f273d-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="f273d-113">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="f273d-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="f273d-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f273d-114">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="f273d-115">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="f273d-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="f273d-116">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="f273d-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="f273d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f273d-117">None</span></span> | <span data-ttu-id="f273d-118">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="f273d-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="f273d-119">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="f273d-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="f273d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f273d-120">None</span></span> | <span data-ttu-id="f273d-121">Atualiza para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f273d-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="f273d-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f273d-122">Properties</span></span>

| <span data-ttu-id="f273d-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f273d-123">Property</span></span>            | <span data-ttu-id="f273d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f273d-124">Type</span></span>     | <span data-ttu-id="f273d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f273d-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="f273d-126">id</span><span class="sxs-lookup"><span data-stu-id="f273d-126">id</span></span>                  | <span data-ttu-id="f273d-127">string</span><span class="sxs-lookup"><span data-stu-id="f273d-127">string</span></span>   | <span data-ttu-id="f273d-128">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="f273d-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="f273d-129">Relações</span><span class="sxs-lookup"><span data-stu-id="f273d-129">Relationships</span></span>

| <span data-ttu-id="f273d-130">Relação</span><span class="sxs-lookup"><span data-stu-id="f273d-130">Relationship</span></span>   | <span data-ttu-id="f273d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f273d-131">Type</span></span>    | <span data-ttu-id="f273d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f273d-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f273d-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f273d-133">teamsApp</span></span>|[<span data-ttu-id="f273d-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f273d-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="f273d-135">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="f273d-135">The app that is installed.</span></span> |
|<span data-ttu-id="f273d-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="f273d-136">teamsAppDefinition</span></span>|[<span data-ttu-id="f273d-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="f273d-137">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="f273d-138">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f273d-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f273d-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f273d-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="f273d-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="f273d-140">See also</span></span>

- [<span data-ttu-id="f273d-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="f273d-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="f273d-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="f273d-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="f273d-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f273d-143">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
