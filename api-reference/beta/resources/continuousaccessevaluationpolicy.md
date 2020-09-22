---
title: tipo de recurso continuousAccessEvaluationPolicy
description: A avaliação de acesso contínuo (CAE) ajuda no gerenciamento de sessões de autenticação em tempo real. O CAE permite que os clientes manipulem o acesso a recursos por meio do suporte a eventos de revogação instantânea.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a3027dea9a6c264b7af0ab805253946ebda8c97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023422"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a><span data-ttu-id="042ea-104">tipo de recurso continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="042ea-104">continuousAccessEvaluationPolicy resource type</span></span>

<span data-ttu-id="042ea-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="042ea-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="042ea-106">A avaliação de acesso contínuo (CAE) gerencia sessões de autenticação em tempo real.</span><span class="sxs-lookup"><span data-stu-id="042ea-106">Continuous Access Evaluation (CAE) manages authentication sessions in real time.</span></span> <span data-ttu-id="042ea-107">O CAE permite que os clientes manipulem o acesso a recursos por meio do suporte a eventos de revogação instantânea.</span><span class="sxs-lookup"><span data-stu-id="042ea-107">CAE allows customers to handle access to resources by supporting instant revocation events.</span></span>  <span data-ttu-id="042ea-108">Para obter mais informações, consulte a [avaliação de acesso contínuo](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span><span class="sxs-lookup"><span data-stu-id="042ea-108">For more information, see the [Continuous access evaluation](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span></span>

## <a name="methods"></a><span data-ttu-id="042ea-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="042ea-109">Methods</span></span>
|<span data-ttu-id="042ea-110">Método</span><span class="sxs-lookup"><span data-stu-id="042ea-110">Method</span></span>|<span data-ttu-id="042ea-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="042ea-111">Return type</span></span>|<span data-ttu-id="042ea-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="042ea-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="042ea-113">Obter continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="042ea-113">Get continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-get.md)|[<span data-ttu-id="042ea-114">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="042ea-114">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="042ea-115">Ler as propriedades de um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="042ea-115">Read the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|[<span data-ttu-id="042ea-116">Atualizar continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="042ea-116">Update continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-update.md)|[<span data-ttu-id="042ea-117">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="042ea-117">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="042ea-118">Atualiza as propriedades de um objeto [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="042ea-118">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|
## <a name="properties"></a><span data-ttu-id="042ea-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="042ea-119">Properties</span></span>
|<span data-ttu-id="042ea-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="042ea-120">Property</span></span>|<span data-ttu-id="042ea-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="042ea-121">Type</span></span>|<span data-ttu-id="042ea-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="042ea-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="042ea-123">description</span><span class="sxs-lookup"><span data-stu-id="042ea-123">description</span></span>|<span data-ttu-id="042ea-124">String</span><span class="sxs-lookup"><span data-stu-id="042ea-124">String</span></span>|<span data-ttu-id="042ea-125">A avaliação do acesso contínuo bloqueia automaticamente o acesso a recursos e aplicativos, quase em tempo real, quando o acesso de um usuário é removido ou um endereço IP do cliente é alterado.</span><span class="sxs-lookup"><span data-stu-id="042ea-125">Continuous access evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.</span></span> <span data-ttu-id="042ea-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="042ea-126">Read-only.</span></span>|
|<span data-ttu-id="042ea-127">displayName</span><span class="sxs-lookup"><span data-stu-id="042ea-127">displayName</span></span>|<span data-ttu-id="042ea-128">String</span><span class="sxs-lookup"><span data-stu-id="042ea-128">String</span></span>| <span data-ttu-id="042ea-129">O valor é sempre ' avaliação de acesso contínuo '.</span><span class="sxs-lookup"><span data-stu-id="042ea-129">The value is always 'Continuous Access Evaluation'.</span></span> <span data-ttu-id="042ea-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="042ea-130">Read-only.</span></span>|
|<span data-ttu-id="042ea-131">grupos</span><span class="sxs-lookup"><span data-stu-id="042ea-131">groups</span></span>|<span data-ttu-id="042ea-132">Coleção String</span><span class="sxs-lookup"><span data-stu-id="042ea-132">String collection</span></span>|<span data-ttu-id="042ea-133">A coleção de identificadores de grupo no escopo para avaliação.</span><span class="sxs-lookup"><span data-stu-id="042ea-133">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="042ea-134">Todos os grupos estão no escopo quando a coleção está vazia.</span><span class="sxs-lookup"><span data-stu-id="042ea-134">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="042ea-135">id</span><span class="sxs-lookup"><span data-stu-id="042ea-135">id</span></span>|<span data-ttu-id="042ea-136">String</span><span class="sxs-lookup"><span data-stu-id="042ea-136">String</span></span>|<span data-ttu-id="042ea-137">Especifica o identificador de um objeto continuousAccessEvaluationPolicy.</span><span class="sxs-lookup"><span data-stu-id="042ea-137">Specifies the identifier of a continuousAccessEvaluationPolicy object.</span></span> <span data-ttu-id="042ea-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="042ea-138">Read-only.</span></span>|
|<span data-ttu-id="042ea-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="042ea-139">isEnabled</span></span>|<span data-ttu-id="042ea-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="042ea-140">Boolean</span></span>| <span data-ttu-id="042ea-141">`true` para indicar se a avaliação de acesso contínuo deve ser executada; caso contrário `false` .</span><span class="sxs-lookup"><span data-stu-id="042ea-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="042ea-142">usuários</span><span class="sxs-lookup"><span data-stu-id="042ea-142">users</span></span>|<span data-ttu-id="042ea-143">Coleção String</span><span class="sxs-lookup"><span data-stu-id="042ea-143">String collection</span></span>|<span data-ttu-id="042ea-144">A coleção de identificadores de usuário no escopo para avaliação.</span><span class="sxs-lookup"><span data-stu-id="042ea-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="042ea-145">Todos os usuários estão no escopo quando a coleção está vazia.</span><span class="sxs-lookup"><span data-stu-id="042ea-145">All users are in scope when the collection is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="042ea-146">Relações</span><span class="sxs-lookup"><span data-stu-id="042ea-146">Relationships</span></span>
<span data-ttu-id="042ea-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="042ea-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="042ea-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="042ea-148">JSON representation</span></span>
<span data-ttu-id="042ea-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="042ea-149">The following is a JSON representation of the resource.</span></span>
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
