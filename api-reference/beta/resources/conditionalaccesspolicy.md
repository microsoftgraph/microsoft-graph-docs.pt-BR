---
title: tipo de recurso conditionalAccessPolicy
description: Representa uma política de acesso condicional do Azure Active Directory. As políticas de acesso condicional são regras personalizadas que definem um cenário do Access.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 74270d2362bdfd6bbda567c17a45353eda7c319e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031730"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="446ff-104">tipo de recurso conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="446ff-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="446ff-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="446ff-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="446ff-106">Representa uma política de acesso condicional do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="446ff-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="446ff-107">As políticas de acesso condicional são regras personalizadas que definem um cenário do Access.</span><span class="sxs-lookup"><span data-stu-id="446ff-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="446ff-108">Para obter mais informações, consulte a [documentação de acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="446ff-108">For more information, see the [Conditional access documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="446ff-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="446ff-109">Methods</span></span>

| <span data-ttu-id="446ff-110">Método</span><span class="sxs-lookup"><span data-stu-id="446ff-110">Method</span></span>       | <span data-ttu-id="446ff-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="446ff-111">Return Type</span></span> | <span data-ttu-id="446ff-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="446ff-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="446ff-113">Listar conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="446ff-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="446ff-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="446ff-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="446ff-115">Obter todos os objetos conditionalAccessPolicies na organização.</span><span class="sxs-lookup"><span data-stu-id="446ff-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="446ff-116">Criar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="446ff-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="446ff-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="446ff-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="446ff-118">Criar um novo objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="446ff-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="446ff-119">Obter conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="446ff-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="446ff-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="446ff-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="446ff-121">Ler propriedades e relações de um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="446ff-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="446ff-122">Atualizar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="446ff-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="446ff-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="446ff-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="446ff-124">Atualizar um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="446ff-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="446ff-125">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="446ff-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="446ff-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="446ff-126">None</span></span> | <span data-ttu-id="446ff-127">Excluir um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="446ff-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="446ff-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="446ff-128">Properties</span></span>

| <span data-ttu-id="446ff-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="446ff-129">Property</span></span>     | <span data-ttu-id="446ff-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="446ff-130">Type</span></span>        | <span data-ttu-id="446ff-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="446ff-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="446ff-132">conditions</span><span class="sxs-lookup"><span data-stu-id="446ff-132">conditions</span></span>|[<span data-ttu-id="446ff-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="446ff-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="446ff-134">Especifica as regras que devem ser atendidas para que a política seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="446ff-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="446ff-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="446ff-135">Required.</span></span> |
|<span data-ttu-id="446ff-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="446ff-136">createdDateTime</span></span>|<span data-ttu-id="446ff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="446ff-137">DateTimeOffset</span></span>| <span data-ttu-id="446ff-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="446ff-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="446ff-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="446ff-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="446ff-140">ReadOnly.</span><span class="sxs-lookup"><span data-stu-id="446ff-140">Readonly.</span></span> |
|<span data-ttu-id="446ff-141">description</span><span class="sxs-lookup"><span data-stu-id="446ff-141">description</span></span>|<span data-ttu-id="446ff-142">String</span><span class="sxs-lookup"><span data-stu-id="446ff-142">String</span></span>| <span data-ttu-id="446ff-143">Não usado.</span><span class="sxs-lookup"><span data-stu-id="446ff-143">Not used.</span></span> |
|<span data-ttu-id="446ff-144">displayName</span><span class="sxs-lookup"><span data-stu-id="446ff-144">displayName</span></span>|<span data-ttu-id="446ff-145">String</span><span class="sxs-lookup"><span data-stu-id="446ff-145">String</span></span>| <span data-ttu-id="446ff-146">Especifica um nome de exibição para o objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="446ff-146">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="446ff-147">grantControls</span><span class="sxs-lookup"><span data-stu-id="446ff-147">grantControls</span></span>|[<span data-ttu-id="446ff-148">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="446ff-148">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="446ff-149">Especifica os controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="446ff-149">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="446ff-150">id</span><span class="sxs-lookup"><span data-stu-id="446ff-150">id</span></span>|<span data-ttu-id="446ff-151">String</span><span class="sxs-lookup"><span data-stu-id="446ff-151">String</span></span>| <span data-ttu-id="446ff-152">Especifica o identificador de um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="446ff-152">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="446ff-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="446ff-153">Read-only.</span></span>|
|<span data-ttu-id="446ff-154">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="446ff-154">modifiedDateTime</span></span>| <span data-ttu-id="446ff-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="446ff-155">DateTimeOffset</span></span>|<span data-ttu-id="446ff-156">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="446ff-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="446ff-157">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="446ff-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="446ff-158">ReadOnly.</span><span class="sxs-lookup"><span data-stu-id="446ff-158">Readonly.</span></span> |
|<span data-ttu-id="446ff-159">sessionControls</span><span class="sxs-lookup"><span data-stu-id="446ff-159">sessionControls</span></span>|[<span data-ttu-id="446ff-160">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="446ff-160">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="446ff-161">Especifica os controles de sessão que são aplicados após a entrada.</span><span class="sxs-lookup"><span data-stu-id="446ff-161">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="446ff-162">estado</span><span class="sxs-lookup"><span data-stu-id="446ff-162">state</span></span>|<span data-ttu-id="446ff-163">string</span><span class="sxs-lookup"><span data-stu-id="446ff-163">string</span></span>| <span data-ttu-id="446ff-164">Especifica o estado do objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="446ff-164">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="446ff-165">Os valores possíveis são: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="446ff-165">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="446ff-166">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="446ff-166">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="446ff-167">Relações</span><span class="sxs-lookup"><span data-stu-id="446ff-167">Relationships</span></span>

<span data-ttu-id="446ff-168">Nenhum</span><span class="sxs-lookup"><span data-stu-id="446ff-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="446ff-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="446ff-169">JSON representation</span></span>

<span data-ttu-id="446ff-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="446ff-170">The following is a JSON representation of the resource.</span></span>

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


