---
title: Tipo de recurso continuousAccessEvaluationPolicy
description: A Avaliação de Acesso Contínuo (CAE) ajuda no gerenciamento de sessões de autenticação em tempo real. A CAE permite que os clientes manipularem o acesso a recursos suportando eventos de revogação instantânea.
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f34fdacf75b991ff339f4b7cdd823290438e8fea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962634"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a><span data-ttu-id="499d8-104">Tipo de recurso continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="499d8-104">continuousAccessEvaluationPolicy resource type</span></span>

<span data-ttu-id="499d8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="499d8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="499d8-106">A Avaliação de Acesso Contínuo (CAE) gerencia sessões de autenticação em tempo real.</span><span class="sxs-lookup"><span data-stu-id="499d8-106">Continuous Access Evaluation (CAE) manages authentication sessions in real time.</span></span> <span data-ttu-id="499d8-107">A CAE permite que os clientes manipularem o acesso a recursos suportando eventos de revogação instantânea.</span><span class="sxs-lookup"><span data-stu-id="499d8-107">CAE allows customers to handle access to resources by supporting instant revocation events.</span></span>  <span data-ttu-id="499d8-108">Para obter mais informações, consulte a avaliação [de acesso contínuo](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span><span class="sxs-lookup"><span data-stu-id="499d8-108">For more information, see the [Continuous access evaluation](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span></span>

## <a name="methods"></a><span data-ttu-id="499d8-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="499d8-109">Methods</span></span>
|<span data-ttu-id="499d8-110">Método</span><span class="sxs-lookup"><span data-stu-id="499d8-110">Method</span></span>|<span data-ttu-id="499d8-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="499d8-111">Return type</span></span>|<span data-ttu-id="499d8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="499d8-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="499d8-113">Obter continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="499d8-113">Get continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-get.md)|[<span data-ttu-id="499d8-114">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="499d8-114">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="499d8-115">Leia as propriedades de [um objeto continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="499d8-115">Read the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|[<span data-ttu-id="499d8-116">Atualizar continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="499d8-116">Update continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-update.md)|[<span data-ttu-id="499d8-117">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="499d8-117">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="499d8-118">Atualize as propriedades de [um objeto continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="499d8-118">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|
## <a name="properties"></a><span data-ttu-id="499d8-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="499d8-119">Properties</span></span>
|<span data-ttu-id="499d8-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="499d8-120">Property</span></span>|<span data-ttu-id="499d8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="499d8-121">Type</span></span>|<span data-ttu-id="499d8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="499d8-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="499d8-123">description</span><span class="sxs-lookup"><span data-stu-id="499d8-123">description</span></span>|<span data-ttu-id="499d8-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="499d8-124">String</span></span>|<span data-ttu-id="499d8-125">A avaliação de acesso contínuo bloqueia automaticamente o acesso a recursos e aplicativos quase em tempo real quando o acesso de um usuário é removido ou um endereço IP do cliente muda.</span><span class="sxs-lookup"><span data-stu-id="499d8-125">Continuous access evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.</span></span> <span data-ttu-id="499d8-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="499d8-126">Read-only.</span></span>|
|<span data-ttu-id="499d8-127">displayName</span><span class="sxs-lookup"><span data-stu-id="499d8-127">displayName</span></span>|<span data-ttu-id="499d8-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="499d8-128">String</span></span>| <span data-ttu-id="499d8-129">O valor é sempre `Continuous Access Evaluation` .</span><span class="sxs-lookup"><span data-stu-id="499d8-129">The value is always `Continuous Access Evaluation`.</span></span> <span data-ttu-id="499d8-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="499d8-130">Read-only.</span></span>|
|<span data-ttu-id="499d8-131">grupos</span><span class="sxs-lookup"><span data-stu-id="499d8-131">groups</span></span>|<span data-ttu-id="499d8-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="499d8-132">String collection</span></span>|<span data-ttu-id="499d8-133">A coleção de identificadores de grupo no escopo para avaliação.</span><span class="sxs-lookup"><span data-stu-id="499d8-133">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="499d8-134">Todos os grupos estão no escopo quando a coleção está vazia.</span><span class="sxs-lookup"><span data-stu-id="499d8-134">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="499d8-135">id</span><span class="sxs-lookup"><span data-stu-id="499d8-135">id</span></span>|<span data-ttu-id="499d8-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="499d8-136">String</span></span>|<span data-ttu-id="499d8-137">Especifica o identificador de um [objeto continuousAccessEvaluationPolicy.](#continuousaccessevaluationpolicy-resource-type)</span><span class="sxs-lookup"><span data-stu-id="499d8-137">Specifies the identifier of a [continuousAccessEvaluationPolicy](#continuousaccessevaluationpolicy-resource-type) object.</span></span> <span data-ttu-id="499d8-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="499d8-138">Read-only.</span></span>|
|<span data-ttu-id="499d8-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="499d8-139">isEnabled</span></span>|<span data-ttu-id="499d8-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="499d8-140">Boolean</span></span>| <span data-ttu-id="499d8-141">`true` para indicar se a avaliação de acesso contínuo deve ser realizada; caso `false` contrário.</span><span class="sxs-lookup"><span data-stu-id="499d8-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="499d8-142">usuários</span><span class="sxs-lookup"><span data-stu-id="499d8-142">users</span></span>|<span data-ttu-id="499d8-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="499d8-143">String collection</span></span>|<span data-ttu-id="499d8-144">A coleção de identificadores de usuário no escopo para avaliação.</span><span class="sxs-lookup"><span data-stu-id="499d8-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="499d8-145">Todos os usuários estão no escopo quando a coleção está vazia.</span><span class="sxs-lookup"><span data-stu-id="499d8-145">All users are in scope when the collection is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="499d8-146">Relações</span><span class="sxs-lookup"><span data-stu-id="499d8-146">Relationships</span></span>
<span data-ttu-id="499d8-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="499d8-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="499d8-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="499d8-148">JSON representation</span></span>
<span data-ttu-id="499d8-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="499d8-149">The following is a JSON representation of the resource.</span></span>
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
