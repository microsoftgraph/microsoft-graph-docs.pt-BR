# <a name="groupsetting-resource-type"></a><span data-ttu-id="23ede-101">tipo de recurso groupSetting</span><span class="sxs-lookup"><span data-stu-id="23ede-101">groupSetting resource type</span></span>

<span data-ttu-id="23ede-102">As configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nomes de exibição de grupo ou se os usuários convidados podem ser proprietários de grupo.</span><span class="sxs-lookup"><span data-stu-id="23ede-102">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="23ede-p101">As configurações de grupo podem ser criadas com base no [groupSettingTemplates](groupSettingTemplate.md) disponível e alteradas de seus padrões predefinidos. Essas configurações regem os comportamentos de grupo em um nível total de locatários ou para um grupo específico. Quando a mesma configuração é definida no nível do locatário e para um grupo específico, a configuração de nível de grupo anula a configuração de nível de locatários.  Por exemplo, a configuração de nível de locatário pode permitir que os convidados sejam convidados por membros existentes dos grupos, mas uma configuração de grupo individual pode substitui-la e não permitir que os convidados sejam convidados por membros do grupo. As configurações de grupo regem apenas o comportamento dos grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="23ede-p101">Group settings can be created based on the available [groupSettingTemplates](groupSettingTemplate.md), and changed from their preset defaults. These settings govern group behaviors at a tenant-wide level or to a specific group. When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.  For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group. Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="23ede-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="23ede-108">Methods</span></span>

| <span data-ttu-id="23ede-109">Método</span><span class="sxs-lookup"><span data-stu-id="23ede-109">Method</span></span> | <span data-ttu-id="23ede-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23ede-110">Return Type</span></span> | <span data-ttu-id="23ede-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ede-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="23ede-112">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="23ede-112">Create setting</span></span>](../api/groupsetting_post_groupsettings.md) | [<span data-ttu-id="23ede-113">groupSetting</span><span class="sxs-lookup"><span data-stu-id="23ede-113">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="23ede-p102">Crie um objeto de configuração com base em um groupSettingTemplate. A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="23ede-p102">Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="23ede-116">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="23ede-116">Get setting</span></span>](../api/groupsetting_get.md) | [<span data-ttu-id="23ede-117">groupSetting</span><span class="sxs-lookup"><span data-stu-id="23ede-117">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="23ede-118">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="23ede-118">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="23ede-119">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="23ede-119">List settings</span></span>](../api/groupsetting_list.md) | <span data-ttu-id="23ede-120">Conjunto [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="23ede-120">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="23ede-121">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="23ede-121">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="23ede-122">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="23ede-122">Update setting</span></span>](../api/groupsetting_update.md) | [<span data-ttu-id="23ede-123">groupSetting</span><span class="sxs-lookup"><span data-stu-id="23ede-123">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="23ede-124">Atualize o objeto groupsetting.</span><span class="sxs-lookup"><span data-stu-id="23ede-124">Update groupsetting object.</span></span> |
|[<span data-ttu-id="23ede-125">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="23ede-125">Delete setting</span></span>](../api/groupsetting_delete.md) | <span data-ttu-id="23ede-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23ede-126">None</span></span> | <span data-ttu-id="23ede-127">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="23ede-127">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="23ede-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23ede-128">Properties</span></span>

| <span data-ttu-id="23ede-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23ede-129">Property</span></span> | <span data-ttu-id="23ede-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="23ede-130">Type</span></span> | <span data-ttu-id="23ede-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ede-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="23ede-132">displayName</span><span class="sxs-lookup"><span data-stu-id="23ede-132">displayName</span></span>|<span data-ttu-id="23ede-133">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="23ede-133">String</span></span>| <span data-ttu-id="23ede-134">Nome de exibição deste grupo de configurações, originado do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="23ede-134">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="23ede-135">id</span><span class="sxs-lookup"><span data-stu-id="23ede-135">id</span></span>|<span data-ttu-id="23ede-136">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="23ede-136">String</span></span>| <span data-ttu-id="23ede-p103">Identificador exclusivo destas configurações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23ede-p103">Unique identifier for these settings. Read-only.</span></span> |
|<span data-ttu-id="23ede-139">templateId</span><span class="sxs-lookup"><span data-stu-id="23ede-139">templateId</span></span>|<span data-ttu-id="23ede-140">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="23ede-140">String</span></span>| <span data-ttu-id="23ede-p104">Identificador exclusivo para o modelo usado para criar este grupo de configurações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23ede-p104">Unique identifier for the template used to create this group of settings. Read-only.</span></span> |
|<span data-ttu-id="23ede-143">values</span><span class="sxs-lookup"><span data-stu-id="23ede-143">values</span></span>|<span data-ttu-id="23ede-144">conjunto [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="23ede-144">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="23ede-p105">Conjunto de pares de nome/valor. Deve conter e ajustar todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="23ede-p105">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="23ede-147">Relações</span><span class="sxs-lookup"><span data-stu-id="23ede-147">Relationships</span></span>

<span data-ttu-id="23ede-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23ede-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23ede-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23ede-149">JSON representation</span></span>

<span data-ttu-id="23ede-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23ede-150">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->