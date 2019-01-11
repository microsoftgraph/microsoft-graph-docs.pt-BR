---
title: tipo de recurso de teamsApp
description: Um aplicativo no catálogo de aplicativos Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: b02af5148e40cddd6079de3479767110a9877e4f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841570"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="d9695-103">tipo de recurso de teamsApp</span><span class="sxs-lookup"><span data-stu-id="d9695-103">teamsApp resource type</span></span>

> <span data-ttu-id="d9695-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d9695-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9695-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d9695-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9695-106">Um aplicativo no catálogo de aplicativos [Equipes da Microsoft](teams-api-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="d9695-106">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="d9695-107">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados em [equipes](team.md) usando o método [Add app à equipe](../api/teamsappinstallation-add.md) .</span><span class="sxs-lookup"><span data-stu-id="d9695-107">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="d9695-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d9695-108">Methods</span></span>

| <span data-ttu-id="d9695-109">Método</span><span class="sxs-lookup"><span data-stu-id="d9695-109">Method</span></span>       | <span data-ttu-id="d9695-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d9695-110">Return Type</span></span>  |<span data-ttu-id="d9695-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9695-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d9695-112">Listar os aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="d9695-112">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="d9695-113">coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9695-113">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="d9695-114">Liste aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d9695-114">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="d9695-115">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9695-115">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="d9695-116">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d9695-116">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="d9695-117">Publica um aplicativo no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="d9695-117">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="d9695-118">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="d9695-118">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="d9695-119">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d9695-119">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="d9695-120">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="d9695-120">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="d9695-121">Remover um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="d9695-121">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="d9695-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9695-122">None</span></span> | <span data-ttu-id="d9695-123">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="d9695-123">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9695-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9695-124">Properties</span></span>

| <span data-ttu-id="d9695-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9695-125">Property</span></span>            | <span data-ttu-id="d9695-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9695-126">Type</span></span>     | <span data-ttu-id="d9695-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9695-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d9695-128">id</span><span class="sxs-lookup"><span data-stu-id="d9695-128">id</span></span>                  | <span data-ttu-id="d9695-129">string</span><span class="sxs-lookup"><span data-stu-id="d9695-129">string</span></span>   | <span data-ttu-id="d9695-130">O aplicativo de catálogo gerados ID de aplicativo (diferente da identificação de fornecido pelo desenvolvedor no [pacote de aplicativos zip equipes da Microsoft](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="d9695-130">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d9695-131">externalId</span><span class="sxs-lookup"><span data-stu-id="d9695-131">externalId</span></span>          | <span data-ttu-id="d9695-132">string</span><span class="sxs-lookup"><span data-stu-id="d9695-132">string</span></span>   | <span data-ttu-id="d9695-133">A identificação do catálogo fornecido pelo desenvolvedor app nas [equipes da Microsoft zip o pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="d9695-133">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d9695-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d9695-134">displayName</span></span>                | <span data-ttu-id="d9695-135">string</span><span class="sxs-lookup"><span data-stu-id="d9695-135">string</span></span>   | <span data-ttu-id="d9695-136">O nome do aplicativo catálogo fornecido pelo desenvolvedor app nas [equipes da Microsoft zip o pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="d9695-136">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d9695-137">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="d9695-137">distributionMethod</span></span>  | <span data-ttu-id="d9695-138">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="d9695-138">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="d9695-139">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d9695-139">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="d9695-140">valores de teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="d9695-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="d9695-141">Membro</span><span class="sxs-lookup"><span data-stu-id="d9695-141">Member</span></span>|<span data-ttu-id="d9695-142">Valor</span><span class="sxs-lookup"><span data-stu-id="d9695-142">Value</span></span>|<span data-ttu-id="d9695-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9695-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9695-144">repositório</span><span class="sxs-lookup"><span data-stu-id="d9695-144">store</span></span>|<span data-ttu-id="d9695-145">0</span><span class="sxs-lookup"><span data-stu-id="d9695-145">0</span></span>| <span data-ttu-id="d9695-146">O aplicativo está disponível para todos os locatários por meio da loja de app Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d9695-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="d9695-147">organization</span><span class="sxs-lookup"><span data-stu-id="d9695-147">organization</span></span>|<span data-ttu-id="d9695-148">1</span><span class="sxs-lookup"><span data-stu-id="d9695-148">1</span></span>|<span data-ttu-id="d9695-149">O aplicativo está disponível somente neste locatário.</span><span class="sxs-lookup"><span data-stu-id="d9695-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="d9695-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="d9695-150">sideloaded</span></span>|<span data-ttu-id="d9695-151">2</span><span class="sxs-lookup"><span data-stu-id="d9695-151">2</span></span>|<span data-ttu-id="d9695-152">O aplicativo está disponível somente para a equipe do usuário/seu instalados para.</span><span class="sxs-lookup"><span data-stu-id="d9695-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9695-153">Relações</span><span class="sxs-lookup"><span data-stu-id="d9695-153">Relationships</span></span>

| <span data-ttu-id="d9695-154">Relação</span><span class="sxs-lookup"><span data-stu-id="d9695-154">Relationship</span></span> | <span data-ttu-id="d9695-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9695-155">Type</span></span>   | <span data-ttu-id="d9695-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9695-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d9695-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="d9695-157">appDefinitions</span></span>|<span data-ttu-id="d9695-158">coleção [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d9695-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="d9695-159">Os detalhes de cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d9695-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d9695-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9695-160">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="d9695-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="d9695-161">See also</span></span>

- [<span data-ttu-id="d9695-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d9695-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="d9695-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d9695-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="d9695-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d9695-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

