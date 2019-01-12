---
title: tipo de recurso de teamsApp
description: Um aplicativo no catálogo de aplicativos Microsoft Teams.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2493b7f6adee51e5c5622585055cbd3cf2778656
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937443"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="c50ca-103">tipo de recurso de teamsApp</span><span class="sxs-lookup"><span data-stu-id="c50ca-103">teamsApp resource type</span></span>



<span data-ttu-id="c50ca-104">Um aplicativo no catálogo de aplicativos [Equipes da Microsoft](teams-api-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="c50ca-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="c50ca-105">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados em [equipes](team.md) usando o método [Add app à equipe](../api/teamsappinstallation-add.md) .</span><span class="sxs-lookup"><span data-stu-id="c50ca-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="c50ca-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c50ca-106">Methods</span></span>

| <span data-ttu-id="c50ca-107">Método</span><span class="sxs-lookup"><span data-stu-id="c50ca-107">Method</span></span>       | <span data-ttu-id="c50ca-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c50ca-108">Return Type</span></span>  |<span data-ttu-id="c50ca-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c50ca-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c50ca-110">Listar os aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="c50ca-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="c50ca-111">coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="c50ca-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="c50ca-112">Liste aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c50ca-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="c50ca-113">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="c50ca-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="c50ca-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c50ca-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="c50ca-115">Publica um aplicativo no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="c50ca-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="c50ca-116">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="c50ca-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="c50ca-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c50ca-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="c50ca-118">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="c50ca-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="c50ca-119">Remover um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="c50ca-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="c50ca-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c50ca-120">None</span></span> | <span data-ttu-id="c50ca-121">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="c50ca-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="c50ca-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c50ca-122">Properties</span></span>

| <span data-ttu-id="c50ca-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c50ca-123">Property</span></span>            | <span data-ttu-id="c50ca-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c50ca-124">Type</span></span>     | <span data-ttu-id="c50ca-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c50ca-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="c50ca-126">id</span><span class="sxs-lookup"><span data-stu-id="c50ca-126">id</span></span>                  | <span data-ttu-id="c50ca-127">string</span><span class="sxs-lookup"><span data-stu-id="c50ca-127">string</span></span>   | <span data-ttu-id="c50ca-128">O aplicativo de catálogo gerados ID de aplicativo (diferente da identificação de fornecido pelo desenvolvedor no [pacote de aplicativos zip equipes da Microsoft](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="c50ca-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="c50ca-129">externalId</span><span class="sxs-lookup"><span data-stu-id="c50ca-129">externalId</span></span>          | <span data-ttu-id="c50ca-130">string</span><span class="sxs-lookup"><span data-stu-id="c50ca-130">string</span></span>   | <span data-ttu-id="c50ca-131">A identificação do catálogo fornecido pelo desenvolvedor app nas [equipes da Microsoft zip o pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="c50ca-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="c50ca-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c50ca-132">displayName</span></span>                | <span data-ttu-id="c50ca-133">string</span><span class="sxs-lookup"><span data-stu-id="c50ca-133">string</span></span>   | <span data-ttu-id="c50ca-134">O nome do aplicativo catálogo fornecido pelo desenvolvedor app nas [equipes da Microsoft zip o pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="c50ca-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="c50ca-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="c50ca-135">distributionMethod</span></span>  | <span data-ttu-id="c50ca-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="c50ca-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="c50ca-137">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c50ca-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="c50ca-138">valores de teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="c50ca-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="c50ca-139">Membro</span><span class="sxs-lookup"><span data-stu-id="c50ca-139">Member</span></span>|<span data-ttu-id="c50ca-140">Valor</span><span class="sxs-lookup"><span data-stu-id="c50ca-140">Value</span></span>|<span data-ttu-id="c50ca-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="c50ca-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c50ca-142">repositório</span><span class="sxs-lookup"><span data-stu-id="c50ca-142">store</span></span>|<span data-ttu-id="c50ca-143">0</span><span class="sxs-lookup"><span data-stu-id="c50ca-143">0</span></span>| <span data-ttu-id="c50ca-144">O aplicativo está disponível para todos os locatários por meio da loja de app Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c50ca-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="c50ca-145">organization</span><span class="sxs-lookup"><span data-stu-id="c50ca-145">organization</span></span>|<span data-ttu-id="c50ca-146">1</span><span class="sxs-lookup"><span data-stu-id="c50ca-146">1</span></span>|<span data-ttu-id="c50ca-147">O aplicativo está disponível somente neste locatário.</span><span class="sxs-lookup"><span data-stu-id="c50ca-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="c50ca-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="c50ca-148">sideloaded</span></span>|<span data-ttu-id="c50ca-149">2</span><span class="sxs-lookup"><span data-stu-id="c50ca-149">2</span></span>|<span data-ttu-id="c50ca-150">O aplicativo está disponível somente para a equipe do usuário/seu instalados para.</span><span class="sxs-lookup"><span data-stu-id="c50ca-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c50ca-151">Relações</span><span class="sxs-lookup"><span data-stu-id="c50ca-151">Relationships</span></span>

| <span data-ttu-id="c50ca-152">Relação</span><span class="sxs-lookup"><span data-stu-id="c50ca-152">Relationship</span></span> | <span data-ttu-id="c50ca-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="c50ca-153">Type</span></span>   | <span data-ttu-id="c50ca-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="c50ca-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c50ca-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="c50ca-155">appDefinitions</span></span>|<span data-ttu-id="c50ca-156">coleção [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c50ca-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="c50ca-157">Os detalhes de cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c50ca-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c50ca-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c50ca-158">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a><span data-ttu-id="c50ca-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="c50ca-159">See also</span></span>

- [<span data-ttu-id="c50ca-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c50ca-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="c50ca-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c50ca-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="c50ca-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c50ca-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

