# <a name="teamsapp-resource-type"></a><span data-ttu-id="d045c-101">tipo de recurso de teamsApp</span><span class="sxs-lookup"><span data-stu-id="d045c-101">teamsApp resource type</span></span>



<span data-ttu-id="d045c-102">Um aplicativo no catálogo de aplicativos [Equipes da Microsoft](teams_api_overview.md) .</span><span class="sxs-lookup"><span data-stu-id="d045c-102">An app in the [Microsoft Teams](teams_api_overview.md) app catalog.</span></span>

<span data-ttu-id="d045c-103">Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados em [equipes](team.md) usando o método [Add app à equipe](../api/teamsappinstallation_add.md) .</span><span class="sxs-lookup"><span data-stu-id="d045c-103">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation_add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="d045c-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="d045c-104">Methods</span></span>

| <span data-ttu-id="d045c-105">Método</span><span class="sxs-lookup"><span data-stu-id="d045c-105">Method</span></span>       | <span data-ttu-id="d045c-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d045c-106">Return Type</span></span>  |<span data-ttu-id="d045c-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d045c-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d045c-108">Listar os aplicativos publicados</span><span class="sxs-lookup"><span data-stu-id="d045c-108">List published apps</span></span>](../api/teamsapp_list.md) | <span data-ttu-id="d045c-109">coleção [teamsApp](teamsApp.md)</span><span class="sxs-lookup"><span data-stu-id="d045c-109">[teamsApp](teamsApp.md) collection</span></span> | <span data-ttu-id="d045c-110">Liste aplicativos publicados do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d045c-110">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="d045c-111">Publicar um aplicativo</span><span class="sxs-lookup"><span data-stu-id="d045c-111">Publish an app</span></span>](../api/teamsapp_publish.md) | [<span data-ttu-id="d045c-112">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d045c-112">teamsApp</span></span>](teamsApp.md) | <span data-ttu-id="d045c-113">Publica um aplicativo no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="d045c-113">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="d045c-114">Atualizar um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="d045c-114">Update a published app</span></span>](../api/teamsapp_update.md) | [<span data-ttu-id="d045c-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d045c-115">teamsApp</span></span>](teamsApp.md) | <span data-ttu-id="d045c-116">Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="d045c-116">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="d045c-117">Remover um aplicativo publicado</span><span class="sxs-lookup"><span data-stu-id="d045c-117">Remove a published app</span></span>](../api/teamsapp_delete.md) | <span data-ttu-id="d045c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d045c-118">None</span></span> | <span data-ttu-id="d045c-119">Remova um aplicativo publicado do catálogo de aplicativos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="d045c-119">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="d045c-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d045c-120">Properties</span></span>

| <span data-ttu-id="d045c-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d045c-121">Property</span></span>            | <span data-ttu-id="d045c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d045c-122">Type</span></span>     | <span data-ttu-id="d045c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d045c-123">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d045c-124">id</span><span class="sxs-lookup"><span data-stu-id="d045c-124">id</span></span>                  | <span data-ttu-id="d045c-125">string</span><span class="sxs-lookup"><span data-stu-id="d045c-125">string</span></span>   | <span data-ttu-id="d045c-126">O aplicativo de catálogo gerados ID de aplicativo (diferente da identificação de fornecido pelo desenvolvedor no [pacote de aplicativos zip equipes da Microsoft](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="d045c-126">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d045c-127">externalId</span><span class="sxs-lookup"><span data-stu-id="d045c-127">externalId</span></span>          | <span data-ttu-id="d045c-128">string</span><span class="sxs-lookup"><span data-stu-id="d045c-128">string</span></span>   | <span data-ttu-id="d045c-129">A identificação do catálogo fornecido pelo desenvolvedor app nas [equipes da Microsoft zip o pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="d045c-129">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d045c-130">displayName</span><span class="sxs-lookup"><span data-stu-id="d045c-130">displayName</span></span>                | <span data-ttu-id="d045c-131">string</span><span class="sxs-lookup"><span data-stu-id="d045c-131">string</span></span>   | <span data-ttu-id="d045c-132">O nome do aplicativo catálogo fornecido pelo desenvolvedor app nas [equipes da Microsoft zip o pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span><span class="sxs-lookup"><span data-stu-id="d045c-132">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d045c-133">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="d045c-133">distributionMethod</span></span>  | <span data-ttu-id="d045c-134">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="d045c-134">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="d045c-135">O método de distribuição para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d045c-135">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="d045c-136">valores de teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="d045c-136">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="d045c-137">Membro</span><span class="sxs-lookup"><span data-stu-id="d045c-137">Member</span></span>|<span data-ttu-id="d045c-138">Valor</span><span class="sxs-lookup"><span data-stu-id="d045c-138">Value</span></span>|<span data-ttu-id="d045c-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="d045c-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d045c-140">repositório</span><span class="sxs-lookup"><span data-stu-id="d045c-140">store</span></span>|<span data-ttu-id="d045c-141">0</span><span class="sxs-lookup"><span data-stu-id="d045c-141">0</span></span>| <span data-ttu-id="d045c-142">O aplicativo está disponível para todos os locatários por meio da loja de app Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d045c-142">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="d045c-143">organization</span><span class="sxs-lookup"><span data-stu-id="d045c-143">organization</span></span>|<span data-ttu-id="d045c-144">1</span><span class="sxs-lookup"><span data-stu-id="d045c-144">1</span></span>|<span data-ttu-id="d045c-145">O aplicativo está disponível somente neste locatário.</span><span class="sxs-lookup"><span data-stu-id="d045c-145">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="d045c-146">sideloaded</span><span class="sxs-lookup"><span data-stu-id="d045c-146">sideloaded</span></span>|<span data-ttu-id="d045c-147">2</span><span class="sxs-lookup"><span data-stu-id="d045c-147">2</span></span>|<span data-ttu-id="d045c-148">O aplicativo está disponível somente para a equipe do usuário/seu instalados para.</span><span class="sxs-lookup"><span data-stu-id="d045c-148">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d045c-149">Relações</span><span class="sxs-lookup"><span data-stu-id="d045c-149">Relationships</span></span>

| <span data-ttu-id="d045c-150">Relação</span><span class="sxs-lookup"><span data-stu-id="d045c-150">Relationship</span></span> | <span data-ttu-id="d045c-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="d045c-151">Type</span></span>   | <span data-ttu-id="d045c-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="d045c-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d045c-153">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="d045c-153">appDefinitions</span></span>|<span data-ttu-id="d045c-154">coleção [teamsAppDefinition](teamsappdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d045c-154">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="d045c-155">Os detalhes de cada versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d045c-155">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d045c-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d045c-156">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="d045c-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="d045c-157">See also</span></span>

- [<span data-ttu-id="d045c-158">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d045c-158">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="d045c-159">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d045c-159">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="d045c-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d045c-160">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

