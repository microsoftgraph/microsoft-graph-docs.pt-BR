---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f623a71a7d07a019615cfb43a664d875b8dd2def
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791607"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="dc37a-103">tipo de recurso teamsApp</span><span class="sxs-lookup"><span data-stu-id="dc37a-103">teamsApp resource type</span></span>

<span data-ttu-id="dc37a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc37a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc37a-105">Representa um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md) .</span><span class="sxs-lookup"><span data-stu-id="dc37a-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="dc37a-106">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="dc37a-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="dc37a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="dc37a-107">Methods</span></span>

| <span data-ttu-id="dc37a-108">Método</span><span class="sxs-lookup"><span data-stu-id="dc37a-108">Method</span></span>       | <span data-ttu-id="dc37a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dc37a-109">Return Type</span></span>  |<span data-ttu-id="dc37a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc37a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc37a-111">Lista de aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="dc37a-111">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="dc37a-112">Coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="dc37a-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="dc37a-113">Lista de aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="dc37a-113">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="dc37a-114">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc37a-114">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="dc37a-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="dc37a-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="dc37a-116">Publica um aplicativo ao catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="dc37a-116">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="dc37a-117">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="dc37a-117">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="dc37a-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="dc37a-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="dc37a-119">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="dc37a-119">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="dc37a-120">Excluir um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="dc37a-120">Delete a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="dc37a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc37a-121">None</span></span> | <span data-ttu-id="dc37a-122">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="dc37a-122">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc37a-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc37a-123">Properties</span></span>

| <span data-ttu-id="dc37a-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc37a-124">Property</span></span>            | <span data-ttu-id="dc37a-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc37a-125">Type</span></span>     | <span data-ttu-id="dc37a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc37a-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="dc37a-127">id</span><span class="sxs-lookup"><span data-stu-id="dc37a-127">id</span></span>                  | <span data-ttu-id="dc37a-128">string</span><span class="sxs-lookup"><span data-stu-id="dc37a-128">string</span></span>   | <span data-ttu-id="dc37a-129">A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="dc37a-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="dc37a-130">externalId</span><span class="sxs-lookup"><span data-stu-id="dc37a-130">externalId</span></span>          | <span data-ttu-id="dc37a-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc37a-131">string</span></span>   | <span data-ttu-id="dc37a-132">A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="dc37a-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="dc37a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="dc37a-133">displayName</span></span>                | <span data-ttu-id="dc37a-134">string</span><span class="sxs-lookup"><span data-stu-id="dc37a-134">string</span></span>   | <span data-ttu-id="dc37a-135">O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="dc37a-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="dc37a-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="dc37a-136">distributionMethod</span></span>  | <span data-ttu-id="dc37a-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="dc37a-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="dc37a-138">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc37a-138">The method of distribution for the app.</span></span> <span data-ttu-id="dc37a-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc37a-139">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="dc37a-140">valores teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="dc37a-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="dc37a-141">Membro</span><span class="sxs-lookup"><span data-stu-id="dc37a-141">Member</span></span>|<span data-ttu-id="dc37a-142">Valor</span><span class="sxs-lookup"><span data-stu-id="dc37a-142">Value</span></span>|<span data-ttu-id="dc37a-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc37a-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc37a-144">loja</span><span class="sxs-lookup"><span data-stu-id="dc37a-144">store</span></span>|<span data-ttu-id="dc37a-145">,0</span><span class="sxs-lookup"><span data-stu-id="dc37a-145">0</span></span>| <span data-ttu-id="dc37a-146">O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="dc37a-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="dc37a-147">organização</span><span class="sxs-lookup"><span data-stu-id="dc37a-147">organization</span></span>|<span data-ttu-id="dc37a-148">1</span><span class="sxs-lookup"><span data-stu-id="dc37a-148">1</span></span>|<span data-ttu-id="dc37a-149">O aplicativo está disponível somente nesse locatário.</span><span class="sxs-lookup"><span data-stu-id="dc37a-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="dc37a-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="dc37a-150">sideloaded</span></span>|<span data-ttu-id="dc37a-151">duas</span><span class="sxs-lookup"><span data-stu-id="dc37a-151">2</span></span>|<span data-ttu-id="dc37a-152">O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="dc37a-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc37a-153">Relações</span><span class="sxs-lookup"><span data-stu-id="dc37a-153">Relationships</span></span>

| <span data-ttu-id="dc37a-154">Relação</span><span class="sxs-lookup"><span data-stu-id="dc37a-154">Relationship</span></span> | <span data-ttu-id="dc37a-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc37a-155">Type</span></span>   | <span data-ttu-id="dc37a-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc37a-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dc37a-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="dc37a-157">appDefinitions</span></span>|<span data-ttu-id="dc37a-158">Coleção [teamsAppDefinition](teamsappdefinition.md) </span><span class="sxs-lookup"><span data-stu-id="dc37a-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="dc37a-159">Os detalhes para cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc37a-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dc37a-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc37a-160">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="dc37a-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="dc37a-161">See also</span></span>

- [<span data-ttu-id="dc37a-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="dc37a-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="dc37a-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="dc37a-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="dc37a-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dc37a-164">teamsTab</span></span>](../resources/teamstab.md)

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

