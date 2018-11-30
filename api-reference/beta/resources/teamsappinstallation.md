---
title: tipo de recurso de teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
ms.openlocfilehash: 64573e163c0ec5ce9f3282e747dffd4ccc6718de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036143"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="bc9dc-103">tipo de recurso de teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="bc9dc-103">teamsAppInstallation resource type</span></span>

> <span data-ttu-id="bc9dc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bc9dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc9dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bc9dc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc9dc-106">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="bc9dc-106">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="bc9dc-107">Qualquer bots que fazem parte do aplicativo se tornará parte de qualquer aplicativo é adicionado de equipe.</span><span class="sxs-lookup"><span data-stu-id="bc9dc-107">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="bc9dc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="bc9dc-108">Methods</span></span>

| <span data-ttu-id="bc9dc-109">Método</span><span class="sxs-lookup"><span data-stu-id="bc9dc-109">Method</span></span>       | <span data-ttu-id="bc9dc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bc9dc-110">Return Type</span></span>  |<span data-ttu-id="bc9dc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc9dc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bc9dc-112">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="bc9dc-112">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="bc9dc-113">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="bc9dc-113">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="bc9dc-114">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="bc9dc-114">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="bc9dc-115">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc9dc-115">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="bc9dc-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="bc9dc-116">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="bc9dc-117">Adiciona (instala) um aplicativo para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="bc9dc-117">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="bc9dc-118">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc9dc-118">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="bc9dc-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc9dc-119">None</span></span> | <span data-ttu-id="bc9dc-120">Remove (desinstala) um aplicativo da equipe.</span><span class="sxs-lookup"><span data-stu-id="bc9dc-120">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="bc9dc-121">Atualizar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc9dc-121">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="bc9dc-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc9dc-122">None</span></span> | <span data-ttu-id="bc9dc-123">Atualizações para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bc9dc-123">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc9dc-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc9dc-124">Properties</span></span>

| <span data-ttu-id="bc9dc-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc9dc-125">Property</span></span>            | <span data-ttu-id="bc9dc-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc9dc-126">Type</span></span>     | <span data-ttu-id="bc9dc-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc9dc-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="bc9dc-128">id</span><span class="sxs-lookup"><span data-stu-id="bc9dc-128">id</span></span>                  | <span data-ttu-id="bc9dc-129">string</span><span class="sxs-lookup"><span data-stu-id="bc9dc-129">string</span></span>   | <span data-ttu-id="bc9dc-130">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="bc9dc-130">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="bc9dc-131">Relações</span><span class="sxs-lookup"><span data-stu-id="bc9dc-131">Relationships</span></span>

| <span data-ttu-id="bc9dc-132">Relação</span><span class="sxs-lookup"><span data-stu-id="bc9dc-132">Relationship</span></span>   | <span data-ttu-id="bc9dc-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc9dc-133">Type</span></span>    | <span data-ttu-id="bc9dc-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc9dc-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bc9dc-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="bc9dc-135">teamsApp</span></span>|[<span data-ttu-id="bc9dc-136">teamsApp</span><span class="sxs-lookup"><span data-stu-id="bc9dc-136">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="bc9dc-137">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="bc9dc-137">The app that is installed.</span></span> |
|<span data-ttu-id="bc9dc-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="bc9dc-138">teamsAppDefinition</span></span>|[<span data-ttu-id="bc9dc-139">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="bc9dc-139">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="bc9dc-140">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bc9dc-140">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bc9dc-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc9dc-141">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="bc9dc-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="bc9dc-142">See also</span></span>

- [<span data-ttu-id="bc9dc-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="bc9dc-143">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="bc9dc-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="bc9dc-144">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="bc9dc-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bc9dc-145">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

