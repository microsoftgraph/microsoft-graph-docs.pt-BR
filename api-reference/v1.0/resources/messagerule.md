# <a name="messagerule-resource-type"></a><span data-ttu-id="23017-101">Tipo de recurso messageRule</span><span class="sxs-lookup"><span data-stu-id="23017-101">messageRule resource type</span></span>


<span data-ttu-id="23017-102">Uma regra que se aplica a mensagens na Caixa de Entrada de um usuário.</span><span class="sxs-lookup"><span data-stu-id="23017-102">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="23017-103">No Outlook, é possível configurar regras para mensagens recebidas na Caixa de Entrada, para realizar ações específicas em determinadas condições.</span><span class="sxs-lookup"><span data-stu-id="23017-103">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="23017-104">Programaticamente, você pode acessar regras por meio da propriedade de navegação **messageRules** da [pasta](mailfolder.md) Caixa de Entrada.</span><span class="sxs-lookup"><span data-stu-id="23017-104">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="23017-105">Cada regra é representada por esse recurso **messageRule**, as ações de regra disponíveis são representadas pelo tipo complexo [messageRuleActions](messageruleactions.md) e as condições e exceções de regra disponíveis são representadas pelo tipo complexo [messageRulePredicates](messagerulepredicates.md).</span><span class="sxs-lookup"><span data-stu-id="23017-105">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="23017-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23017-106">Properties</span></span>
| <span data-ttu-id="23017-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23017-107">Property</span></span>     | <span data-ttu-id="23017-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="23017-108">Type</span></span>   |<span data-ttu-id="23017-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="23017-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="23017-110">actions</span><span class="sxs-lookup"><span data-stu-id="23017-110">actions</span></span> | [<span data-ttu-id="23017-111">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="23017-111">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="23017-112">Ações a serem realizadas em uma mensagem quando as condições correspondentes forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="23017-112">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="23017-113">conditions</span><span class="sxs-lookup"><span data-stu-id="23017-113">conditions</span></span> | [<span data-ttu-id="23017-114">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="23017-114">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="23017-115">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="23017-115">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="23017-116">displayName</span><span class="sxs-lookup"><span data-stu-id="23017-116">displayName</span></span> | <span data-ttu-id="23017-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23017-117">String</span></span> | <span data-ttu-id="23017-118">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="23017-118">The display name of the rule.</span></span> |
| <span data-ttu-id="23017-119">exceptions</span><span class="sxs-lookup"><span data-stu-id="23017-119">exceptions</span></span> | [<span data-ttu-id="23017-120">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="23017-120">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="23017-121">Condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="23017-121">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="23017-122">hasError</span><span class="sxs-lookup"><span data-stu-id="23017-122">hasError</span></span> | <span data-ttu-id="23017-123">Booleano</span><span class="sxs-lookup"><span data-stu-id="23017-123">Boolean</span></span> | <span data-ttu-id="23017-124">Indica se a regra está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="23017-124">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="23017-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23017-125">Read-only.</span></span> |
| <span data-ttu-id="23017-126">id</span><span class="sxs-lookup"><span data-stu-id="23017-126">id</span></span> |<span data-ttu-id="23017-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23017-127">String</span></span>|<span data-ttu-id="23017-128">O identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="23017-128">The unique identifier of the rule.</span></span> <span data-ttu-id="23017-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23017-129">Read-only.</span></span>|
| <span data-ttu-id="23017-130">isEnabled</span><span class="sxs-lookup"><span data-stu-id="23017-130">isEnabled</span></span> | <span data-ttu-id="23017-131">Booleano</span><span class="sxs-lookup"><span data-stu-id="23017-131">Boolean</span></span> | <span data-ttu-id="23017-132">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="23017-132">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="23017-133">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="23017-133">isReadOnly</span></span> | <span data-ttu-id="23017-134">Booleano</span><span class="sxs-lookup"><span data-stu-id="23017-134">Boolean</span></span> | <span data-ttu-id="23017-135">Indica se a regra é somente leitura e não pode ser modificada ou excluída pelas regras da API REST.</span><span class="sxs-lookup"><span data-stu-id="23017-135">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="23017-136">sequence</span><span class="sxs-lookup"><span data-stu-id="23017-136">sequence</span></span> | <span data-ttu-id="23017-137">Int32</span><span class="sxs-lookup"><span data-stu-id="23017-137">Int32</span></span> | <span data-ttu-id="23017-138">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="23017-138">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="23017-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23017-139">JSON representation</span></span>
<span data-ttu-id="23017-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23017-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
   "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.messageRule"
}-->

```json
{
  "actions": {"@odata.type": "microsoft.graph.messageRuleActions"},
  "conditions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "displayName": "String",
  "exceptions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "hasError": "Boolean",
  "id": "String",
  "isEnabled": "Boolean",
  "isReadOnly": "Boolean",
  "sequence": "Int32"
}

```

## <a name="methods"></a><span data-ttu-id="23017-141">Métodos</span><span class="sxs-lookup"><span data-stu-id="23017-141">Methods</span></span>
| <span data-ttu-id="23017-142">Método</span><span class="sxs-lookup"><span data-stu-id="23017-142">Method</span></span>           | <span data-ttu-id="23017-143">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23017-143">Return Type</span></span>    |<span data-ttu-id="23017-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="23017-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23017-145">Listar regras</span><span class="sxs-lookup"><span data-stu-id="23017-145">List rules</span></span>](../api/mailfolder_list_messagerules.md) | <span data-ttu-id="23017-146">Coleção [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="23017-146">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="23017-147">Obtenha todos os objetos **messageRule** definidos para a Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="23017-147">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="23017-148">Obter regra</span><span class="sxs-lookup"><span data-stu-id="23017-148">Get rule</span></span>](../api/messagerule_get.md) | [<span data-ttu-id="23017-149">messageRule</span><span class="sxs-lookup"><span data-stu-id="23017-149">messageRule</span></span>](messagerule.md) |<span data-ttu-id="23017-150">Leia as propriedades e as relações de um objeto **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="23017-150">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="23017-151">Criar</span><span class="sxs-lookup"><span data-stu-id="23017-151">Create</span></span>](../api/mailfolder_post_messagerules.md) | [<span data-ttu-id="23017-152">messageRule</span><span class="sxs-lookup"><span data-stu-id="23017-152">messageRule</span></span>](messagerule.md) |<span data-ttu-id="23017-153">Crie um objeto **messageRule** especificando um conjunto de condições e ações.</span><span class="sxs-lookup"><span data-stu-id="23017-153">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="23017-154">Atualizar</span><span class="sxs-lookup"><span data-stu-id="23017-154">Update</span></span>](../api/messagerule_update.md) | [<span data-ttu-id="23017-155">messageRule</span><span class="sxs-lookup"><span data-stu-id="23017-155">messageRule</span></span>](messagerule.md) |<span data-ttu-id="23017-156">Altere as propriedades graváveis em um objeto **messageRule** e salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="23017-156">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="23017-157">Excluir</span><span class="sxs-lookup"><span data-stu-id="23017-157">Delete</span></span>](../api/messagerule_delete.md) | <span data-ttu-id="23017-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23017-158">None</span></span> |<span data-ttu-id="23017-159">Exclua o objeto **messageRule** especificado.</span><span class="sxs-lookup"><span data-stu-id="23017-159">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->