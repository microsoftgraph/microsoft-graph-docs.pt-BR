---
title: tipo de recurso de teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: nkramer
ms.openlocfilehash: e845bf10bc5513bc6a5079c295fde2eb6d7b6fa5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312807"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="cbb80-103">tipo de recurso de teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="cbb80-103">teamsAppInstallation resource type</span></span>



<span data-ttu-id="cbb80-104">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="cbb80-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="cbb80-105">Qualquer bots que fazem parte do aplicativo se tornará parte de qualquer aplicativo é adicionado de equipe.</span><span class="sxs-lookup"><span data-stu-id="cbb80-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="cbb80-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cbb80-106">Methods</span></span>

| <span data-ttu-id="cbb80-107">Método</span><span class="sxs-lookup"><span data-stu-id="cbb80-107">Method</span></span>       | <span data-ttu-id="cbb80-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cbb80-108">Return Type</span></span>  |<span data-ttu-id="cbb80-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbb80-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbb80-110">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="cbb80-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="cbb80-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="cbb80-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="cbb80-112">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="cbb80-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="cbb80-113">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbb80-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="cbb80-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="cbb80-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="cbb80-115">Adiciona (instala) um aplicativo para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="cbb80-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="cbb80-116">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbb80-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="cbb80-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cbb80-117">None</span></span> | <span data-ttu-id="cbb80-118">Remove (desinstala) um aplicativo da equipe.</span><span class="sxs-lookup"><span data-stu-id="cbb80-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="cbb80-119">Atualizar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbb80-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="cbb80-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cbb80-120">None</span></span> | <span data-ttu-id="cbb80-121">Atualizações para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cbb80-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="cbb80-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbb80-122">Properties</span></span>

| <span data-ttu-id="cbb80-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbb80-123">Property</span></span>            | <span data-ttu-id="cbb80-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbb80-124">Type</span></span>     | <span data-ttu-id="cbb80-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbb80-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="cbb80-126">id</span><span class="sxs-lookup"><span data-stu-id="cbb80-126">id</span></span>                  | <span data-ttu-id="cbb80-127">string</span><span class="sxs-lookup"><span data-stu-id="cbb80-127">string</span></span>   | <span data-ttu-id="cbb80-128">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="cbb80-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="cbb80-129">Relações</span><span class="sxs-lookup"><span data-stu-id="cbb80-129">Relationships</span></span>

| <span data-ttu-id="cbb80-130">Relação</span><span class="sxs-lookup"><span data-stu-id="cbb80-130">Relationship</span></span>   | <span data-ttu-id="cbb80-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbb80-131">Type</span></span>    | <span data-ttu-id="cbb80-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbb80-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cbb80-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cbb80-133">teamsApp</span></span>|[<span data-ttu-id="cbb80-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cbb80-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="cbb80-135">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="cbb80-135">The app that is installed.</span></span> |
|<span data-ttu-id="cbb80-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="cbb80-136">teamsAppDefinition</span></span>|[<span data-ttu-id="cbb80-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="cbb80-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="cbb80-138">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cbb80-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cbb80-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbb80-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="cbb80-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="cbb80-140">See also</span></span>

- [<span data-ttu-id="cbb80-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cbb80-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="cbb80-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="cbb80-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="cbb80-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cbb80-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

