---
title: Tipo de recurso continuousAccessEvaluationPolicy
description: A Avaliação de Acesso Contínuo (CAE) ajuda no gerenciamento de sessões de autenticação em tempo real. A CAE permite que os clientes manipularem o acesso a recursos suportando eventos de revogação instantânea.
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 58c4f913c8a5fc3b4f7c1c129c7126437035cbe7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444260"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a><span data-ttu-id="0e4c0-104">Tipo de recurso continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="0e4c0-104">continuousAccessEvaluationPolicy resource type</span></span>

<span data-ttu-id="0e4c0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e4c0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e4c0-106">A Avaliação de Acesso Contínuo (CAE) gerencia sessões de autenticação em tempo real.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-106">Continuous Access Evaluation (CAE) manages authentication sessions in real time.</span></span> <span data-ttu-id="0e4c0-107">A CAE permite que os clientes manipularem o acesso a recursos suportando eventos de revogação instantânea.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-107">CAE allows customers to handle access to resources by supporting instant revocation events.</span></span>  <span data-ttu-id="0e4c0-108">Para obter mais informações, consulte a avaliação [de acesso contínuo](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span><span class="sxs-lookup"><span data-stu-id="0e4c0-108">For more information, see the [Continuous access evaluation](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span></span>

## <a name="methods"></a><span data-ttu-id="0e4c0-109">Methods</span><span class="sxs-lookup"><span data-stu-id="0e4c0-109">Methods</span></span>
|<span data-ttu-id="0e4c0-110">Método</span><span class="sxs-lookup"><span data-stu-id="0e4c0-110">Method</span></span>|<span data-ttu-id="0e4c0-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0e4c0-111">Return type</span></span>|<span data-ttu-id="0e4c0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e4c0-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e4c0-113">Obter continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="0e4c0-113">Get continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-get.md)|[<span data-ttu-id="0e4c0-114">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="0e4c0-114">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="0e4c0-115">Leia as propriedades de [um objeto continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0e4c0-115">Read the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|[<span data-ttu-id="0e4c0-116">Atualizar continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="0e4c0-116">Update continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-update.md)|[<span data-ttu-id="0e4c0-117">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="0e4c0-117">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="0e4c0-118">Atualize as propriedades de [um objeto continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0e4c0-118">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|
## <a name="properties"></a><span data-ttu-id="0e4c0-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e4c0-119">Properties</span></span>
|<span data-ttu-id="0e4c0-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e4c0-120">Property</span></span>|<span data-ttu-id="0e4c0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e4c0-121">Type</span></span>|<span data-ttu-id="0e4c0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e4c0-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e4c0-123">description</span><span class="sxs-lookup"><span data-stu-id="0e4c0-123">description</span></span>|<span data-ttu-id="0e4c0-124">String</span><span class="sxs-lookup"><span data-stu-id="0e4c0-124">String</span></span>|<span data-ttu-id="0e4c0-125">A avaliação de acesso contínuo bloqueia automaticamente o acesso a recursos e aplicativos quase em tempo real quando o acesso de um usuário é removido ou um endereço IP do cliente muda.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-125">Continuous access evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.</span></span> <span data-ttu-id="0e4c0-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-126">Read-only.</span></span>|
|<span data-ttu-id="0e4c0-127">displayName</span><span class="sxs-lookup"><span data-stu-id="0e4c0-127">displayName</span></span>|<span data-ttu-id="0e4c0-128">String</span><span class="sxs-lookup"><span data-stu-id="0e4c0-128">String</span></span>| <span data-ttu-id="0e4c0-129">O valor é sempre "Avaliação de Acesso Contínuo".</span><span class="sxs-lookup"><span data-stu-id="0e4c0-129">The value is always 'Continuous Access Evaluation'.</span></span> <span data-ttu-id="0e4c0-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-130">Read-only.</span></span>|
|<span data-ttu-id="0e4c0-131">grupos</span><span class="sxs-lookup"><span data-stu-id="0e4c0-131">groups</span></span>|<span data-ttu-id="0e4c0-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e4c0-132">String collection</span></span>|<span data-ttu-id="0e4c0-133">A coleção de identificadores de grupo no escopo para avaliação.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-133">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="0e4c0-134">Todos os grupos estão no escopo quando a coleção está vazia.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-134">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="0e4c0-135">id</span><span class="sxs-lookup"><span data-stu-id="0e4c0-135">id</span></span>|<span data-ttu-id="0e4c0-136">String</span><span class="sxs-lookup"><span data-stu-id="0e4c0-136">String</span></span>|<span data-ttu-id="0e4c0-137">Especifica o identificador de um objeto continuousAccessEvaluationPolicy.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-137">Specifies the identifier of a continuousAccessEvaluationPolicy object.</span></span> <span data-ttu-id="0e4c0-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-138">Read-only.</span></span>|
|<span data-ttu-id="0e4c0-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0e4c0-139">isEnabled</span></span>|<span data-ttu-id="0e4c0-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="0e4c0-140">Boolean</span></span>| <span data-ttu-id="0e4c0-141">`true` para indicar se a avaliação de acesso contínuo deve ser realizada; caso `false` contrário.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="0e4c0-142">usuários</span><span class="sxs-lookup"><span data-stu-id="0e4c0-142">users</span></span>|<span data-ttu-id="0e4c0-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e4c0-143">String collection</span></span>|<span data-ttu-id="0e4c0-144">A coleção de identificadores de usuário no escopo para avaliação.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="0e4c0-145">Todos os usuários estão no escopo quando a coleção está vazia.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-145">All users are in scope when the collection is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e4c0-146">Relações</span><span class="sxs-lookup"><span data-stu-id="0e4c0-146">Relationships</span></span>
<span data-ttu-id="0e4c0-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e4c0-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e4c0-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e4c0-148">JSON representation</span></span>
<span data-ttu-id="0e4c0-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e4c0-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "users": [
    "String"
  ],
  "groups": [
    "String"
  ]
}
```
