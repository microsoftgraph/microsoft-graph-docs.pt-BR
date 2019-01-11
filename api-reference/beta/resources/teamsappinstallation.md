---
title: tipo de recurso de teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 5eca63cb3385fa03f8dffadff0482dc79a1dcfe3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871509"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="8d72b-103">tipo de recurso de teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8d72b-103">teamsAppInstallation resource type</span></span>

> <span data-ttu-id="8d72b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8d72b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d72b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8d72b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d72b-106">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="8d72b-106">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="8d72b-107">Qualquer bots que fazem parte do aplicativo se tornará parte de qualquer aplicativo é adicionado de equipe.</span><span class="sxs-lookup"><span data-stu-id="8d72b-107">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="8d72b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8d72b-108">Methods</span></span>

| <span data-ttu-id="8d72b-109">Método</span><span class="sxs-lookup"><span data-stu-id="8d72b-109">Method</span></span>       | <span data-ttu-id="8d72b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8d72b-110">Return Type</span></span>  |<span data-ttu-id="8d72b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d72b-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d72b-112">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="8d72b-112">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="8d72b-113">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8d72b-113">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="8d72b-114">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="8d72b-114">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="8d72b-115">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d72b-115">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="8d72b-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8d72b-116">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="8d72b-117">Adiciona (instala) um aplicativo para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="8d72b-117">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="8d72b-118">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d72b-118">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="8d72b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d72b-119">None</span></span> | <span data-ttu-id="8d72b-120">Remove (desinstala) um aplicativo da equipe.</span><span class="sxs-lookup"><span data-stu-id="8d72b-120">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="8d72b-121">Atualizar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d72b-121">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="8d72b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d72b-122">None</span></span> | <span data-ttu-id="8d72b-123">Atualizações para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8d72b-123">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d72b-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d72b-124">Properties</span></span>

| <span data-ttu-id="8d72b-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d72b-125">Property</span></span>            | <span data-ttu-id="8d72b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d72b-126">Type</span></span>     | <span data-ttu-id="8d72b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d72b-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="8d72b-128">id</span><span class="sxs-lookup"><span data-stu-id="8d72b-128">id</span></span>                  | <span data-ttu-id="8d72b-129">string</span><span class="sxs-lookup"><span data-stu-id="8d72b-129">string</span></span>   | <span data-ttu-id="8d72b-130">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="8d72b-130">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="8d72b-131">Relações</span><span class="sxs-lookup"><span data-stu-id="8d72b-131">Relationships</span></span>

| <span data-ttu-id="8d72b-132">Relação</span><span class="sxs-lookup"><span data-stu-id="8d72b-132">Relationship</span></span>   | <span data-ttu-id="8d72b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d72b-133">Type</span></span>    | <span data-ttu-id="8d72b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d72b-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8d72b-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8d72b-135">teamsApp</span></span>|[<span data-ttu-id="8d72b-136">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8d72b-136">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="8d72b-137">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="8d72b-137">The app that is installed.</span></span> |
|<span data-ttu-id="8d72b-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8d72b-138">teamsAppDefinition</span></span>|[<span data-ttu-id="8d72b-139">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8d72b-139">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="8d72b-140">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8d72b-140">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d72b-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d72b-141">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="8d72b-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="8d72b-142">See also</span></span>

- [<span data-ttu-id="8d72b-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8d72b-143">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="8d72b-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8d72b-144">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="8d72b-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8d72b-145">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

