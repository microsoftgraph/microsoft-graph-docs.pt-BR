---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2307bd50509cc1a44ee4de0a30309a2be98dcb3e
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791670"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="c824e-103">tipo de recurso teamsApp</span><span class="sxs-lookup"><span data-stu-id="c824e-103">teamsApp resource type</span></span>

<span data-ttu-id="c824e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c824e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c824e-105">Representa um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c824e-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="c824e-106">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="c824e-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="c824e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c824e-107">Methods</span></span>

| <span data-ttu-id="c824e-108">Método</span><span class="sxs-lookup"><span data-stu-id="c824e-108">Method</span></span>       | <span data-ttu-id="c824e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c824e-109">Return Type</span></span>  |<span data-ttu-id="c824e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c824e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c824e-111">Lista de aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="c824e-111">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="c824e-112">Coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="c824e-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="c824e-113">Lista de aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c824e-113">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="c824e-114">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="c824e-114">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="c824e-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c824e-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="c824e-116">Publica um aplicativo ao catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="c824e-116">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="c824e-117">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="c824e-117">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="c824e-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c824e-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="c824e-119">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="c824e-119">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="c824e-120">Apagar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="c824e-120">Delete a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="c824e-121">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="c824e-121">None</span></span> | <span data-ttu-id="c824e-122">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="c824e-122">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="c824e-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c824e-123">Properties</span></span>

| <span data-ttu-id="c824e-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c824e-124">Property</span></span>            | <span data-ttu-id="c824e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="c824e-125">Type</span></span>     | <span data-ttu-id="c824e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c824e-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="c824e-127">id</span><span class="sxs-lookup"><span data-stu-id="c824e-127">id</span></span>                  | <span data-ttu-id="c824e-128">string</span><span class="sxs-lookup"><span data-stu-id="c824e-128">string</span></span>   | <span data-ttu-id="c824e-129">A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="c824e-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="c824e-130">externalId</span><span class="sxs-lookup"><span data-stu-id="c824e-130">externalId</span></span>          | <span data-ttu-id="c824e-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c824e-131">string</span></span>   | <span data-ttu-id="c824e-132">A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="c824e-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="c824e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c824e-133">displayName</span></span>                | <span data-ttu-id="c824e-134">string</span><span class="sxs-lookup"><span data-stu-id="c824e-134">string</span></span>   | <span data-ttu-id="c824e-135">O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="c824e-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="c824e-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="c824e-136">distributionMethod</span></span>  | <span data-ttu-id="c824e-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="c824e-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="c824e-138">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c824e-138">The method of distribution for the app.</span></span> <span data-ttu-id="c824e-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c824e-139">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="c824e-140">valores teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="c824e-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="c824e-141">Membro</span><span class="sxs-lookup"><span data-stu-id="c824e-141">Member</span></span>|<span data-ttu-id="c824e-142">Valor</span><span class="sxs-lookup"><span data-stu-id="c824e-142">Value</span></span>|<span data-ttu-id="c824e-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="c824e-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c824e-144">loja</span><span class="sxs-lookup"><span data-stu-id="c824e-144">store</span></span>|<span data-ttu-id="c824e-145">0</span><span class="sxs-lookup"><span data-stu-id="c824e-145">0</span></span>| <span data-ttu-id="c824e-146">O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c824e-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="c824e-147">organização</span><span class="sxs-lookup"><span data-stu-id="c824e-147">organization</span></span>|<span data-ttu-id="c824e-148">1</span><span class="sxs-lookup"><span data-stu-id="c824e-148">1</span></span>|<span data-ttu-id="c824e-149">O aplicativo está disponível somente nesse locatário.</span><span class="sxs-lookup"><span data-stu-id="c824e-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="c824e-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="c824e-150">sideloaded</span></span>|<span data-ttu-id="c824e-151">2</span><span class="sxs-lookup"><span data-stu-id="c824e-151">2</span></span>|<span data-ttu-id="c824e-152">O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="c824e-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c824e-153">Relações</span><span class="sxs-lookup"><span data-stu-id="c824e-153">Relationships</span></span>

| <span data-ttu-id="c824e-154">Relação</span><span class="sxs-lookup"><span data-stu-id="c824e-154">Relationship</span></span> | <span data-ttu-id="c824e-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="c824e-155">Type</span></span>   | <span data-ttu-id="c824e-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="c824e-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c824e-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="c824e-157">appDefinitions</span></span>|<span data-ttu-id="c824e-158">Coleção [teamsAppDefinition](teamsappdefinition.md) </span><span class="sxs-lookup"><span data-stu-id="c824e-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="c824e-159">Os detalhes para cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c824e-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c824e-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c824e-160">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c824e-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="c824e-161">See also</span></span>

- [<span data-ttu-id="c824e-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c824e-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="c824e-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c824e-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="c824e-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c824e-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

