---
title: tipo de recurso governanceRoleSetting
description: Representa um conjunto de configurações em cada definição de função que precisam ser avaliadas quando as atribuições de função são criadas ou modificadas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 61889ef9f5ecd968b52704138260d3b39ceaf961
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081640"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="bfe7d-103">tipo de recurso governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="bfe7d-103">governanceRoleSetting resource type</span></span>

<span data-ttu-id="bfe7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfe7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfe7d-105">Representa um conjunto de configurações em cada definição de função que precisam ser avaliadas quando as atribuições de função são criadas ou modificadas.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-105">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="bfe7d-106">Por exemplo, as configurações de função podem incluir a regra "duração da atribuição máxima", regra "MFA necessária na ativação" e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-106">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="bfe7d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="bfe7d-107">Methods</span></span>

| <span data-ttu-id="bfe7d-108">Método</span><span class="sxs-lookup"><span data-stu-id="bfe7d-108">Method</span></span>          | <span data-ttu-id="bfe7d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bfe7d-109">Return Type</span></span> |<span data-ttu-id="bfe7d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfe7d-110">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="bfe7d-111">List</span><span class="sxs-lookup"><span data-stu-id="bfe7d-111">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="bfe7d-112">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-112">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="bfe7d-113">Lista uma coleção de configurações de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-113">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="bfe7d-114">Get</span><span class="sxs-lookup"><span data-stu-id="bfe7d-114">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="bfe7d-115">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="bfe7d-115">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="bfe7d-116">Leia as propriedades e as relações de uma configuração de função.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-116">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="bfe7d-117">Update</span><span class="sxs-lookup"><span data-stu-id="bfe7d-117">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="bfe7d-118">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="bfe7d-118">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="bfe7d-119">Atualize um objeto de configuração de função.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-119">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bfe7d-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfe7d-120">Properties</span></span>
|<span data-ttu-id="bfe7d-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfe7d-121">Property</span></span>               |<span data-ttu-id="bfe7d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfe7d-122">Type</span></span>                                      |<span data-ttu-id="bfe7d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfe7d-123">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="bfe7d-124">id</span><span class="sxs-lookup"><span data-stu-id="bfe7d-124">id</span></span>                   |<span data-ttu-id="bfe7d-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfe7d-125">String</span></span>                                  |<span data-ttu-id="bfe7d-126">A ID do roleSetting.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-126">The id of the roleSetting.</span></span>|
|<span data-ttu-id="bfe7d-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="bfe7d-127">resourceId</span></span>           |<span data-ttu-id="bfe7d-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfe7d-128">String</span></span>                                  |<span data-ttu-id="bfe7d-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-129">Required.</span></span> <span data-ttu-id="bfe7d-130">A ID do recurso ao qual a configuração de função está associada.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-130">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="bfe7d-131">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="bfe7d-131">roleDefinitionId</span></span>     |<span data-ttu-id="bfe7d-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfe7d-132">String</span></span>                                  |<span data-ttu-id="bfe7d-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-133">Required.</span></span> <span data-ttu-id="bfe7d-134">A ID da definição de função à qual a configuração de função está associada.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-134">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="bfe7d-135">isDefault</span><span class="sxs-lookup"><span data-stu-id="bfe7d-135">isDefault</span></span>            |<span data-ttu-id="bfe7d-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="bfe7d-136">Boolean</span></span>                                 |<span data-ttu-id="bfe7d-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-137">Read-only.</span></span> <span data-ttu-id="bfe7d-138">Indica se o roleSetting é um padrão roleSetting</span><span class="sxs-lookup"><span data-stu-id="bfe7d-138">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="bfe7d-139">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfe7d-139">lastUpdatedDateTime</span></span>  |<span data-ttu-id="bfe7d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfe7d-140">DateTimeOffset</span></span>                          |<span data-ttu-id="bfe7d-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-141">Read-only.</span></span> <span data-ttu-id="bfe7d-142">A hora em que a configuração da função foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-142">The time when the role setting was last updated.</span></span> <span data-ttu-id="bfe7d-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bfe7d-144">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bfe7d-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bfe7d-145">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="bfe7d-145">lastUpdatedBy</span></span>        |<span data-ttu-id="bfe7d-146">String</span><span class="sxs-lookup"><span data-stu-id="bfe7d-146">String</span></span>                                  |<span data-ttu-id="bfe7d-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-147">Read-only.</span></span> <span data-ttu-id="bfe7d-148">O nome de exibição do administrador que atualizou pela última vez o roleSetting.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-148">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="bfe7d-149">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="bfe7d-149">adminEligibleSettings</span></span>|<span data-ttu-id="bfe7d-150">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-150">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bfe7d-151">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-151">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="bfe7d-152">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="bfe7d-152">adminMemberSettings</span></span>  |<span data-ttu-id="bfe7d-153">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-153">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bfe7d-154">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-154">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="bfe7d-155">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="bfe7d-155">userEligibleSettings</span></span> |<span data-ttu-id="bfe7d-156">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-156">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bfe7d-157">As configurações de regra que são avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-157">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="bfe7d-158">A configuração não é suportada por enquanto.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-158">The setting is not supported for now.</span></span>|
|<span data-ttu-id="bfe7d-159">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="bfe7d-159">userMemberSettings</span></span>   |<span data-ttu-id="bfe7d-160">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-160">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bfe7d-161">As configurações de regra que são avaliadas quando um usuário tenta ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-161">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfe7d-162">Relações</span><span class="sxs-lookup"><span data-stu-id="bfe7d-162">Relationships</span></span>
| <span data-ttu-id="bfe7d-163">Relação</span><span class="sxs-lookup"><span data-stu-id="bfe7d-163">Relationship</span></span> | <span data-ttu-id="bfe7d-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfe7d-164">Type</span></span>   |<span data-ttu-id="bfe7d-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfe7d-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfe7d-166">recurso</span><span class="sxs-lookup"><span data-stu-id="bfe7d-166">resource</span></span>|[<span data-ttu-id="bfe7d-167">governanceResource</span><span class="sxs-lookup"><span data-stu-id="bfe7d-167">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="bfe7d-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-168">Read-only.</span></span> <span data-ttu-id="bfe7d-169">O recurso associado para esta configuração de função.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-169">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="bfe7d-170">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="bfe7d-170">roleDefinition</span></span>|[<span data-ttu-id="bfe7d-171">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bfe7d-171">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="bfe7d-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-172">Read-only.</span></span> <span data-ttu-id="bfe7d-173">A definição de função aplicada a essa configuração de função.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-173">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bfe7d-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfe7d-174">JSON representation</span></span>

<span data-ttu-id="bfe7d-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-175">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


