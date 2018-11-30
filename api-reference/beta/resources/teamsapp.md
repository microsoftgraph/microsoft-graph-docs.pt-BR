---
title: tipo de recurso de teamsApp
description: Um aplicativo no catálogo de aplicativos Microsoft Teams.
ms.openlocfilehash: bb9081306cbcc5d8537c86e7f3f59afff89a03b0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036145"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="a2352-103">tipo de recurso de teamsApp</span><span class="sxs-lookup"><span data-stu-id="a2352-103">teamsApp resource type</span></span>

> <span data-ttu-id="a2352-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a2352-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2352-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a2352-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2352-106">Um aplicativo no catálogo de aplicativos [Equipes da Microsoft](teams-api-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="a2352-106">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="a2352-107">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados em [equipes](team.md) usando o método [Add app à equipe](../api/teamsappinstallation-add.md) .</span><span class="sxs-lookup"><span data-stu-id="a2352-107">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="a2352-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a2352-108">Methods</span></span>

| <span data-ttu-id="a2352-109">Método</span><span class="sxs-lookup"><span data-stu-id="a2352-109">Method</span></span>       | <span data-ttu-id="a2352-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a2352-110">Return Type</span></span>  |<span data-ttu-id="a2352-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2352-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2352-112">Listar os aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="a2352-112">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="a2352-113">coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="a2352-113">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="a2352-114">Liste aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a2352-114">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="a2352-115">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2352-115">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="a2352-116">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a2352-116">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="a2352-117">Publica um aplicativo no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="a2352-117">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="a2352-118">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="a2352-118">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="a2352-119">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a2352-119">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="a2352-120">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="a2352-120">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="a2352-121">Remover um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="a2352-121">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="a2352-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2352-122">None</span></span> | <span data-ttu-id="a2352-123">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="a2352-123">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2352-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2352-124">Properties</span></span>

| <span data-ttu-id="a2352-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2352-125">Property</span></span>            | <span data-ttu-id="a2352-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2352-126">Type</span></span>     | <span data-ttu-id="a2352-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2352-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="a2352-128">id</span><span class="sxs-lookup"><span data-stu-id="a2352-128">id</span></span>                  | <span data-ttu-id="a2352-129">string</span><span class="sxs-lookup"><span data-stu-id="a2352-129">string</span></span>   | <span data-ttu-id="a2352-130">O aplicativo de catálogo gerados ID de aplicativo (diferente da identificação de fornecido pelo desenvolvedor no [pacote de aplicativos zip equipes da Microsoft](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="a2352-130">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="a2352-131">externalId</span><span class="sxs-lookup"><span data-stu-id="a2352-131">externalId</span></span>          | <span data-ttu-id="a2352-132">string</span><span class="sxs-lookup"><span data-stu-id="a2352-132">string</span></span>   | <span data-ttu-id="a2352-133">A identificação do catálogo fornecido pelo desenvolvedor app nas [equipes da Microsoft zip o pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="a2352-133">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="a2352-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a2352-134">displayName</span></span>                | <span data-ttu-id="a2352-135">string</span><span class="sxs-lookup"><span data-stu-id="a2352-135">string</span></span>   | <span data-ttu-id="a2352-136">O nome do aplicativo catálogo fornecido pelo desenvolvedor app nas [equipes da Microsoft zip o pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="a2352-136">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="a2352-137">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="a2352-137">distributionMethod</span></span>  | <span data-ttu-id="a2352-138">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="a2352-138">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="a2352-139">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a2352-139">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="a2352-140">valores de teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="a2352-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="a2352-141">Membro</span><span class="sxs-lookup"><span data-stu-id="a2352-141">Member</span></span>|<span data-ttu-id="a2352-142">Valor</span><span class="sxs-lookup"><span data-stu-id="a2352-142">Value</span></span>|<span data-ttu-id="a2352-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2352-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2352-144">repositório</span><span class="sxs-lookup"><span data-stu-id="a2352-144">store</span></span>|<span data-ttu-id="a2352-145">0</span><span class="sxs-lookup"><span data-stu-id="a2352-145">0</span></span>| <span data-ttu-id="a2352-146">O aplicativo está disponível para todos os locatários por meio da loja de app Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a2352-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="a2352-147">organization</span><span class="sxs-lookup"><span data-stu-id="a2352-147">organization</span></span>|<span data-ttu-id="a2352-148">1</span><span class="sxs-lookup"><span data-stu-id="a2352-148">1</span></span>|<span data-ttu-id="a2352-149">O aplicativo está disponível somente neste locatário.</span><span class="sxs-lookup"><span data-stu-id="a2352-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="a2352-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="a2352-150">sideloaded</span></span>|<span data-ttu-id="a2352-151">2</span><span class="sxs-lookup"><span data-stu-id="a2352-151">2</span></span>|<span data-ttu-id="a2352-152">O aplicativo está disponível somente para a equipe do usuário/seu instalados para.</span><span class="sxs-lookup"><span data-stu-id="a2352-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2352-153">Relações</span><span class="sxs-lookup"><span data-stu-id="a2352-153">Relationships</span></span>

| <span data-ttu-id="a2352-154">Relação</span><span class="sxs-lookup"><span data-stu-id="a2352-154">Relationship</span></span> | <span data-ttu-id="a2352-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2352-155">Type</span></span>   | <span data-ttu-id="a2352-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2352-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a2352-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="a2352-157">appDefinitions</span></span>|<span data-ttu-id="a2352-158">coleção [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a2352-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="a2352-159">Os detalhes de cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a2352-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a2352-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2352-160">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="a2352-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="a2352-161">See also</span></span>

- [<span data-ttu-id="a2352-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a2352-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="a2352-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a2352-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="a2352-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a2352-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

