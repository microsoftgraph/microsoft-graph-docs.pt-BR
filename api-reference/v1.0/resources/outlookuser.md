# <a name="outlookuser-resource-type"></a><span data-ttu-id="23224-101">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="23224-101">outlookUser resource type</span></span>


<span data-ttu-id="23224-102">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="23224-102">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="23224-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="23224-103">Methods</span></span>

| <span data-ttu-id="23224-104">Método</span><span class="sxs-lookup"><span data-stu-id="23224-104">Method</span></span>           | <span data-ttu-id="23224-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23224-105">Return Type</span></span>    |<span data-ttu-id="23224-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="23224-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23224-107">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="23224-107">Create category</span></span>](../api/outlookuser_post_mastercategories.md) | [<span data-ttu-id="23224-108">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="23224-108">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="23224-109">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="23224-109">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="23224-110">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="23224-110">List categories</span></span>](../api/outlookuser_list_mastercategories.md) | <span data-ttu-id="23224-111">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="23224-111">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="23224-112">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="23224-112">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="23224-113">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="23224-113">supportedLanguages</span></span>](../api/outlookuser_supportedlanguages.md) | <span data-ttu-id="23224-114">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="23224-114">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="23224-115">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="23224-115">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="23224-116">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="23224-116">supportedTimeZones</span></span>](../api/outlookuser_supportedtimezones.md) | <span data-ttu-id="23224-117">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="23224-117">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="23224-118">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="23224-118">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="23224-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23224-119">Properties</span></span>
<span data-ttu-id="23224-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="23224-120">None</span></span>

## <a name="relationships"></a><span data-ttu-id="23224-121">Relações</span><span class="sxs-lookup"><span data-stu-id="23224-121">Relationships</span></span>
| <span data-ttu-id="23224-122">Relação</span><span class="sxs-lookup"><span data-stu-id="23224-122">Relationship</span></span> | <span data-ttu-id="23224-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="23224-123">Type</span></span>   |<span data-ttu-id="23224-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="23224-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23224-125">masterCategories</span><span class="sxs-lookup"><span data-stu-id="23224-125">masterCategories</span></span>|<span data-ttu-id="23224-126">Coleção [outlookCategory](../resources/outlookCategory.md)</span><span class="sxs-lookup"><span data-stu-id="23224-126">[outlookCategory](../resources/outlookCategory.md) collection</span></span>| <span data-ttu-id="23224-127">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="23224-127">A list of categories defined for the user.</span></span> | 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->