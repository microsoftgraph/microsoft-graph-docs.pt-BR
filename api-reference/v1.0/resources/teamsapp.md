---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 55fd373fd59f79abdfca8b3e066ca496daf8770b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706000"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="eda89-103">tipo de recurso teamsApp</span><span class="sxs-lookup"><span data-stu-id="eda89-103">teamsApp resource type</span></span>

<span data-ttu-id="eda89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eda89-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eda89-105">Representa um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="eda89-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="eda89-106">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/team-post-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="eda89-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/team-post-installedapps.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="eda89-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="eda89-107">Methods</span></span>

| <span data-ttu-id="eda89-108">Método</span><span class="sxs-lookup"><span data-stu-id="eda89-108">Method</span></span>       | <span data-ttu-id="eda89-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eda89-109">Return Type</span></span>  |<span data-ttu-id="eda89-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eda89-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eda89-111">Listar aplicativos no catálogo</span><span class="sxs-lookup"><span data-stu-id="eda89-111">List apps in catalog</span></span>](../api/appcatalogs-list-teamsapps.md) | <span data-ttu-id="eda89-112">Coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="eda89-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="eda89-113">Liste todos os aplicativos no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="eda89-113">List all the apps in the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="eda89-114">Carregar aplicativo no catálogo</span><span class="sxs-lookup"><span data-stu-id="eda89-114">Upload app to catalog</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="eda89-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="eda89-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="eda89-116">Faça upload de um aplicativo para o catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="eda89-116">Upload an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="eda89-117">Atualizar aplicativo no catálogo</span><span class="sxs-lookup"><span data-stu-id="eda89-117">Update app in catalog</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="eda89-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="eda89-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="eda89-119">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="eda89-119">Update an app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="eda89-120">Remover aplicativo do catálogo</span><span class="sxs-lookup"><span data-stu-id="eda89-120">Delete app from catalog</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="eda89-121">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="eda89-121">None</span></span> | <span data-ttu-id="eda89-122">Remova um aplicativo do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="eda89-122">Remove an app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="eda89-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eda89-123">Properties</span></span>

| <span data-ttu-id="eda89-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eda89-124">Property</span></span>            | <span data-ttu-id="eda89-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="eda89-125">Type</span></span>     | <span data-ttu-id="eda89-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="eda89-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="eda89-127">id</span><span class="sxs-lookup"><span data-stu-id="eda89-127">id</span></span>                  | <span data-ttu-id="eda89-128">string</span><span class="sxs-lookup"><span data-stu-id="eda89-128">string</span></span>   | <span data-ttu-id="eda89-129">A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="eda89-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="eda89-130">externalId</span><span class="sxs-lookup"><span data-stu-id="eda89-130">externalId</span></span>          | <span data-ttu-id="eda89-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eda89-131">string</span></span>   | <span data-ttu-id="eda89-132">A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="eda89-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="eda89-133">displayName</span><span class="sxs-lookup"><span data-stu-id="eda89-133">displayName</span></span>                | <span data-ttu-id="eda89-134">string</span><span class="sxs-lookup"><span data-stu-id="eda89-134">string</span></span>   | <span data-ttu-id="eda89-135">O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="eda89-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="eda89-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="eda89-136">distributionMethod</span></span>  | <span data-ttu-id="eda89-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="eda89-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="eda89-138">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eda89-138">The method of distribution for the app.</span></span> <span data-ttu-id="eda89-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eda89-139">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="eda89-140">valores teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="eda89-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="eda89-141">Membro</span><span class="sxs-lookup"><span data-stu-id="eda89-141">Member</span></span>|<span data-ttu-id="eda89-142">Valor</span><span class="sxs-lookup"><span data-stu-id="eda89-142">Value</span></span>|<span data-ttu-id="eda89-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="eda89-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eda89-144">loja</span><span class="sxs-lookup"><span data-stu-id="eda89-144">store</span></span>|<span data-ttu-id="eda89-145">0</span><span class="sxs-lookup"><span data-stu-id="eda89-145">0</span></span>| <span data-ttu-id="eda89-146">O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="eda89-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="eda89-147">organização</span><span class="sxs-lookup"><span data-stu-id="eda89-147">organization</span></span>|<span data-ttu-id="eda89-148">1</span><span class="sxs-lookup"><span data-stu-id="eda89-148">1</span></span>|<span data-ttu-id="eda89-149">O aplicativo está disponível somente nesse locatário.</span><span class="sxs-lookup"><span data-stu-id="eda89-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="eda89-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="eda89-150">sideloaded</span></span>|<span data-ttu-id="eda89-151">2</span><span class="sxs-lookup"><span data-stu-id="eda89-151">2</span></span>|<span data-ttu-id="eda89-152">O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="eda89-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eda89-153">Relações</span><span class="sxs-lookup"><span data-stu-id="eda89-153">Relationships</span></span>

| <span data-ttu-id="eda89-154">Relação</span><span class="sxs-lookup"><span data-stu-id="eda89-154">Relationship</span></span> | <span data-ttu-id="eda89-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="eda89-155">Type</span></span>   | <span data-ttu-id="eda89-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="eda89-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="eda89-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="eda89-157">appDefinitions</span></span>|<span data-ttu-id="eda89-158">Coleção [teamsAppDefinition](teamsappdefinition.md) </span><span class="sxs-lookup"><span data-stu-id="eda89-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="eda89-159">Os detalhes para cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eda89-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eda89-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eda89-160">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "string",
  "distributionMethod": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="eda89-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="eda89-161">See also</span></span>

- [<span data-ttu-id="eda89-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="eda89-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="eda89-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="eda89-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="eda89-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eda89-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


