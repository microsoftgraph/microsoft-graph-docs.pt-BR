---
title: tipo de recurso conditionalAccessPolicy
description: Representa uma política de acesso condicional do Azure Active Directory. As políticas de acesso condicional são regras personalizadas que definem um cenário do Access.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b74360794ddad62a1cbda9b835f0490d447d8367
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384402"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="4387a-104">tipo de recurso conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="4387a-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="4387a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4387a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4387a-106">Representa uma política de acesso condicional do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4387a-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="4387a-107">As políticas de acesso condicional são regras personalizadas que definem um cenário do Access.</span><span class="sxs-lookup"><span data-stu-id="4387a-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="4387a-108">Para obter mais informações, consulte a [documentação de acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="4387a-108">For more information, see the [Conditional access documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="4387a-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="4387a-109">Methods</span></span>

| <span data-ttu-id="4387a-110">Método</span><span class="sxs-lookup"><span data-stu-id="4387a-110">Method</span></span>       | <span data-ttu-id="4387a-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4387a-111">Return Type</span></span> | <span data-ttu-id="4387a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4387a-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4387a-113">Listar conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="4387a-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="4387a-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="4387a-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="4387a-115">Obter todos os objetos conditionalAccessPolicies na organização.</span><span class="sxs-lookup"><span data-stu-id="4387a-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="4387a-116">Criar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="4387a-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="4387a-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="4387a-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="4387a-118">Criar um novo objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="4387a-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="4387a-119">Obter conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="4387a-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="4387a-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="4387a-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="4387a-121">Ler propriedades e relações de um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="4387a-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="4387a-122">Atualizar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="4387a-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="4387a-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="4387a-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="4387a-124">Atualizar um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="4387a-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="4387a-125">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="4387a-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="4387a-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4387a-126">None</span></span> | <span data-ttu-id="4387a-127">Excluir um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="4387a-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4387a-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4387a-128">Properties</span></span>

| <span data-ttu-id="4387a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4387a-129">Property</span></span>     | <span data-ttu-id="4387a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4387a-130">Type</span></span>        | <span data-ttu-id="4387a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4387a-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4387a-132">conditions</span><span class="sxs-lookup"><span data-stu-id="4387a-132">conditions</span></span>|[<span data-ttu-id="4387a-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="4387a-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="4387a-134">Especifica as regras que devem ser atendidas para que a política seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="4387a-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="4387a-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4387a-135">Required.</span></span> |
|<span data-ttu-id="4387a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4387a-136">createdDateTime</span></span>|<span data-ttu-id="4387a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4387a-137">DateTimeOffset</span></span>| <span data-ttu-id="4387a-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4387a-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4387a-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4387a-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4387a-140">ReadOnly.</span><span class="sxs-lookup"><span data-stu-id="4387a-140">Readonly.</span></span> |
|<span data-ttu-id="4387a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="4387a-141">displayName</span></span>|<span data-ttu-id="4387a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4387a-142">String</span></span>| <span data-ttu-id="4387a-143">Especifica um nome de exibição para o objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="4387a-143">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="4387a-144">grantControls</span><span class="sxs-lookup"><span data-stu-id="4387a-144">grantControls</span></span>|[<span data-ttu-id="4387a-145">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="4387a-145">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="4387a-146">Especifica os controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="4387a-146">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="4387a-147">id</span><span class="sxs-lookup"><span data-stu-id="4387a-147">id</span></span>|<span data-ttu-id="4387a-148">String</span><span class="sxs-lookup"><span data-stu-id="4387a-148">String</span></span>| <span data-ttu-id="4387a-149">Especifica o identificador de um objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="4387a-149">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="4387a-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4387a-150">Read-only.</span></span>|
|<span data-ttu-id="4387a-151">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4387a-151">modifiedDateTime</span></span>| <span data-ttu-id="4387a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4387a-152">DateTimeOffset</span></span>|<span data-ttu-id="4387a-153">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4387a-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4387a-154">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4387a-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4387a-155">ReadOnly.</span><span class="sxs-lookup"><span data-stu-id="4387a-155">Readonly.</span></span> |
|<span data-ttu-id="4387a-156">sessionControls</span><span class="sxs-lookup"><span data-stu-id="4387a-156">sessionControls</span></span>|[<span data-ttu-id="4387a-157">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="4387a-157">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="4387a-158">Especifica os controles de sessão que são aplicados após a entrada.</span><span class="sxs-lookup"><span data-stu-id="4387a-158">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="4387a-159">estado</span><span class="sxs-lookup"><span data-stu-id="4387a-159">state</span></span>|<span data-ttu-id="4387a-160">string</span><span class="sxs-lookup"><span data-stu-id="4387a-160">string</span></span>| <span data-ttu-id="4387a-161">Especifica o estado do objeto conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="4387a-161">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="4387a-162">Os valores possíveis são: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="4387a-162">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="4387a-163">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4387a-163">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4387a-164">Relações</span><span class="sxs-lookup"><span data-stu-id="4387a-164">Relationships</span></span>

<span data-ttu-id="4387a-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4387a-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4387a-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4387a-166">JSON representation</span></span>

<span data-ttu-id="4387a-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4387a-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
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
