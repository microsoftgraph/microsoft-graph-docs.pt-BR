---
title: tipo de recurso conditionalAccessPolicy
description: Representa uma política de acesso condicional do Azure Active Directory. As políticas de acesso condicional são regras personalizadas que definem um cenário do Access.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d8291bcd418af5549a8abb7dd30deebcdde9ed03
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636803"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="911f2-104">tipo de recurso conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="911f2-104">conditionalAccessPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="911f2-105">Representa uma política de acesso condicional do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="911f2-105">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="911f2-106">As políticas de acesso condicional são regras personalizadas que definem um cenário do Access.</span><span class="sxs-lookup"><span data-stu-id="911f2-106">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="911f2-107">Para obter mais informações, consulte a [documentação de acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="911f2-107">For more information, see the [Conditional access documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="911f2-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="911f2-108">Methods</span></span>

| <span data-ttu-id="911f2-109">Método</span><span class="sxs-lookup"><span data-stu-id="911f2-109">Method</span></span>       | <span data-ttu-id="911f2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="911f2-110">Return Type</span></span> | <span data-ttu-id="911f2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="911f2-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="911f2-112">Listar conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="911f2-112">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="911f2-113">[conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="911f2-113">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="911f2-114">Obter todos os objetos conditionalAccessPolicies na organização.</span><span class="sxs-lookup"><span data-stu-id="911f2-114">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="911f2-115">Criar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="911f2-115">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="911f2-116">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="911f2-116">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="911f2-117">Criar um novo objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="911f2-117">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="911f2-118">Obter conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="911f2-118">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="911f2-119">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="911f2-119">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="911f2-120">Ler propriedades e relações de um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="911f2-120">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="911f2-121">Atualizar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="911f2-121">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="911f2-122">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="911f2-122">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="911f2-123">Atualizar um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="911f2-123">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="911f2-124">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="911f2-124">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="911f2-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="911f2-125">None</span></span> | <span data-ttu-id="911f2-126">Excluir um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="911f2-126">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="911f2-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="911f2-127">Properties</span></span>

| <span data-ttu-id="911f2-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="911f2-128">Property</span></span>     | <span data-ttu-id="911f2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="911f2-129">Type</span></span>        | <span data-ttu-id="911f2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="911f2-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="911f2-131">conditions</span><span class="sxs-lookup"><span data-stu-id="911f2-131">conditions</span></span>|[<span data-ttu-id="911f2-132">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="911f2-132">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="911f2-133">Especifica as regras que devem ser atendidas para que a política seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="911f2-133">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="911f2-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="911f2-134">Required.</span></span> |
|<span data-ttu-id="911f2-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="911f2-135">createdDateTime</span></span>|<span data-ttu-id="911f2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="911f2-136">DateTimeOffset</span></span>| <span data-ttu-id="911f2-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="911f2-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="911f2-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="911f2-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="911f2-139">ReadOnly.</span><span class="sxs-lookup"><span data-stu-id="911f2-139">Readonly.</span></span> |
|<span data-ttu-id="911f2-140">description</span><span class="sxs-lookup"><span data-stu-id="911f2-140">description</span></span>|<span data-ttu-id="911f2-141">String</span><span class="sxs-lookup"><span data-stu-id="911f2-141">String</span></span>| <span data-ttu-id="911f2-142">Não usado.</span><span class="sxs-lookup"><span data-stu-id="911f2-142">Not used.</span></span> |
|<span data-ttu-id="911f2-143">displayName</span><span class="sxs-lookup"><span data-stu-id="911f2-143">displayName</span></span>|<span data-ttu-id="911f2-144">String</span><span class="sxs-lookup"><span data-stu-id="911f2-144">String</span></span>| <span data-ttu-id="911f2-145">Especifica um nome de exibição para o objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="911f2-145">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="911f2-146">grantControls</span><span class="sxs-lookup"><span data-stu-id="911f2-146">grantControls</span></span>|[<span data-ttu-id="911f2-147">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="911f2-147">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="911f2-148">Especifica os controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="911f2-148">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="911f2-149">id</span><span class="sxs-lookup"><span data-stu-id="911f2-149">id</span></span>|<span data-ttu-id="911f2-150">String</span><span class="sxs-lookup"><span data-stu-id="911f2-150">String</span></span>| <span data-ttu-id="911f2-151">Especifica o identificador de um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="911f2-151">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="911f2-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="911f2-152">Read-only.</span></span>|
|<span data-ttu-id="911f2-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="911f2-153">modifiedDateTime</span></span>| <span data-ttu-id="911f2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="911f2-154">DateTimeOffset</span></span>|<span data-ttu-id="911f2-155">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="911f2-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="911f2-156">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="911f2-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="911f2-157">ReadOnly.</span><span class="sxs-lookup"><span data-stu-id="911f2-157">Readonly.</span></span> |
|<span data-ttu-id="911f2-158">sessionControls</span><span class="sxs-lookup"><span data-stu-id="911f2-158">sessionControls</span></span>|[<span data-ttu-id="911f2-159">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="911f2-159">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="911f2-160">Especifica os controles de sessão que são aplicados após a entrada.</span><span class="sxs-lookup"><span data-stu-id="911f2-160">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="911f2-161">estado</span><span class="sxs-lookup"><span data-stu-id="911f2-161">state</span></span>|<span data-ttu-id="911f2-162">string</span><span class="sxs-lookup"><span data-stu-id="911f2-162">string</span></span>| <span data-ttu-id="911f2-163">Especifica o estado do objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="911f2-163">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="911f2-164">Os valores possíveis são: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="911f2-164">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="911f2-165">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="911f2-165">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="911f2-166">Relações</span><span class="sxs-lookup"><span data-stu-id="911f2-166">Relationships</span></span>

<span data-ttu-id="911f2-167">Nenhum</span><span class="sxs-lookup"><span data-stu-id="911f2-167">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="911f2-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="911f2-168">JSON representation</span></span>

<span data-ttu-id="911f2-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="911f2-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "baseType": "",
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
