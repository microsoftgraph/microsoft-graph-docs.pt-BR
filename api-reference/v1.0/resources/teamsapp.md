---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2493b7f6adee51e5c5622585055cbd3cf2778656
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462267"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="2a572-103">tipo de recurso teamsApp</span><span class="sxs-lookup"><span data-stu-id="2a572-103">teamsApp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a572-104">Um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="2a572-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="2a572-105">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="2a572-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="2a572-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2a572-106">Methods</span></span>

| <span data-ttu-id="2a572-107">Método</span><span class="sxs-lookup"><span data-stu-id="2a572-107">Method</span></span>       | <span data-ttu-id="2a572-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2a572-108">Return Type</span></span>  |<span data-ttu-id="2a572-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a572-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a572-110">Lista de aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="2a572-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="2a572-111">Coleção [teamsApp](teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a572-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="2a572-112">Lista de aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2a572-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|<span data-ttu-id="2a572-113">[Publicar um aplicativo](../api/teamsapp-publish.md)</span><span class="sxs-lookup"><span data-stu-id="2a572-113">[AppCatalog.ReadWrite.All: Publish an app (](../api/teamsapp-publish.md))</span></span> | [<span data-ttu-id="2a572-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2a572-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="2a572-115">Publica um aplicativo ao catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="2a572-115">Publish an app to your organization's app catalog.</span></span>|
|<span data-ttu-id="2a572-116">[Atualizar um aplicativo publicado](../api/teamsapp-update.md)</span><span class="sxs-lookup"><span data-stu-id="2a572-116">[AppCatalog.ReadWrite.All: Update a published app (](../api/teamsapp-update.md))</span></span> | [<span data-ttu-id="2a572-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2a572-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="2a572-118">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="2a572-118">Update a published app in your organization's app catalog.</span></span>|
|<span data-ttu-id="2a572-119">[Remover um aplicativo publicado](../api/teamsapp-delete.md)</span><span class="sxs-lookup"><span data-stu-id="2a572-119">[AppCatalog.ReadWrite.All: Remove a published app (](../api/teamsapp-delete.md))</span></span> | <span data-ttu-id="2a572-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2a572-120">None</span></span> | <span data-ttu-id="2a572-121">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="2a572-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a572-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a572-122">Properties</span></span>

| <span data-ttu-id="2a572-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a572-123">Property</span></span>            | <span data-ttu-id="2a572-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a572-124">Type</span></span>     | <span data-ttu-id="2a572-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a572-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="2a572-126">id</span><span class="sxs-lookup"><span data-stu-id="2a572-126">id</span></span>                  | <span data-ttu-id="2a572-127">string</span><span class="sxs-lookup"><span data-stu-id="2a572-127">string</span></span>   | <span data-ttu-id="2a572-128">A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](https://docs.microsoft.com/pt-BR/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="2a572-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/pt-BR/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="2a572-129">externalId</span><span class="sxs-lookup"><span data-stu-id="2a572-129">externalId</span></span>          | <span data-ttu-id="2a572-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a572-130">string</span></span>   | <span data-ttu-id="2a572-131">A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](https://docs.microsoft.com/pt-BR/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="2a572-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/pt-BR/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="2a572-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2a572-132">displayName</span></span>                | <span data-ttu-id="2a572-133">string</span><span class="sxs-lookup"><span data-stu-id="2a572-133">string</span></span>   | <span data-ttu-id="2a572-134">O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](https://docs.microsoft.com/pt-BR/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="2a572-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/pt-BR/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="2a572-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="2a572-135">distributionMethod</span></span>  | <span data-ttu-id="2a572-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="2a572-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="2a572-137">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a572-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="2a572-138">valores teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="2a572-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="2a572-139">Membro</span><span class="sxs-lookup"><span data-stu-id="2a572-139">Member</span></span>|<span data-ttu-id="2a572-140">Valor</span><span class="sxs-lookup"><span data-stu-id="2a572-140">Value</span></span>|<span data-ttu-id="2a572-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a572-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a572-142">loja</span><span class="sxs-lookup"><span data-stu-id="2a572-142">Store</span></span>|<span data-ttu-id="2a572-143">0</span><span class="sxs-lookup"><span data-stu-id="2a572-143">0%</span></span>| <span data-ttu-id="2a572-144">O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2a572-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="2a572-145">organização</span><span class="sxs-lookup"><span data-stu-id="2a572-145">organization</span></span>|<span data-ttu-id="2a572-146">1</span><span class="sxs-lookup"><span data-stu-id="2a572-146">$1</span></span>|<span data-ttu-id="2a572-147">O aplicativo está disponível somente nesse locatário.</span><span class="sxs-lookup"><span data-stu-id="2a572-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="2a572-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="2a572-148">sideloaded</span></span>|<span data-ttu-id="2a572-149">2</span><span class="sxs-lookup"><span data-stu-id="2a572-149">-2</span></span>|<span data-ttu-id="2a572-150">O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="2a572-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a572-151">Relações</span><span class="sxs-lookup"><span data-stu-id="2a572-151">Relationships</span></span>

| <span data-ttu-id="2a572-152">Relação</span><span class="sxs-lookup"><span data-stu-id="2a572-152">Relationship</span></span> | <span data-ttu-id="2a572-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a572-153">Type</span></span>   | <span data-ttu-id="2a572-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a572-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2a572-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="2a572-155">appDefinitions</span></span>|<span data-ttu-id="2a572-156">Coleção [teamsAppDefinition](teamsappdefinition.md) </span><span class="sxs-lookup"><span data-stu-id="2a572-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="2a572-157">Os detalhes para cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a572-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2a572-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a572-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="2a572-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="2a572-159">See also</span></span>

- [<span data-ttu-id="2a572-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2a572-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="2a572-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2a572-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="2a572-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2a572-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsapp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

