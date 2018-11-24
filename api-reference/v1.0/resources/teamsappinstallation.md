# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="66641-101">tipo de recurso de teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="66641-101">teamsAppInstallation resource type</span></span>



<span data-ttu-id="66641-102">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="66641-102">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="66641-103">Qualquer bots que fazem parte do aplicativo se tornará parte de qualquer aplicativo é adicionado de equipe.</span><span class="sxs-lookup"><span data-stu-id="66641-103">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="66641-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="66641-104">Methods</span></span>

| <span data-ttu-id="66641-105">Método</span><span class="sxs-lookup"><span data-stu-id="66641-105">Method</span></span>       | <span data-ttu-id="66641-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="66641-106">Return Type</span></span>  |<span data-ttu-id="66641-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="66641-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="66641-108">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="66641-108">List apps</span></span>](../api/teamsappinstallation_list.md) | [<span data-ttu-id="66641-109">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="66641-109">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="66641-110">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="66641-110">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="66641-111">Adicionar aplicativo</span><span class="sxs-lookup"><span data-stu-id="66641-111">Add app</span></span>](../api/teamsappinstallation_add.md) | [<span data-ttu-id="66641-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="66641-112">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="66641-113">Adiciona (instala) um aplicativo para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="66641-113">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="66641-114">Remover aplicativo</span><span class="sxs-lookup"><span data-stu-id="66641-114">Remove app</span></span>](../api/teamsappinstallation_delete.md) | <span data-ttu-id="66641-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66641-115">None</span></span> | <span data-ttu-id="66641-116">Remove (desinstala) um aplicativo da equipe.</span><span class="sxs-lookup"><span data-stu-id="66641-116">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="66641-117">Atualizar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="66641-117">Upgrade app</span></span>](../api/teamsappinstallation_delete.md) | <span data-ttu-id="66641-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66641-118">None</span></span> | <span data-ttu-id="66641-119">Atualizações para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66641-119">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="66641-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66641-120">Properties</span></span>

| <span data-ttu-id="66641-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66641-121">Property</span></span>            | <span data-ttu-id="66641-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="66641-122">Type</span></span>     | <span data-ttu-id="66641-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="66641-123">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="66641-124">id</span><span class="sxs-lookup"><span data-stu-id="66641-124">id</span></span>                  | <span data-ttu-id="66641-125">string</span><span class="sxs-lookup"><span data-stu-id="66641-125">string</span></span>   | <span data-ttu-id="66641-126">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="66641-126">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="66641-127">Relações</span><span class="sxs-lookup"><span data-stu-id="66641-127">Relationships</span></span>

| <span data-ttu-id="66641-128">Relação</span><span class="sxs-lookup"><span data-stu-id="66641-128">Relationship</span></span>   | <span data-ttu-id="66641-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="66641-129">Type</span></span>    | <span data-ttu-id="66641-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="66641-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="66641-131">teamsApp</span><span class="sxs-lookup"><span data-stu-id="66641-131">teamsApp</span></span>|[<span data-ttu-id="66641-132">teamsApp</span><span class="sxs-lookup"><span data-stu-id="66641-132">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="66641-133">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="66641-133">The app that is installed.</span></span> |
|<span data-ttu-id="66641-134">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="66641-134">teamsAppDefinition</span></span>|[<span data-ttu-id="66641-135">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="66641-135">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="66641-136">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66641-136">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66641-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66641-137">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="66641-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="66641-138">See also</span></span>

- [<span data-ttu-id="66641-139">teamsApp</span><span class="sxs-lookup"><span data-stu-id="66641-139">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="66641-140">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="66641-140">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="66641-141">teamsTab</span><span class="sxs-lookup"><span data-stu-id="66641-141">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

