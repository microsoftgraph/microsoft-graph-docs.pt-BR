# <a name="outlookuser-resource-type"></a><span data-ttu-id="1d257-101">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="1d257-101">outlookUser resource type</span></span>


<span data-ttu-id="1d257-102">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="1d257-102">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="1d257-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="1d257-103">Methods</span></span>

| <span data-ttu-id="1d257-104">Método</span><span class="sxs-lookup"><span data-stu-id="1d257-104">Method</span></span>           | <span data-ttu-id="1d257-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1d257-105">Return Type</span></span>    |<span data-ttu-id="1d257-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d257-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d257-107">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="1d257-107">Create category</span></span>](../api/outlookuser_post_mastercategories.md) | [<span data-ttu-id="1d257-108">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="1d257-108">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="1d257-109">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="1d257-109">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="1d257-110">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="1d257-110">List categories</span></span>](../api/outlookuser_list_mastercategories.md) | <span data-ttu-id="1d257-111">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1d257-111">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="1d257-112">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="1d257-112">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="1d257-113">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="1d257-113">supportedLanguages</span></span>](../api/outlookuser_supportedlanguages.md) | <span data-ttu-id="1d257-114">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="1d257-114">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="1d257-115">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="1d257-115">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="1d257-116">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="1d257-116">supportedTimeZones</span></span>](../api/outlookuser_supportedtimezones.md) | <span data-ttu-id="1d257-117">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="1d257-117">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="1d257-118">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="1d257-118">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="1d257-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d257-119">Properties</span></span>
<span data-ttu-id="1d257-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d257-120">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1d257-121">Relações</span><span class="sxs-lookup"><span data-stu-id="1d257-121">Relationships</span></span>
| <span data-ttu-id="1d257-122">Relação</span><span class="sxs-lookup"><span data-stu-id="1d257-122">Relationship</span></span> | <span data-ttu-id="1d257-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d257-123">Type</span></span>   |<span data-ttu-id="1d257-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d257-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d257-125">masterCategories</span><span class="sxs-lookup"><span data-stu-id="1d257-125">masterCategories</span></span>|<span data-ttu-id="1d257-126">Coleção [outlookCategory](../resources/outlookCategory.md)</span><span class="sxs-lookup"><span data-stu-id="1d257-126">[outlookCategory](../resources/outlookCategory.md) collection</span></span>| <span data-ttu-id="1d257-127">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="1d257-127">A list of categories defined for the user.</span></span> | 

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookUser",
  "@odata.annotations": [
    {
      "property": "masterCategories",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->