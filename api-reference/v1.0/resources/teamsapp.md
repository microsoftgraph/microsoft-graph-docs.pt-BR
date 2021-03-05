---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2ffa5b3f5562e83d1e1e1ef64629e39a1da41cd4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472857"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="27386-103">tipo de recurso teamsApp</span><span class="sxs-lookup"><span data-stu-id="27386-103">teamsApp resource type</span></span>

<span data-ttu-id="27386-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27386-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27386-105">Representa um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="27386-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="27386-106">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/team-post-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="27386-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/team-post-installedapps.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="27386-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="27386-107">Methods</span></span>

| <span data-ttu-id="27386-108">Método</span><span class="sxs-lookup"><span data-stu-id="27386-108">Method</span></span>       | <span data-ttu-id="27386-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="27386-109">Return Type</span></span>  |<span data-ttu-id="27386-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="27386-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27386-111">Listar aplicativos no catálogo</span><span class="sxs-lookup"><span data-stu-id="27386-111">List apps in catalog</span></span>](../api/appcatalogs-list-teamsapps.md) | <span data-ttu-id="27386-112">Coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="27386-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="27386-113">Liste todos os aplicativos no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="27386-113">List all the apps in the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="27386-114">Carregar aplicativo no catálogo</span><span class="sxs-lookup"><span data-stu-id="27386-114">Upload app to catalog</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="27386-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="27386-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="27386-116">Faça upload de um aplicativo para o catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="27386-116">Upload an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="27386-117">Atualizar aplicativo no catálogo</span><span class="sxs-lookup"><span data-stu-id="27386-117">Update app in catalog</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="27386-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="27386-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="27386-119">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="27386-119">Update an app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="27386-120">Remover aplicativo do catálogo</span><span class="sxs-lookup"><span data-stu-id="27386-120">Delete app from catalog</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="27386-121">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="27386-121">None</span></span> | <span data-ttu-id="27386-122">Remova um aplicativo do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="27386-122">Remove an app from your organization's app catalog.</span></span>|
|[<span data-ttu-id="27386-123">Obter um bot associado ao aplicativo no catálogo</span><span class="sxs-lookup"><span data-stu-id="27386-123">Get bot associated with app in catalog</span></span>](../api/teamworkbot-get.md) | [<span data-ttu-id="27386-124">teamworkbot</span><span class="sxs-lookup"><span data-stu-id="27386-124">teamworkbot</span></span>](teamworkbot.md) | <span data-ttu-id="27386-125">Obter o bot associado ao aplicativo no Teams.</span><span class="sxs-lookup"><span data-stu-id="27386-125">Get the bot associated with the Teams app.</span></span>|

## <a name="properties"></a><span data-ttu-id="27386-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27386-126">Properties</span></span>

| <span data-ttu-id="27386-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27386-127">Property</span></span>            | <span data-ttu-id="27386-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="27386-128">Type</span></span>     | <span data-ttu-id="27386-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="27386-129">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="27386-130">id</span><span class="sxs-lookup"><span data-stu-id="27386-130">id</span></span>                  | <span data-ttu-id="27386-131">string</span><span class="sxs-lookup"><span data-stu-id="27386-131">string</span></span>   | <span data-ttu-id="27386-132">A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="27386-132">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="27386-133">externalId</span><span class="sxs-lookup"><span data-stu-id="27386-133">externalId</span></span>          | <span data-ttu-id="27386-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27386-134">string</span></span>   | <span data-ttu-id="27386-135">A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="27386-135">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="27386-136">displayName</span><span class="sxs-lookup"><span data-stu-id="27386-136">displayName</span></span>                | <span data-ttu-id="27386-137">string</span><span class="sxs-lookup"><span data-stu-id="27386-137">string</span></span>   | <span data-ttu-id="27386-138">O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="27386-138">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="27386-139">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="27386-139">distributionMethod</span></span>  | <span data-ttu-id="27386-140">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="27386-140">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="27386-141">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27386-141">The method of distribution for the app.</span></span> <span data-ttu-id="27386-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27386-142">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="27386-143">valores teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="27386-143">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="27386-144">Membro</span><span class="sxs-lookup"><span data-stu-id="27386-144">Member</span></span>|<span data-ttu-id="27386-145">Valor</span><span class="sxs-lookup"><span data-stu-id="27386-145">Value</span></span>|<span data-ttu-id="27386-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="27386-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27386-147">loja</span><span class="sxs-lookup"><span data-stu-id="27386-147">store</span></span>|<span data-ttu-id="27386-148">0</span><span class="sxs-lookup"><span data-stu-id="27386-148">0</span></span>| <span data-ttu-id="27386-149">O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="27386-149">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="27386-150">organização</span><span class="sxs-lookup"><span data-stu-id="27386-150">organization</span></span>|<span data-ttu-id="27386-151">1</span><span class="sxs-lookup"><span data-stu-id="27386-151">1</span></span>|<span data-ttu-id="27386-152">O aplicativo está disponível somente nesse locatário.</span><span class="sxs-lookup"><span data-stu-id="27386-152">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="27386-153">sideloaded</span><span class="sxs-lookup"><span data-stu-id="27386-153">sideloaded</span></span>|<span data-ttu-id="27386-154">2</span><span class="sxs-lookup"><span data-stu-id="27386-154">2</span></span>|<span data-ttu-id="27386-155">O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="27386-155">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27386-156">Relações</span><span class="sxs-lookup"><span data-stu-id="27386-156">Relationships</span></span>

| <span data-ttu-id="27386-157">Relação</span><span class="sxs-lookup"><span data-stu-id="27386-157">Relationship</span></span> | <span data-ttu-id="27386-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="27386-158">Type</span></span>   | <span data-ttu-id="27386-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="27386-159">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="27386-160">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="27386-160">appDefinitions</span></span>|<span data-ttu-id="27386-161">Coleção [teamsAppDefinition](teamsappdefinition.md) </span><span class="sxs-lookup"><span data-stu-id="27386-161">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="27386-162">Os detalhes para cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27386-162">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="27386-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27386-163">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="27386-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="27386-164">See also</span></span>

- [<span data-ttu-id="27386-165">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="27386-165">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="27386-166">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="27386-166">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="27386-167">teamsTab</span><span class="sxs-lookup"><span data-stu-id="27386-167">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


