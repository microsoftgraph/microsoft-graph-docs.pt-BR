# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="524db-101">tipo de recurso de teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="524db-101">teamsAppDefinition resource type</span></span>



<span data-ttu-id="524db-102">Os detalhes de uma versão de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="524db-102">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="524db-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="524db-103">Properties</span></span>

| <span data-ttu-id="524db-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="524db-104">Property</span></span>            | <span data-ttu-id="524db-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="524db-105">Type</span></span>     | <span data-ttu-id="524db-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="524db-106">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="524db-107">id</span><span class="sxs-lookup"><span data-stu-id="524db-107">id</span></span>                  | <span data-ttu-id="524db-108">string</span><span class="sxs-lookup"><span data-stu-id="524db-108">string</span></span>   | <span data-ttu-id="524db-109">Uma identificação exclusiva (não o appid equipes).</span><span class="sxs-lookup"><span data-stu-id="524db-109">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="524db-110">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="524db-110">teamsAppId</span></span>          | <span data-ttu-id="524db-111">string</span><span class="sxs-lookup"><span data-stu-id="524db-111">string</span></span>   | <span data-ttu-id="524db-112">A identificação de manifesto do aplicativo de equipes.</span><span class="sxs-lookup"><span data-stu-id="524db-112">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="524db-113">displayName</span><span class="sxs-lookup"><span data-stu-id="524db-113">displayName</span></span>         | <span data-ttu-id="524db-114">string</span><span class="sxs-lookup"><span data-stu-id="524db-114">string</span></span>   | <span data-ttu-id="524db-115">O nome do aplicativo fornecido pelo desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="524db-115">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="524db-116">version</span><span class="sxs-lookup"><span data-stu-id="524db-116">version</span></span>             | <span data-ttu-id="524db-117">string</span><span class="sxs-lookup"><span data-stu-id="524db-117">string</span></span>   | <span data-ttu-id="524db-118">O número de versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="524db-118">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="524db-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="524db-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a><span data-ttu-id="524db-120">Confira também</span><span class="sxs-lookup"><span data-stu-id="524db-120">See also</span></span>

- [<span data-ttu-id="524db-121">teamsApp</span><span class="sxs-lookup"><span data-stu-id="524db-121">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="524db-122">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="524db-122">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="524db-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="524db-123">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

