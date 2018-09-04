# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="d8a05-101">tipo de recurso groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d8a05-101">groupSettingTemplate resource type</span></span>

<span data-ttu-id="d8a05-p101">Os modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário. As [configurações de grupo](groupsetting.md) podem ser criadas com base no **groupSettingTemplates** disponível e valores alterados de seus padrões predefinidos. Os modelos de configuração de grupo não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de nível de locatário ou configurações de grupo específico. Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office 365 e incluem as configurações, como se os usuários podem criar grupos ou convidar pessoas de fora da organização a se tornarem membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="d8a05-p101">Group setting templates represent system-defined settings available to the tenant. [Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults. Group setting templates cannot be created, updated or deleted. These settings can represent tenant-wide settings, or can represent specific group settings. Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="d8a05-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d8a05-107">Methods</span></span>

| <span data-ttu-id="d8a05-108">Método</span><span class="sxs-lookup"><span data-stu-id="d8a05-108">Method</span></span> | <span data-ttu-id="d8a05-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d8a05-109">Return Type</span></span> | <span data-ttu-id="d8a05-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8a05-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8a05-111">Obter groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d8a05-111">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate_get.md) | [<span data-ttu-id="d8a05-112">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d8a05-112">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="d8a05-113">Leia as propriedades específicas de um dos objetos groupSettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="d8a05-113">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="d8a05-114">Lista groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d8a05-114">List groupSettingTemplate</span></span>](../api/groupsettingtemplate_list.md) | [<span data-ttu-id="d8a05-115">Coleção de groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d8a05-115">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="d8a05-116">Lista todos os objetos de groupSettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="d8a05-116">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8a05-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8a05-117">Properties</span></span>

| <span data-ttu-id="d8a05-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8a05-118">Property</span></span> | <span data-ttu-id="d8a05-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8a05-119">Type</span></span> | <span data-ttu-id="d8a05-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8a05-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d8a05-121">descrição</span><span class="sxs-lookup"><span data-stu-id="d8a05-121">description</span></span>|<span data-ttu-id="d8a05-122">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8a05-122">String</span></span>| <span data-ttu-id="d8a05-123">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="d8a05-123">Description of the template.</span></span> |
|<span data-ttu-id="d8a05-124">displayName</span><span class="sxs-lookup"><span data-stu-id="d8a05-124">displayName</span></span>|<span data-ttu-id="d8a05-125">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8a05-125">String</span></span>| <span data-ttu-id="d8a05-126">Nome para exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="d8a05-126">Display name of the template.</span></span> |
|<span data-ttu-id="d8a05-127">id</span><span class="sxs-lookup"><span data-stu-id="d8a05-127">id</span></span>|<span data-ttu-id="d8a05-128">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8a05-128">String</span></span>| <span data-ttu-id="d8a05-p102">O identificador exclusivo do modelo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8a05-p102">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="d8a05-131">values</span><span class="sxs-lookup"><span data-stu-id="d8a05-131">values</span></span>|<span data-ttu-id="d8a05-132">Conjunto [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="d8a05-132">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="d8a05-133">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem este modelo.</span><span class="sxs-lookup"><span data-stu-id="d8a05-133">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d8a05-134">Relações</span><span class="sxs-lookup"><span data-stu-id="d8a05-134">Relationships</span></span>

<span data-ttu-id="d8a05-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8a05-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d8a05-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8a05-136">JSON representation</span></span>

<span data-ttu-id="d8a05-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8a05-137">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->