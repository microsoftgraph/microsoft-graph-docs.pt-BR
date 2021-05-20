---
title: Tipo de recurso conditionalAccessPolicy
description: Representa uma Azure Active Directory de acesso condicional. As políticas de acesso condicional são regras personalizadas que definem um cenário de acesso.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2c64d0dc0c531437f000e9c2e36d1af51ddf204d
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547173"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="25be8-104">Tipo de recurso conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="25be8-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="25be8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25be8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25be8-106">Representa uma Azure Active Directory de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="25be8-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="25be8-107">As políticas de acesso condicional são regras personalizadas que definem um cenário de acesso.</span><span class="sxs-lookup"><span data-stu-id="25be8-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="25be8-108">Para obter mais informações, consulte [a documentação de acesso condicional](/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="25be8-108">For more information, see the [Conditional access documentation](/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="25be8-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="25be8-109">Methods</span></span>

| <span data-ttu-id="25be8-110">Método</span><span class="sxs-lookup"><span data-stu-id="25be8-110">Method</span></span>       | <span data-ttu-id="25be8-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="25be8-111">Return Type</span></span> | <span data-ttu-id="25be8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="25be8-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="25be8-113">Listar conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="25be8-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="25be8-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="25be8-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="25be8-115">Obter todos os objetos conditionalAccessPolicies na organização.</span><span class="sxs-lookup"><span data-stu-id="25be8-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="25be8-116">Criar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="25be8-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="25be8-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="25be8-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="25be8-118">Crie um novo objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="25be8-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="25be8-119">Obter conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="25be8-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="25be8-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="25be8-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="25be8-121">Ler propriedades e relações de um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="25be8-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="25be8-122">Atualizar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="25be8-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="25be8-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="25be8-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="25be8-124">Atualize um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="25be8-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="25be8-125">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="25be8-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="25be8-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25be8-126">None</span></span> | <span data-ttu-id="25be8-127">Exclua um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="25be8-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="25be8-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25be8-128">Properties</span></span>

| <span data-ttu-id="25be8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25be8-129">Property</span></span>     | <span data-ttu-id="25be8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="25be8-130">Type</span></span>        | <span data-ttu-id="25be8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="25be8-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="25be8-132">conditions</span><span class="sxs-lookup"><span data-stu-id="25be8-132">conditions</span></span>|[<span data-ttu-id="25be8-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="25be8-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="25be8-134">Especifica as regras que devem ser atendidas para que a política seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="25be8-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="25be8-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25be8-135">Required.</span></span> |
|<span data-ttu-id="25be8-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25be8-136">createdDateTime</span></span>|<span data-ttu-id="25be8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25be8-137">DateTimeOffset</span></span>| <span data-ttu-id="25be8-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="25be8-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25be8-139">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="25be8-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="25be8-140">Readonly.</span><span class="sxs-lookup"><span data-stu-id="25be8-140">Readonly.</span></span> |
|<span data-ttu-id="25be8-141">descrição</span><span class="sxs-lookup"><span data-stu-id="25be8-141">description</span></span>|<span data-ttu-id="25be8-142">String</span><span class="sxs-lookup"><span data-stu-id="25be8-142">String</span></span>| <span data-ttu-id="25be8-143">Não usado.</span><span class="sxs-lookup"><span data-stu-id="25be8-143">Not used.</span></span> |
|<span data-ttu-id="25be8-144">displayName</span><span class="sxs-lookup"><span data-stu-id="25be8-144">displayName</span></span>|<span data-ttu-id="25be8-145">String</span><span class="sxs-lookup"><span data-stu-id="25be8-145">String</span></span>| <span data-ttu-id="25be8-146">Especifica um nome de exibição para o objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="25be8-146">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="25be8-147">grantControls</span><span class="sxs-lookup"><span data-stu-id="25be8-147">grantControls</span></span>|[<span data-ttu-id="25be8-148">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="25be8-148">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="25be8-149">Especifica os controles de concessão que devem ser cumpridos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="25be8-149">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="25be8-150">id</span><span class="sxs-lookup"><span data-stu-id="25be8-150">id</span></span>|<span data-ttu-id="25be8-151">String</span><span class="sxs-lookup"><span data-stu-id="25be8-151">String</span></span>| <span data-ttu-id="25be8-152">Especifica o identificador de um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="25be8-152">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="25be8-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25be8-153">Read-only.</span></span>|
|<span data-ttu-id="25be8-154">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25be8-154">modifiedDateTime</span></span>| <span data-ttu-id="25be8-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25be8-155">DateTimeOffset</span></span>|<span data-ttu-id="25be8-156">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="25be8-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25be8-157">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="25be8-157">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="25be8-158">Readonly.</span><span class="sxs-lookup"><span data-stu-id="25be8-158">Readonly.</span></span> |
|<span data-ttu-id="25be8-159">sessionControls</span><span class="sxs-lookup"><span data-stu-id="25be8-159">sessionControls</span></span>|[<span data-ttu-id="25be8-160">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="25be8-160">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="25be8-161">Especifica os controles de sessão que são imposto após a assinatura.</span><span class="sxs-lookup"><span data-stu-id="25be8-161">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="25be8-162">state</span><span class="sxs-lookup"><span data-stu-id="25be8-162">state</span></span>|<span data-ttu-id="25be8-163">conditionalAccessPolicyState</span><span class="sxs-lookup"><span data-stu-id="25be8-163">conditionalAccessPolicyState</span></span>| <span data-ttu-id="25be8-164">Especifica o estado do objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="25be8-164">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="25be8-165">Os valores possíveis são: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="25be8-165">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="25be8-166">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25be8-166">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="25be8-167">Relações</span><span class="sxs-lookup"><span data-stu-id="25be8-167">Relationships</span></span>

<span data-ttu-id="25be8-168">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25be8-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25be8-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25be8-169">JSON representation</span></span>

<span data-ttu-id="25be8-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25be8-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "baseType":"microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
{
  "conditions": {"@odata.type": "microsoft.graph.conditionalAccessConditionSet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "grantControls": {"@odata.type": "microsoft.graph.conditionalAccessGrantControls"},
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)",
  "sessionControls": {"@odata.type": "microsoft.graph.conditionalAccessSessionControls"},
  "state": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
