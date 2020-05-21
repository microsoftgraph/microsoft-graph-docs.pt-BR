---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1e3ed231c6bd741afe3dcd502d517006c402fc77
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335331"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="cd234-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="cd234-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="cd234-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd234-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd234-105">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="cd234-105">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="cd234-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe à qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="cd234-106">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="cd234-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="cd234-107">Methods</span></span>

| <span data-ttu-id="cd234-108">Método</span><span class="sxs-lookup"><span data-stu-id="cd234-108">Method</span></span>       | <span data-ttu-id="cd234-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cd234-109">Return Type</span></span>  |<span data-ttu-id="cd234-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd234-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd234-111">Listar aplicativos</span><span class="sxs-lookup"><span data-stu-id="cd234-111">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="cd234-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="cd234-112">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="cd234-113">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="cd234-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="cd234-114">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd234-114">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="cd234-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="cd234-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="cd234-116">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="cd234-116">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="cd234-117">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd234-117">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="cd234-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd234-118">None</span></span> | <span data-ttu-id="cd234-119">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="cd234-119">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="cd234-120">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd234-120">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="cd234-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd234-121">None</span></span> | <span data-ttu-id="cd234-122">Atualiza para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd234-122">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd234-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd234-123">Properties</span></span>

| <span data-ttu-id="cd234-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd234-124">Property</span></span>            | <span data-ttu-id="cd234-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd234-125">Type</span></span>     | <span data-ttu-id="cd234-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd234-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="cd234-127">id</span><span class="sxs-lookup"><span data-stu-id="cd234-127">id</span></span>                  | <span data-ttu-id="cd234-128">string</span><span class="sxs-lookup"><span data-stu-id="cd234-128">string</span></span>   | <span data-ttu-id="cd234-129">Uma ID exclusiva (não a AppID do Teams).</span><span class="sxs-lookup"><span data-stu-id="cd234-129">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="cd234-130">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="cd234-130">Relationships</span></span>

| <span data-ttu-id="cd234-131">Relação</span><span class="sxs-lookup"><span data-stu-id="cd234-131">Relationship</span></span>   | <span data-ttu-id="cd234-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd234-132">Type</span></span>    | <span data-ttu-id="cd234-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd234-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cd234-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cd234-134">teamsApp</span></span>|[<span data-ttu-id="cd234-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cd234-135">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="cd234-136">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="cd234-136">The app that is installed.</span></span> |
|<span data-ttu-id="cd234-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="cd234-137">teamsAppDefinition</span></span>|[<span data-ttu-id="cd234-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="cd234-138">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="cd234-139">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cd234-139">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cd234-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd234-140">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="cd234-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="cd234-141">See also</span></span>

- [<span data-ttu-id="cd234-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cd234-142">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="cd234-143">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="cd234-143">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="cd234-144">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cd234-144">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
