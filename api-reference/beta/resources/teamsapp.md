---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a944c9aa1f679b053fa7ceda645885b584a1dce
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606787"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="52509-103">tipo de recurso teamsApp</span><span class="sxs-lookup"><span data-stu-id="52509-103">teamsApp resource type</span></span>

<span data-ttu-id="52509-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52509-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52509-105">Representa um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="52509-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="52509-106">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/team-post-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="52509-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/team-post-installedapps.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="52509-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="52509-107">Methods</span></span>

| <span data-ttu-id="52509-108">Método</span><span class="sxs-lookup"><span data-stu-id="52509-108">Method</span></span>       | <span data-ttu-id="52509-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52509-109">Return Type</span></span>  |<span data-ttu-id="52509-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="52509-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52509-111">Lista de aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="52509-111">List published apps</span></span>](../api/appcatalogs-list-teamsapps.md) | <span data-ttu-id="52509-112">Coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="52509-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="52509-113">Lista de aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="52509-113">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="52509-114">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="52509-114">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="52509-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="52509-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="52509-116">Publica um aplicativo ao catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="52509-116">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="52509-117">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="52509-117">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="52509-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="52509-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="52509-119">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="52509-119">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="52509-120">Apagar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="52509-120">Delete a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="52509-121">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="52509-121">None</span></span> | <span data-ttu-id="52509-122">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="52509-122">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="52509-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52509-123">Properties</span></span>

| <span data-ttu-id="52509-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52509-124">Property</span></span>            | <span data-ttu-id="52509-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="52509-125">Type</span></span>     | <span data-ttu-id="52509-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="52509-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="52509-127">id</span><span class="sxs-lookup"><span data-stu-id="52509-127">id</span></span>                  | <span data-ttu-id="52509-128">string</span><span class="sxs-lookup"><span data-stu-id="52509-128">string</span></span>   | <span data-ttu-id="52509-129">A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="52509-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="52509-130">externalId</span><span class="sxs-lookup"><span data-stu-id="52509-130">externalId</span></span>          | <span data-ttu-id="52509-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52509-131">string</span></span>   | <span data-ttu-id="52509-132">A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="52509-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="52509-133">displayName</span><span class="sxs-lookup"><span data-stu-id="52509-133">displayName</span></span>                | <span data-ttu-id="52509-134">string</span><span class="sxs-lookup"><span data-stu-id="52509-134">string</span></span>   | <span data-ttu-id="52509-135">O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="52509-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="52509-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="52509-136">distributionMethod</span></span>  | <span data-ttu-id="52509-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="52509-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="52509-138">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="52509-138">The method of distribution for the app.</span></span> <span data-ttu-id="52509-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52509-139">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="52509-140">valores teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="52509-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="52509-141">Membro</span><span class="sxs-lookup"><span data-stu-id="52509-141">Member</span></span>|<span data-ttu-id="52509-142">Valor</span><span class="sxs-lookup"><span data-stu-id="52509-142">Value</span></span>|<span data-ttu-id="52509-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="52509-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52509-144">loja</span><span class="sxs-lookup"><span data-stu-id="52509-144">store</span></span>|<span data-ttu-id="52509-145">0</span><span class="sxs-lookup"><span data-stu-id="52509-145">0</span></span>| <span data-ttu-id="52509-146">O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="52509-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="52509-147">organização</span><span class="sxs-lookup"><span data-stu-id="52509-147">organization</span></span>|<span data-ttu-id="52509-148">1</span><span class="sxs-lookup"><span data-stu-id="52509-148">1</span></span>|<span data-ttu-id="52509-149">O aplicativo está disponível somente nesse locatário.</span><span class="sxs-lookup"><span data-stu-id="52509-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="52509-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="52509-150">sideloaded</span></span>|<span data-ttu-id="52509-151">2</span><span class="sxs-lookup"><span data-stu-id="52509-151">2</span></span>|<span data-ttu-id="52509-152">O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="52509-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52509-153">Relações</span><span class="sxs-lookup"><span data-stu-id="52509-153">Relationships</span></span>

| <span data-ttu-id="52509-154">Relação</span><span class="sxs-lookup"><span data-stu-id="52509-154">Relationship</span></span> | <span data-ttu-id="52509-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="52509-155">Type</span></span>   | <span data-ttu-id="52509-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="52509-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="52509-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="52509-157">appDefinitions</span></span>|<span data-ttu-id="52509-158">Coleção [teamsAppDefinition](teamsappdefinition.md) </span><span class="sxs-lookup"><span data-stu-id="52509-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="52509-159">Os detalhes para cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="52509-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52509-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52509-160">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="52509-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="52509-161">See also</span></span>

- [<span data-ttu-id="52509-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="52509-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="52509-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="52509-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="52509-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="52509-164">teamsTab</span></span>](../resources/teamstab.md)

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



