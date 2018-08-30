# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="501cd-101">Tipo de recurso groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="501cd-101">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="501cd-102">Representa uma política de ciclo de vida de um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="501cd-102">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="501cd-103">Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos.</span><span class="sxs-lookup"><span data-stu-id="501cd-103">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="501cd-104">Por exemplo, após 180 dias o grupo expira.</span><span class="sxs-lookup"><span data-stu-id="501cd-104">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="501cd-105">Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="501cd-105">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="501cd-106">Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="501cd-106">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="501cd-107">Por exemplo, a nova validade do grupo é de 180 dias após a renovação.</span><span class="sxs-lookup"><span data-stu-id="501cd-107">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="501cd-108">Caso não seja renovado, ele expirará e será excluído.</span><span class="sxs-lookup"><span data-stu-id="501cd-108">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="501cd-109">É possível renovar o grupo no prazo de 30 dias da data de exclusão.</span><span class="sxs-lookup"><span data-stu-id="501cd-109">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="501cd-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="501cd-110">Methods</span></span>

| <span data-ttu-id="501cd-111">Método</span><span class="sxs-lookup"><span data-stu-id="501cd-111">Method</span></span> | <span data-ttu-id="501cd-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="501cd-112">Return Type</span></span> | <span data-ttu-id="501cd-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="501cd-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="501cd-114">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="501cd-114">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_get.md) | [<span data-ttu-id="501cd-115">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="501cd-115">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="501cd-116">Leia as propriedades e os relacionamentos de um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="501cd-116">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="501cd-117">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="501cd-117">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy_list.md) | <span data-ttu-id="501cd-118">Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="501cd-118">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="501cd-119">Listar todos os objetos groupLifecyclePolicies.</span><span class="sxs-lookup"><span data-stu-id="501cd-119">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="501cd-120">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="501cd-120">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_update.md) | [<span data-ttu-id="501cd-121">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="501cd-121">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="501cd-122">Atualizar um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="501cd-122">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="501cd-123">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="501cd-123">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_delete.md) | <span data-ttu-id="501cd-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="501cd-124">None</span></span> | <span data-ttu-id="501cd-125">Excluir um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="501cd-125">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="501cd-126">Adicionar um grupo a um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="501cd-126">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_addgroup.md)|<span data-ttu-id="501cd-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="501cd-127">None</span></span>| <span data-ttu-id="501cd-128">Adicionar um grupo a uma política de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="501cd-128">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="501cd-129">Remover um grupo de um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="501cd-129">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_removegroup.md)|<span data-ttu-id="501cd-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="501cd-130">None</span></span>| <span data-ttu-id="501cd-131">Remover um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="501cd-131">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="501cd-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="501cd-132">Properties</span></span>

| <span data-ttu-id="501cd-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="501cd-133">Property</span></span> | <span data-ttu-id="501cd-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="501cd-134">Type</span></span> | <span data-ttu-id="501cd-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="501cd-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="501cd-136">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="501cd-136">alternateNotificationEmails</span></span>|<span data-ttu-id="501cd-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="501cd-137">String</span></span>| <span data-ttu-id="501cd-138">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="501cd-138">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="501cd-139">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="501cd-139">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="501cd-140">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="501cd-140">groupLifetimeInDays</span></span>|<span data-ttu-id="501cd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="501cd-141">Int32</span></span>| <span data-ttu-id="501cd-142">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="501cd-142">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="501cd-143">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="501cd-143">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="501cd-144">id</span><span class="sxs-lookup"><span data-stu-id="501cd-144">id</span></span>|<span data-ttu-id="501cd-145">Guid</span><span class="sxs-lookup"><span data-stu-id="501cd-145">Guid</span></span>| <span data-ttu-id="501cd-146">Um identificador exclusivo de uma política.</span><span class="sxs-lookup"><span data-stu-id="501cd-146">A unique identifier for a policy.</span></span> <span data-ttu-id="501cd-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="501cd-147">Read-only.</span></span>|
|<span data-ttu-id="501cd-148">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="501cd-148">managedGroupTypes</span></span>|<span data-ttu-id="501cd-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="501cd-149">String</span></span>| <span data-ttu-id="501cd-150">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="501cd-150">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="501cd-151">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="501cd-151">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="501cd-152">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="501cd-152">Relationships</span></span>

<span data-ttu-id="501cd-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="501cd-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="501cd-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="501cd-154">JSON representation</span></span>

<span data-ttu-id="501cd-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="501cd-155">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->