---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: eb7c75f144f2056e610e45f86b44a19d9211f306
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706119"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="d06f2-103">tipo de recurso teamsApp</span><span class="sxs-lookup"><span data-stu-id="d06f2-103">teamsApp resource type</span></span>

<span data-ttu-id="d06f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d06f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d06f2-105">Representa um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="d06f2-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="d06f2-106">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/team-post-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="d06f2-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/team-post-installedapps.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="d06f2-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d06f2-107">Methods</span></span>

| <span data-ttu-id="d06f2-108">Método</span><span class="sxs-lookup"><span data-stu-id="d06f2-108">Method</span></span>       | <span data-ttu-id="d06f2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d06f2-109">Return Type</span></span>  |<span data-ttu-id="d06f2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d06f2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d06f2-111">Listar aplicativos no catálogo</span><span class="sxs-lookup"><span data-stu-id="d06f2-111">List apps in catalog</span></span>](../api/appcatalogs-list-teamsapps.md) | <span data-ttu-id="d06f2-112">Coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="d06f2-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="d06f2-113">Listar todos os aplicativos no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d06f2-113">List all the apps in the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="d06f2-114">Carregar aplicativo no catálogo</span><span class="sxs-lookup"><span data-stu-id="d06f2-114">Upload app to catalog</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="d06f2-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d06f2-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="d06f2-116">Carregar um aplicativo para o catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="d06f2-116">Upload an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="d06f2-117">Atualizar aplicativo no catálogo</span><span class="sxs-lookup"><span data-stu-id="d06f2-117">Update app in catalog</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="d06f2-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d06f2-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="d06f2-119">Atualize um aplicativo no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="d06f2-119">Update an app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="d06f2-120">Excluir aplicativo do catálogo</span><span class="sxs-lookup"><span data-stu-id="d06f2-120">Delete app from catalog</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="d06f2-121">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="d06f2-121">None</span></span> | <span data-ttu-id="d06f2-122">Remover um aplicativo do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="d06f2-122">Remove an app from your organization's app catalog.</span></span>|
|[<span data-ttu-id="d06f2-123">Obter bot associado ao aplicativo no catálogo</span><span class="sxs-lookup"><span data-stu-id="d06f2-123">Get bot associated with app in catalog</span></span>](../api/teamworkbot-get.md) | [<span data-ttu-id="d06f2-124">teamworkbot</span><span class="sxs-lookup"><span data-stu-id="d06f2-124">teamworkbot</span></span>](teamworkbot.md) | <span data-ttu-id="d06f2-125">Obter o bot associado ao aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="d06f2-125">Get the bot associated with the Teams app.</span></span>|

## <a name="properties"></a><span data-ttu-id="d06f2-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d06f2-126">Properties</span></span>

| <span data-ttu-id="d06f2-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d06f2-127">Property</span></span>            | <span data-ttu-id="d06f2-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="d06f2-128">Type</span></span>     | <span data-ttu-id="d06f2-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d06f2-129">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d06f2-130">id</span><span class="sxs-lookup"><span data-stu-id="d06f2-130">id</span></span>                  | <span data-ttu-id="d06f2-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d06f2-131">string</span></span>   | <span data-ttu-id="d06f2-132">A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="d06f2-132">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d06f2-133">externalId</span><span class="sxs-lookup"><span data-stu-id="d06f2-133">externalId</span></span>          | <span data-ttu-id="d06f2-134">string</span><span class="sxs-lookup"><span data-stu-id="d06f2-134">string</span></span>   | <span data-ttu-id="d06f2-135">A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="d06f2-135">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d06f2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d06f2-136">displayName</span></span>                | <span data-ttu-id="d06f2-137">string</span><span class="sxs-lookup"><span data-stu-id="d06f2-137">string</span></span>   | <span data-ttu-id="d06f2-138">O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="d06f2-138">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d06f2-139">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="d06f2-139">distributionMethod</span></span>  | <span data-ttu-id="d06f2-140">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="d06f2-140">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="d06f2-141">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d06f2-141">The method of distribution for the app.</span></span> <span data-ttu-id="d06f2-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d06f2-142">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="d06f2-143">valores teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="d06f2-143">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="d06f2-144">Membro</span><span class="sxs-lookup"><span data-stu-id="d06f2-144">Member</span></span>|<span data-ttu-id="d06f2-145">Valor</span><span class="sxs-lookup"><span data-stu-id="d06f2-145">Value</span></span>|<span data-ttu-id="d06f2-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="d06f2-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d06f2-147">loja</span><span class="sxs-lookup"><span data-stu-id="d06f2-147">store</span></span>|<span data-ttu-id="d06f2-148">,0</span><span class="sxs-lookup"><span data-stu-id="d06f2-148">0</span></span>| <span data-ttu-id="d06f2-149">O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d06f2-149">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="d06f2-150">organização</span><span class="sxs-lookup"><span data-stu-id="d06f2-150">organization</span></span>|<span data-ttu-id="d06f2-151">1</span><span class="sxs-lookup"><span data-stu-id="d06f2-151">1</span></span>|<span data-ttu-id="d06f2-152">O aplicativo está disponível somente nesse locatário.</span><span class="sxs-lookup"><span data-stu-id="d06f2-152">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="d06f2-153">sideloaded</span><span class="sxs-lookup"><span data-stu-id="d06f2-153">sideloaded</span></span>|<span data-ttu-id="d06f2-154">duas</span><span class="sxs-lookup"><span data-stu-id="d06f2-154">2</span></span>|<span data-ttu-id="d06f2-155">O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="d06f2-155">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d06f2-156">Relações</span><span class="sxs-lookup"><span data-stu-id="d06f2-156">Relationships</span></span>

| <span data-ttu-id="d06f2-157">Relação</span><span class="sxs-lookup"><span data-stu-id="d06f2-157">Relationship</span></span> | <span data-ttu-id="d06f2-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="d06f2-158">Type</span></span>   | <span data-ttu-id="d06f2-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="d06f2-159">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d06f2-160">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="d06f2-160">appDefinitions</span></span>|<span data-ttu-id="d06f2-161">Coleção [teamsAppDefinition](teamsappdefinition.md) </span><span class="sxs-lookup"><span data-stu-id="d06f2-161">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="d06f2-162">Os detalhes para cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d06f2-162">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d06f2-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d06f2-163">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="d06f2-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="d06f2-164">See also</span></span>

- [<span data-ttu-id="d06f2-165">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d06f2-165">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="d06f2-166">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d06f2-166">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="d06f2-167">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d06f2-167">teamsTab</span></span>](../resources/teamstab.md)

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



