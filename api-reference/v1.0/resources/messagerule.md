---
title: Tipo de recurso messageRule
description: Uma regra que se aplica a mensagens na Caixa de Entrada de um usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9f3ded6cb3fff7ac29968085e228549c32c5e2d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036117"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="96157-103">Tipo de recurso messageRule</span><span class="sxs-lookup"><span data-stu-id="96157-103">messageRule resource type</span></span>


<span data-ttu-id="96157-104">Uma regra que se aplica a mensagens na Caixa de Entrada de um usuário.</span><span class="sxs-lookup"><span data-stu-id="96157-104">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="96157-105">No Outlook, é possível configurar regras para mensagens recebidas na Caixa de Entrada, para realizar ações específicas em determinadas condições.</span><span class="sxs-lookup"><span data-stu-id="96157-105">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="96157-106">Programaticamente, você pode acessar regras por meio da propriedade de navegação **messageRules** da [pasta](mailfolder.md) Caixa de Entrada.</span><span class="sxs-lookup"><span data-stu-id="96157-106">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="96157-107">Cada regra é representada por esse recurso **messageRule**, as ações de regra disponíveis são representadas pelo tipo complexo [messageRuleActions](messageruleactions.md) e as condições e exceções de regra disponíveis são representadas pelo tipo complexo [messageRulePredicates](messagerulepredicates.md).</span><span class="sxs-lookup"><span data-stu-id="96157-107">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="96157-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96157-108">Properties</span></span>
| <span data-ttu-id="96157-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96157-109">Property</span></span>     | <span data-ttu-id="96157-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="96157-110">Type</span></span>   |<span data-ttu-id="96157-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="96157-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96157-112">actions</span><span class="sxs-lookup"><span data-stu-id="96157-112">actions</span></span> | [<span data-ttu-id="96157-113">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="96157-113">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="96157-114">Ações a serem realizadas em uma mensagem quando as condições correspondentes forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="96157-114">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="96157-115">conditions</span><span class="sxs-lookup"><span data-stu-id="96157-115">conditions</span></span> | [<span data-ttu-id="96157-116">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="96157-116">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="96157-117">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="96157-117">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="96157-118">displayName</span><span class="sxs-lookup"><span data-stu-id="96157-118">displayName</span></span> | <span data-ttu-id="96157-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96157-119">String</span></span> | <span data-ttu-id="96157-120">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="96157-120">The display name of the rule.</span></span> |
| <span data-ttu-id="96157-121">exceptions</span><span class="sxs-lookup"><span data-stu-id="96157-121">exceptions</span></span> | [<span data-ttu-id="96157-122">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="96157-122">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="96157-123">Condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="96157-123">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="96157-124">hasError</span><span class="sxs-lookup"><span data-stu-id="96157-124">hasError</span></span> | <span data-ttu-id="96157-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="96157-125">Boolean</span></span> | <span data-ttu-id="96157-126">Indica se a regra está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="96157-126">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="96157-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="96157-127">Read-only.</span></span> |
| <span data-ttu-id="96157-128">id</span><span class="sxs-lookup"><span data-stu-id="96157-128">id</span></span> |<span data-ttu-id="96157-129">String</span><span class="sxs-lookup"><span data-stu-id="96157-129">String</span></span>|<span data-ttu-id="96157-130">O identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="96157-130">The unique identifier of the rule.</span></span> <span data-ttu-id="96157-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="96157-131">Read-only.</span></span>|
| <span data-ttu-id="96157-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="96157-132">isEnabled</span></span> | <span data-ttu-id="96157-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="96157-133">Boolean</span></span> | <span data-ttu-id="96157-134">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="96157-134">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="96157-135">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="96157-135">isReadOnly</span></span> | <span data-ttu-id="96157-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="96157-136">Boolean</span></span> | <span data-ttu-id="96157-137">Indica se a regra é somente leitura e não pode ser modificada ou excluída pelas regras da API REST.</span><span class="sxs-lookup"><span data-stu-id="96157-137">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="96157-138">sequence</span><span class="sxs-lookup"><span data-stu-id="96157-138">sequence</span></span> | <span data-ttu-id="96157-139">Int32</span><span class="sxs-lookup"><span data-stu-id="96157-139">Int32</span></span> | <span data-ttu-id="96157-140">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="96157-140">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="96157-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96157-141">JSON representation</span></span>
<span data-ttu-id="96157-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96157-142">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="96157-143">Métodos</span><span class="sxs-lookup"><span data-stu-id="96157-143">Methods</span></span>
| <span data-ttu-id="96157-144">Método</span><span class="sxs-lookup"><span data-stu-id="96157-144">Method</span></span>           | <span data-ttu-id="96157-145">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="96157-145">Return Type</span></span>    |<span data-ttu-id="96157-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="96157-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96157-147">Listar regras</span><span class="sxs-lookup"><span data-stu-id="96157-147">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="96157-148">Coleção [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="96157-148">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="96157-149">Obtenha todos os objetos **messageRule** definidos para a Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="96157-149">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="96157-150">Obter regra</span><span class="sxs-lookup"><span data-stu-id="96157-150">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="96157-151">messageRule</span><span class="sxs-lookup"><span data-stu-id="96157-151">messageRule</span></span>](messagerule.md) |<span data-ttu-id="96157-152">Leia as propriedades e as relações de um objeto **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="96157-152">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="96157-153">Criar</span><span class="sxs-lookup"><span data-stu-id="96157-153">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="96157-154">messageRule</span><span class="sxs-lookup"><span data-stu-id="96157-154">messageRule</span></span>](messagerule.md) |<span data-ttu-id="96157-155">Crie um objeto **messageRule** especificando um conjunto de condições e ações.</span><span class="sxs-lookup"><span data-stu-id="96157-155">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="96157-156">Atualizar</span><span class="sxs-lookup"><span data-stu-id="96157-156">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="96157-157">messageRule</span><span class="sxs-lookup"><span data-stu-id="96157-157">messageRule</span></span>](messagerule.md) |<span data-ttu-id="96157-158">Altere as propriedades graváveis em um objeto **messageRule** e salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="96157-158">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="96157-159">Delete</span><span class="sxs-lookup"><span data-stu-id="96157-159">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="96157-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96157-160">None</span></span> |<span data-ttu-id="96157-161">Exclua o objeto **messageRule** especificado.</span><span class="sxs-lookup"><span data-stu-id="96157-161">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
