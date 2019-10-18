---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9cd1122a39fbe99e62c578486d863af8e13b96b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033807"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="8f1c8-103">tipo de recurso teamsApp</span><span class="sxs-lookup"><span data-stu-id="8f1c8-103">teamsApp resource type</span></span>



<span data-ttu-id="8f1c8-104">Um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8f1c8-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="8f1c8-105">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="8f1c8-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="8f1c8-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8f1c8-106">Methods</span></span>

| <span data-ttu-id="8f1c8-107">Método</span><span class="sxs-lookup"><span data-stu-id="8f1c8-107">Method</span></span>       | <span data-ttu-id="8f1c8-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8f1c8-108">Return Type</span></span>  |<span data-ttu-id="8f1c8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f1c8-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f1c8-110">Lista de aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="8f1c8-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="8f1c8-111">Coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="8f1c8-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="8f1c8-112">Lista de aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8f1c8-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="8f1c8-113">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f1c8-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="8f1c8-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8f1c8-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="8f1c8-115">Publica um aplicativo ao catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="8f1c8-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="8f1c8-116">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="8f1c8-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="8f1c8-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="8f1c8-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="8f1c8-118">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="8f1c8-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="8f1c8-119">Remover um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="8f1c8-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="8f1c8-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f1c8-120">None</span></span> | <span data-ttu-id="8f1c8-121">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="8f1c8-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f1c8-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f1c8-122">Properties</span></span>

| <span data-ttu-id="8f1c8-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f1c8-123">Property</span></span>            | <span data-ttu-id="8f1c8-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f1c8-124">Type</span></span>     | <span data-ttu-id="8f1c8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f1c8-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="8f1c8-126">id</span><span class="sxs-lookup"><span data-stu-id="8f1c8-126">id</span></span>                  | <span data-ttu-id="8f1c8-127">string</span><span class="sxs-lookup"><span data-stu-id="8f1c8-127">string</span></span>   | <span data-ttu-id="8f1c8-128">A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8f1c8-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="8f1c8-129">externalId</span><span class="sxs-lookup"><span data-stu-id="8f1c8-129">externalId</span></span>          | <span data-ttu-id="8f1c8-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f1c8-130">string</span></span>   | <span data-ttu-id="8f1c8-131">A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8f1c8-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="8f1c8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8f1c8-132">displayName</span></span>                | <span data-ttu-id="8f1c8-133">string</span><span class="sxs-lookup"><span data-stu-id="8f1c8-133">string</span></span>   | <span data-ttu-id="8f1c8-134">O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="8f1c8-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="8f1c8-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="8f1c8-135">distributionMethod</span></span>  | <span data-ttu-id="8f1c8-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="8f1c8-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="8f1c8-137">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f1c8-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="8f1c8-138">valores teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="8f1c8-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="8f1c8-139">Membro</span><span class="sxs-lookup"><span data-stu-id="8f1c8-139">Member</span></span>|<span data-ttu-id="8f1c8-140">Valor</span><span class="sxs-lookup"><span data-stu-id="8f1c8-140">Value</span></span>|<span data-ttu-id="8f1c8-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f1c8-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f1c8-142">loja</span><span class="sxs-lookup"><span data-stu-id="8f1c8-142">store</span></span>|<span data-ttu-id="8f1c8-143">0</span><span class="sxs-lookup"><span data-stu-id="8f1c8-143">0</span></span>| <span data-ttu-id="8f1c8-144">O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8f1c8-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="8f1c8-145">organização</span><span class="sxs-lookup"><span data-stu-id="8f1c8-145">organization</span></span>|<span data-ttu-id="8f1c8-146">1</span><span class="sxs-lookup"><span data-stu-id="8f1c8-146">1</span></span>|<span data-ttu-id="8f1c8-147">O aplicativo está disponível somente nesse locatário.</span><span class="sxs-lookup"><span data-stu-id="8f1c8-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="8f1c8-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="8f1c8-148">sideloaded</span></span>|<span data-ttu-id="8f1c8-149">2</span><span class="sxs-lookup"><span data-stu-id="8f1c8-149">2</span></span>|<span data-ttu-id="8f1c8-150">O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="8f1c8-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f1c8-151">Relações</span><span class="sxs-lookup"><span data-stu-id="8f1c8-151">Relationships</span></span>

| <span data-ttu-id="8f1c8-152">Relação</span><span class="sxs-lookup"><span data-stu-id="8f1c8-152">Relationship</span></span> | <span data-ttu-id="8f1c8-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f1c8-153">Type</span></span>   | <span data-ttu-id="8f1c8-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f1c8-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8f1c8-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="8f1c8-155">appDefinitions</span></span>|<span data-ttu-id="8f1c8-156">Coleção [teamsAppDefinition](teamsappdefinition.md) </span><span class="sxs-lookup"><span data-stu-id="8f1c8-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="8f1c8-157">Os detalhes para cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f1c8-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8f1c8-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f1c8-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="8f1c8-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="8f1c8-159">See also</span></span>

- [<span data-ttu-id="8f1c8-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8f1c8-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="8f1c8-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="8f1c8-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="8f1c8-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="8f1c8-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

