---
title: tipo de recurso de teamsApp
description: Um aplicativo no catálogo de aplicativos Microsoft Teams.
author: nkramer
ms.openlocfilehash: b0f3bb42bb90c2c3f0211c5a7092fa7fdb9b10b5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305324"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="3bef5-103">tipo de recurso de teamsApp</span><span class="sxs-lookup"><span data-stu-id="3bef5-103">teamsApp resource type</span></span>

> <span data-ttu-id="3bef5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3bef5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bef5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3bef5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3bef5-106">Um aplicativo no catálogo de aplicativos [Equipes da Microsoft](teams-api-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="3bef5-106">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="3bef5-107">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados em [equipes](team.md) usando o método [Add app à equipe](../api/teamsappinstallation-add.md) .</span><span class="sxs-lookup"><span data-stu-id="3bef5-107">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="3bef5-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3bef5-108">Methods</span></span>

| <span data-ttu-id="3bef5-109">Método</span><span class="sxs-lookup"><span data-stu-id="3bef5-109">Method</span></span>       | <span data-ttu-id="3bef5-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3bef5-110">Return Type</span></span>  |<span data-ttu-id="3bef5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bef5-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3bef5-112">Listar os aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="3bef5-112">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="3bef5-113">coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bef5-113">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="3bef5-114">Liste aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3bef5-114">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="3bef5-115">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bef5-115">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="3bef5-116">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3bef5-116">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="3bef5-117">Publica um aplicativo no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="3bef5-117">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="3bef5-118">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="3bef5-118">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="3bef5-119">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3bef5-119">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="3bef5-120">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="3bef5-120">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="3bef5-121">Remover um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="3bef5-121">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="3bef5-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bef5-122">None</span></span> | <span data-ttu-id="3bef5-123">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="3bef5-123">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="3bef5-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bef5-124">Properties</span></span>

| <span data-ttu-id="3bef5-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bef5-125">Property</span></span>            | <span data-ttu-id="3bef5-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bef5-126">Type</span></span>     | <span data-ttu-id="3bef5-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bef5-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="3bef5-128">id</span><span class="sxs-lookup"><span data-stu-id="3bef5-128">id</span></span>                  | <span data-ttu-id="3bef5-129">string</span><span class="sxs-lookup"><span data-stu-id="3bef5-129">string</span></span>   | <span data-ttu-id="3bef5-130">O aplicativo de catálogo gerados ID de aplicativo (diferente da identificação de fornecido pelo desenvolvedor no [pacote de aplicativos zip equipes da Microsoft](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="3bef5-130">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="3bef5-131">externalId</span><span class="sxs-lookup"><span data-stu-id="3bef5-131">externalId</span></span>          | <span data-ttu-id="3bef5-132">string</span><span class="sxs-lookup"><span data-stu-id="3bef5-132">string</span></span>   | <span data-ttu-id="3bef5-133">A identificação do catálogo fornecido pelo desenvolvedor app nas [equipes da Microsoft zip o pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="3bef5-133">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="3bef5-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3bef5-134">displayName</span></span>                | <span data-ttu-id="3bef5-135">string</span><span class="sxs-lookup"><span data-stu-id="3bef5-135">string</span></span>   | <span data-ttu-id="3bef5-136">O nome do aplicativo catálogo fornecido pelo desenvolvedor app nas [equipes da Microsoft zip o pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="3bef5-136">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="3bef5-137">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="3bef5-137">distributionMethod</span></span>  | <span data-ttu-id="3bef5-138">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="3bef5-138">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="3bef5-139">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3bef5-139">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="3bef5-140">valores de teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="3bef5-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="3bef5-141">Member</span><span class="sxs-lookup"><span data-stu-id="3bef5-141">Member</span></span>|<span data-ttu-id="3bef5-142">Valor</span><span class="sxs-lookup"><span data-stu-id="3bef5-142">Value</span></span>|<span data-ttu-id="3bef5-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bef5-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bef5-144">repositório</span><span class="sxs-lookup"><span data-stu-id="3bef5-144">store</span></span>|<span data-ttu-id="3bef5-145">0</span><span class="sxs-lookup"><span data-stu-id="3bef5-145">0</span></span>| <span data-ttu-id="3bef5-146">O aplicativo está disponível para todos os locatários por meio da loja de app Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3bef5-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="3bef5-147">organization</span><span class="sxs-lookup"><span data-stu-id="3bef5-147">organization</span></span>|<span data-ttu-id="3bef5-148">1</span><span class="sxs-lookup"><span data-stu-id="3bef5-148">1</span></span>|<span data-ttu-id="3bef5-149">O aplicativo está disponível somente neste locatário.</span><span class="sxs-lookup"><span data-stu-id="3bef5-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="3bef5-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="3bef5-150">sideloaded</span></span>|<span data-ttu-id="3bef5-151">2</span><span class="sxs-lookup"><span data-stu-id="3bef5-151">2</span></span>|<span data-ttu-id="3bef5-152">O aplicativo está disponível somente para a equipe do usuário/seu instalados para.</span><span class="sxs-lookup"><span data-stu-id="3bef5-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bef5-153">Relações</span><span class="sxs-lookup"><span data-stu-id="3bef5-153">Relationships</span></span>

| <span data-ttu-id="3bef5-154">Relação</span><span class="sxs-lookup"><span data-stu-id="3bef5-154">Relationship</span></span> | <span data-ttu-id="3bef5-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bef5-155">Type</span></span>   | <span data-ttu-id="3bef5-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bef5-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3bef5-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="3bef5-157">appDefinitions</span></span>|<span data-ttu-id="3bef5-158">coleção [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3bef5-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="3bef5-159">Os detalhes de cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3bef5-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3bef5-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bef5-160">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="3bef5-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="3bef5-161">See also</span></span>

- [<span data-ttu-id="3bef5-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="3bef5-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="3bef5-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="3bef5-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="3bef5-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="3bef5-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

