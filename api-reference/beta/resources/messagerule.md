---
title: Tipo de recurso messageRule
description: Uma regra que se aplica a mensagens na Caixa de Entrada de um usuário.
author: angelgolfer-ms
ms.openlocfilehash: 1824e9a8d840da824efb79eff4b98bac02a8c187
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307725"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="e7cdb-103">Tipo de recurso messageRule</span><span class="sxs-lookup"><span data-stu-id="e7cdb-103">messageRule resource type</span></span>

> <span data-ttu-id="e7cdb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7cdb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7cdb-106">Uma regra que se aplica a mensagens na Caixa de Entrada de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-106">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="e7cdb-107">No Outlook, é possível configurar regras para mensagens recebidas na Caixa de Entrada, para realizar ações específicas em determinadas condições.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-107">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="e7cdb-108">Programaticamente, você pode acessar regras por meio da propriedade de navegação **messageRules** da [pasta](mailfolder.md) Caixa de Entrada.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-108">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="e7cdb-109">Cada regra é representada por esse recurso **messageRule**, as ações de regra disponíveis são representadas pelo tipo complexo [messageRuleActions](messageruleactions.md) e as condições e exceções de regra disponíveis são representadas pelo tipo complexo [messageRulePredicates](messagerulepredicates.md).</span><span class="sxs-lookup"><span data-stu-id="e7cdb-109">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="e7cdb-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7cdb-110">Properties</span></span>
| <span data-ttu-id="e7cdb-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7cdb-111">Property</span></span>     | <span data-ttu-id="e7cdb-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7cdb-112">Type</span></span>   |<span data-ttu-id="e7cdb-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7cdb-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e7cdb-114">actions</span><span class="sxs-lookup"><span data-stu-id="e7cdb-114">actions</span></span> | [<span data-ttu-id="e7cdb-115">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="e7cdb-115">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="e7cdb-116">Ações a serem realizadas em uma mensagem quando as condições correspondentes forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-116">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="e7cdb-117">conditions</span><span class="sxs-lookup"><span data-stu-id="e7cdb-117">conditions</span></span> | [<span data-ttu-id="e7cdb-118">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e7cdb-118">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="e7cdb-119">Condições que, quando atendidas, acionarão as ações correspondentes dessa regra.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-119">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="e7cdb-120">displayName</span><span class="sxs-lookup"><span data-stu-id="e7cdb-120">displayName</span></span> | <span data-ttu-id="e7cdb-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7cdb-121">String</span></span> | <span data-ttu-id="e7cdb-122">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-122">The display name of the rule.</span></span> |
| <span data-ttu-id="e7cdb-123">exceptions</span><span class="sxs-lookup"><span data-stu-id="e7cdb-123">exceptions</span></span> | [<span data-ttu-id="e7cdb-124">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e7cdb-124">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="e7cdb-125">Condições de exceção para a regra.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-125">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="e7cdb-126">hasError</span><span class="sxs-lookup"><span data-stu-id="e7cdb-126">hasError</span></span> | <span data-ttu-id="e7cdb-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7cdb-127">Boolean</span></span> | <span data-ttu-id="e7cdb-128">Indica se a regra está em uma condição de erro.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-128">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="e7cdb-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-129">Read-only.</span></span> |
| <span data-ttu-id="e7cdb-130">id</span><span class="sxs-lookup"><span data-stu-id="e7cdb-130">id</span></span> |<span data-ttu-id="e7cdb-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7cdb-131">String</span></span>|<span data-ttu-id="e7cdb-132">O identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-132">The unique identifier of the rule.</span></span> <span data-ttu-id="e7cdb-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-133">Read-only.</span></span>|
| <span data-ttu-id="e7cdb-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e7cdb-134">isEnabled</span></span> | <span data-ttu-id="e7cdb-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7cdb-135">Boolean</span></span> | <span data-ttu-id="e7cdb-136">Indica se a regra está habilitada para ser aplicada a mensagens.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-136">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="e7cdb-137">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="e7cdb-137">isReadOnly</span></span> | <span data-ttu-id="e7cdb-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7cdb-138">Boolean</span></span> | <span data-ttu-id="e7cdb-139">Indica se a regra é somente leitura e não pode ser modificada ou excluída pelas regras da API REST.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-139">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="e7cdb-140">sequence</span><span class="sxs-lookup"><span data-stu-id="e7cdb-140">sequence</span></span> | <span data-ttu-id="e7cdb-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e7cdb-141">Int32</span></span> | <span data-ttu-id="e7cdb-142">Indica a ordem em que a regra é executada, entre outras regras.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-142">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e7cdb-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7cdb-143">JSON representation</span></span>
<span data-ttu-id="e7cdb-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-144">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="e7cdb-145">Métodos</span><span class="sxs-lookup"><span data-stu-id="e7cdb-145">Methods</span></span>
| <span data-ttu-id="e7cdb-146">Método</span><span class="sxs-lookup"><span data-stu-id="e7cdb-146">Method</span></span>           | <span data-ttu-id="e7cdb-147">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e7cdb-147">Return Type</span></span>    |<span data-ttu-id="e7cdb-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7cdb-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7cdb-149">Listar regras</span><span class="sxs-lookup"><span data-stu-id="e7cdb-149">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="e7cdb-150">Coleção [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="e7cdb-150">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="e7cdb-151">Obtenha todos os objetos **messageRule** definidos para a Caixa de Entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-151">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="e7cdb-152">Obter regra</span><span class="sxs-lookup"><span data-stu-id="e7cdb-152">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="e7cdb-153">messageRule</span><span class="sxs-lookup"><span data-stu-id="e7cdb-153">messageRule</span></span>](messagerule.md) |<span data-ttu-id="e7cdb-154">Leia as propriedades e as relações de um objeto **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-154">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="e7cdb-155">Criar</span><span class="sxs-lookup"><span data-stu-id="e7cdb-155">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="e7cdb-156">messageRule</span><span class="sxs-lookup"><span data-stu-id="e7cdb-156">messageRule</span></span>](messagerule.md) |<span data-ttu-id="e7cdb-157">Crie um objeto **messageRule** especificando um conjunto de condições e ações.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-157">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="e7cdb-158">Atualizar</span><span class="sxs-lookup"><span data-stu-id="e7cdb-158">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="e7cdb-159">messageRule</span><span class="sxs-lookup"><span data-stu-id="e7cdb-159">messageRule</span></span>](messagerule.md) |<span data-ttu-id="e7cdb-160">Altere as propriedades graváveis em um objeto **messageRule** e salve as alterações.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-160">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="e7cdb-161">Excluir</span><span class="sxs-lookup"><span data-stu-id="e7cdb-161">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="e7cdb-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e7cdb-162">None</span></span> |<span data-ttu-id="e7cdb-163">Exclua o objeto **messageRule** especificado.</span><span class="sxs-lookup"><span data-stu-id="e7cdb-163">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->