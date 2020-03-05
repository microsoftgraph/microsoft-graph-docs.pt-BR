---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f4f13bf13b34c41c7c15c3356cc67636e6f441c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519922"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="03b02-103">tipo de recurso teamsApp</span><span class="sxs-lookup"><span data-stu-id="03b02-103">teamsApp resource type</span></span>

<span data-ttu-id="03b02-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="03b02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03b02-105">Um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="03b02-105">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="03b02-106">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="03b02-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="03b02-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="03b02-107">Methods</span></span>

| <span data-ttu-id="03b02-108">Método</span><span class="sxs-lookup"><span data-stu-id="03b02-108">Method</span></span>       | <span data-ttu-id="03b02-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03b02-109">Return Type</span></span>  |<span data-ttu-id="03b02-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="03b02-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03b02-111">Lista de aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="03b02-111">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="03b02-112">Coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="03b02-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="03b02-113">Lista de aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="03b02-113">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="03b02-114">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="03b02-114">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="03b02-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="03b02-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="03b02-116">Publica um aplicativo ao catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="03b02-116">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="03b02-117">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="03b02-117">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="03b02-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="03b02-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="03b02-119">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="03b02-119">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="03b02-120">Remover um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="03b02-120">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="03b02-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03b02-121">None</span></span> | <span data-ttu-id="03b02-122">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="03b02-122">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="03b02-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03b02-123">Properties</span></span>

| <span data-ttu-id="03b02-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03b02-124">Property</span></span>            | <span data-ttu-id="03b02-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="03b02-125">Type</span></span>     | <span data-ttu-id="03b02-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="03b02-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="03b02-127">id</span><span class="sxs-lookup"><span data-stu-id="03b02-127">id</span></span>                  | <span data-ttu-id="03b02-128">string</span><span class="sxs-lookup"><span data-stu-id="03b02-128">string</span></span>   | <span data-ttu-id="03b02-129">A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="03b02-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="03b02-130">externalId</span><span class="sxs-lookup"><span data-stu-id="03b02-130">externalId</span></span>          | <span data-ttu-id="03b02-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03b02-131">string</span></span>   | <span data-ttu-id="03b02-132">A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="03b02-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="03b02-133">displayName</span><span class="sxs-lookup"><span data-stu-id="03b02-133">displayName</span></span>                | <span data-ttu-id="03b02-134">string</span><span class="sxs-lookup"><span data-stu-id="03b02-134">string</span></span>   | <span data-ttu-id="03b02-135">O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="03b02-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="03b02-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="03b02-136">distributionMethod</span></span>  | <span data-ttu-id="03b02-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="03b02-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="03b02-138">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="03b02-138">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="03b02-139">valores teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="03b02-139">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="03b02-140">Membro</span><span class="sxs-lookup"><span data-stu-id="03b02-140">Member</span></span>|<span data-ttu-id="03b02-141">Valor</span><span class="sxs-lookup"><span data-stu-id="03b02-141">Value</span></span>|<span data-ttu-id="03b02-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="03b02-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03b02-143">loja</span><span class="sxs-lookup"><span data-stu-id="03b02-143">store</span></span>|<span data-ttu-id="03b02-144">,0</span><span class="sxs-lookup"><span data-stu-id="03b02-144">0</span></span>| <span data-ttu-id="03b02-145">O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="03b02-145">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="03b02-146">organização</span><span class="sxs-lookup"><span data-stu-id="03b02-146">organization</span></span>|<span data-ttu-id="03b02-147">1 </span><span class="sxs-lookup"><span data-stu-id="03b02-147">1</span></span>|<span data-ttu-id="03b02-148">O aplicativo está disponível somente nesse locatário.</span><span class="sxs-lookup"><span data-stu-id="03b02-148">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="03b02-149">sideloaded</span><span class="sxs-lookup"><span data-stu-id="03b02-149">sideloaded</span></span>|<span data-ttu-id="03b02-150">2 </span><span class="sxs-lookup"><span data-stu-id="03b02-150">2</span></span>|<span data-ttu-id="03b02-151">O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="03b02-151">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03b02-152">Relações</span><span class="sxs-lookup"><span data-stu-id="03b02-152">Relationships</span></span>

| <span data-ttu-id="03b02-153">Relação</span><span class="sxs-lookup"><span data-stu-id="03b02-153">Relationship</span></span> | <span data-ttu-id="03b02-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="03b02-154">Type</span></span>   | <span data-ttu-id="03b02-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="03b02-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="03b02-156">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="03b02-156">appDefinitions</span></span>|<span data-ttu-id="03b02-157">Coleção [teamsAppDefinition](teamsappdefinition.md) </span><span class="sxs-lookup"><span data-stu-id="03b02-157">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="03b02-158">Os detalhes para cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="03b02-158">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03b02-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03b02-159">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="03b02-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="03b02-160">See also</span></span>

- [<span data-ttu-id="03b02-161">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="03b02-161">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="03b02-162">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="03b02-162">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="03b02-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="03b02-163">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

