---
title: Tipo de recurso messageRule
description: Uma regra que se aplica a mensagens na Caixa de Entrada de um usuário.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6147640a221b72716f20bf4a90e74e25a7f9a448
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133760"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="10ed4-103">Tipo de recurso messageRule</span><span class="sxs-lookup"><span data-stu-id="10ed4-103">messageRule resource type</span></span>

<span data-ttu-id="10ed4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10ed4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10ed4-105">Uma regra que se aplica a mensagens na Caixa de Entrada de um usuário.</span><span class="sxs-lookup"><span data-stu-id="10ed4-105">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="10ed4-106">No Outlook, é possível configurar regras para mensagens recebidas na Caixa de Entrada, para realizar ações específicas em determinadas condições.</span><span class="sxs-lookup"><span data-stu-id="10ed4-106">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="10ed4-107">Programaticamente, você pode acessar regras por meio da propriedade de navegação **messageRules** da [pasta](mailfolder.md) Caixa de Entrada.</span><span class="sxs-lookup"><span data-stu-id="10ed4-107">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="10ed4-108">Cada regra é representada por esse recurso **messageRule**, as ações de regra disponíveis são representadas pelo tipo complexo [messageRuleActions](messageruleactions.md) e as condições e exceções de regra disponíveis são representadas pelo tipo complexo [messageRulePredicates](messagerulepredicates.md).</span><span class="sxs-lookup"><span data-stu-id="10ed4-108">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="10ed4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10ed4-109">Properties</span></span>
| <span data-ttu-id="10ed4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10ed4-110">Property</span></span>     | <span data-ttu-id="10ed4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="10ed4-111">Type</span></span>   |<span data-ttu-id="10ed4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="10ed4-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10ed4-113">actions</span><span class="sxs-lookup"><span data-stu-id="10ed4-113">actions</span></span> | [<span data-ttu-id="10ed4-114">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="10ed4-114">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="10ed4-115">Ações a serem realizadas em uma mensagem quando as condições correspondentes forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="10ed4-115">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="10ed4-116">conditions</span><span class="sxs-lookup"><span data-stu-id="10ed4-116">conditions</span></span> | [<span data-ttu-id="10ed4-117">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="10ed4-117">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="10ed4-118">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="10ed4-118">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="10ed4-119">displayName</span><span class="sxs-lookup"><span data-stu-id="10ed4-119">displayName</span></span> | <span data-ttu-id="10ed4-120">String</span><span class="sxs-lookup"><span data-stu-id="10ed4-120">String</span></span> | <span data-ttu-id="10ed4-121">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="10ed4-121">The display name of the rule.</span></span> |
| <span data-ttu-id="10ed4-122">exceptions</span><span class="sxs-lookup"><span data-stu-id="10ed4-122">exceptions</span></span> | [<span data-ttu-id="10ed4-123">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="10ed4-123">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="10ed4-124">Condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="10ed4-124">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="10ed4-125">hasError</span><span class="sxs-lookup"><span data-stu-id="10ed4-125">hasError</span></span> | <span data-ttu-id="10ed4-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="10ed4-126">Boolean</span></span> | <span data-ttu-id="10ed4-127">Indica se a regra está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="10ed4-127">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="10ed4-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10ed4-128">Read-only.</span></span> |
| <span data-ttu-id="10ed4-129">id</span><span class="sxs-lookup"><span data-stu-id="10ed4-129">id</span></span> |<span data-ttu-id="10ed4-130">String</span><span class="sxs-lookup"><span data-stu-id="10ed4-130">String</span></span>|<span data-ttu-id="10ed4-131">O identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="10ed4-131">The unique identifier of the rule.</span></span> <span data-ttu-id="10ed4-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10ed4-132">Read-only.</span></span>|
| <span data-ttu-id="10ed4-133">isEnabled</span><span class="sxs-lookup"><span data-stu-id="10ed4-133">isEnabled</span></span> | <span data-ttu-id="10ed4-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="10ed4-134">Boolean</span></span> | <span data-ttu-id="10ed4-135">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="10ed4-135">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="10ed4-136">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="10ed4-136">isReadOnly</span></span> | <span data-ttu-id="10ed4-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="10ed4-137">Boolean</span></span> | <span data-ttu-id="10ed4-138">Indica se a regra é somente leitura e não pode ser modificada ou excluída pelas regras da API REST.</span><span class="sxs-lookup"><span data-stu-id="10ed4-138">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="10ed4-139">sequence</span><span class="sxs-lookup"><span data-stu-id="10ed4-139">sequence</span></span> | <span data-ttu-id="10ed4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="10ed4-140">Int32</span></span> | <span data-ttu-id="10ed4-141">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="10ed4-141">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="10ed4-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10ed4-142">JSON representation</span></span>
<span data-ttu-id="10ed4-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10ed4-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
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

## <a name="methods"></a><span data-ttu-id="10ed4-144">Métodos</span><span class="sxs-lookup"><span data-stu-id="10ed4-144">Methods</span></span>
| <span data-ttu-id="10ed4-145">Método</span><span class="sxs-lookup"><span data-stu-id="10ed4-145">Method</span></span>           | <span data-ttu-id="10ed4-146">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="10ed4-146">Return Type</span></span>    |<span data-ttu-id="10ed4-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="10ed4-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="10ed4-148">Listar regras</span><span class="sxs-lookup"><span data-stu-id="10ed4-148">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="10ed4-149">Coleção [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="10ed4-149">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="10ed4-150">Obtenha todos os objetos **messageRule** definidos para a Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="10ed4-150">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="10ed4-151">Obter regra</span><span class="sxs-lookup"><span data-stu-id="10ed4-151">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="10ed4-152">messageRule</span><span class="sxs-lookup"><span data-stu-id="10ed4-152">messageRule</span></span>](messagerule.md) |<span data-ttu-id="10ed4-153">Leia as propriedades e as relações de um objeto **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="10ed4-153">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="10ed4-154">Criar</span><span class="sxs-lookup"><span data-stu-id="10ed4-154">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="10ed4-155">messageRule</span><span class="sxs-lookup"><span data-stu-id="10ed4-155">messageRule</span></span>](messagerule.md) |<span data-ttu-id="10ed4-156">Crie um objeto **messageRule** especificando um conjunto de condições e ações.</span><span class="sxs-lookup"><span data-stu-id="10ed4-156">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="10ed4-157">Atualizar</span><span class="sxs-lookup"><span data-stu-id="10ed4-157">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="10ed4-158">messageRule</span><span class="sxs-lookup"><span data-stu-id="10ed4-158">messageRule</span></span>](messagerule.md) |<span data-ttu-id="10ed4-159">Altere as propriedades graváveis em um objeto **messageRule** e salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="10ed4-159">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="10ed4-160">Delete</span><span class="sxs-lookup"><span data-stu-id="10ed4-160">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="10ed4-161">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="10ed4-161">None</span></span> |<span data-ttu-id="10ed4-162">Exclua o objeto **messageRule** especificado.</span><span class="sxs-lookup"><span data-stu-id="10ed4-162">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


