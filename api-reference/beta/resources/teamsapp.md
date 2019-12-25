---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b3ee13166a81fad96e577efd6721983714ca17b4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870058"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="30d2e-103">tipo de recurso teamsApp</span><span class="sxs-lookup"><span data-stu-id="30d2e-103">teamsApp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30d2e-104">Um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="30d2e-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="30d2e-105">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="30d2e-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="30d2e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="30d2e-106">Methods</span></span>

| <span data-ttu-id="30d2e-107">Método</span><span class="sxs-lookup"><span data-stu-id="30d2e-107">Method</span></span>       | <span data-ttu-id="30d2e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="30d2e-108">Return Type</span></span>  |<span data-ttu-id="30d2e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="30d2e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30d2e-110">Lista de aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="30d2e-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="30d2e-111">Coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="30d2e-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="30d2e-112">Lista de aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="30d2e-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="30d2e-113">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="30d2e-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="30d2e-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="30d2e-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="30d2e-115">Publica um aplicativo ao catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="30d2e-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="30d2e-116">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="30d2e-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="30d2e-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="30d2e-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="30d2e-118">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="30d2e-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="30d2e-119">Remover um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="30d2e-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="30d2e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="30d2e-120">None</span></span> | <span data-ttu-id="30d2e-121">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="30d2e-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="30d2e-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30d2e-122">Properties</span></span>

| <span data-ttu-id="30d2e-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30d2e-123">Property</span></span>            | <span data-ttu-id="30d2e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="30d2e-124">Type</span></span>     | <span data-ttu-id="30d2e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="30d2e-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="30d2e-126">id</span><span class="sxs-lookup"><span data-stu-id="30d2e-126">id</span></span>                  | <span data-ttu-id="30d2e-127">string</span><span class="sxs-lookup"><span data-stu-id="30d2e-127">string</span></span>   | <span data-ttu-id="30d2e-128">A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="30d2e-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="30d2e-129">externalId</span><span class="sxs-lookup"><span data-stu-id="30d2e-129">externalId</span></span>          | <span data-ttu-id="30d2e-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30d2e-130">string</span></span>   | <span data-ttu-id="30d2e-131">A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="30d2e-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="30d2e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="30d2e-132">displayName</span></span>                | <span data-ttu-id="30d2e-133">string</span><span class="sxs-lookup"><span data-stu-id="30d2e-133">string</span></span>   | <span data-ttu-id="30d2e-134">O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="30d2e-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="30d2e-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="30d2e-135">distributionMethod</span></span>  | <span data-ttu-id="30d2e-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="30d2e-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="30d2e-137">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30d2e-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="30d2e-138">valores teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="30d2e-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="30d2e-139">Membro</span><span class="sxs-lookup"><span data-stu-id="30d2e-139">Member</span></span>|<span data-ttu-id="30d2e-140">Valor</span><span class="sxs-lookup"><span data-stu-id="30d2e-140">Value</span></span>|<span data-ttu-id="30d2e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="30d2e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30d2e-142">loja</span><span class="sxs-lookup"><span data-stu-id="30d2e-142">store</span></span>|<span data-ttu-id="30d2e-143">0</span><span class="sxs-lookup"><span data-stu-id="30d2e-143">0</span></span>| <span data-ttu-id="30d2e-144">O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="30d2e-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="30d2e-145">organização</span><span class="sxs-lookup"><span data-stu-id="30d2e-145">organization</span></span>|<span data-ttu-id="30d2e-146">1</span><span class="sxs-lookup"><span data-stu-id="30d2e-146">1</span></span>|<span data-ttu-id="30d2e-147">O aplicativo está disponível somente nesse locatário.</span><span class="sxs-lookup"><span data-stu-id="30d2e-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="30d2e-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="30d2e-148">sideloaded</span></span>|<span data-ttu-id="30d2e-149">2</span><span class="sxs-lookup"><span data-stu-id="30d2e-149">2</span></span>|<span data-ttu-id="30d2e-150">O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="30d2e-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30d2e-151">Relações</span><span class="sxs-lookup"><span data-stu-id="30d2e-151">Relationships</span></span>

| <span data-ttu-id="30d2e-152">Relação</span><span class="sxs-lookup"><span data-stu-id="30d2e-152">Relationship</span></span> | <span data-ttu-id="30d2e-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="30d2e-153">Type</span></span>   | <span data-ttu-id="30d2e-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="30d2e-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="30d2e-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="30d2e-155">appDefinitions</span></span>|<span data-ttu-id="30d2e-156">Coleção [teamsAppDefinition](teamsappdefinition.md) </span><span class="sxs-lookup"><span data-stu-id="30d2e-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="30d2e-157">Os detalhes para cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30d2e-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="30d2e-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30d2e-158">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="30d2e-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="30d2e-159">See also</span></span>

- [<span data-ttu-id="30d2e-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="30d2e-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="30d2e-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="30d2e-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="30d2e-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="30d2e-162">teamsTab</span></span>](../resources/teamstab.md)

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

