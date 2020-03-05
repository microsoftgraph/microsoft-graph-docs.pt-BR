---
title: tipo de recurso governanceRoleSetting
description: " regra e assim por diante."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9cf027969fb6ae988fd3e57da9d6c3002a4b4da9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497325"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="c1898-103">tipo de recurso governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="c1898-103">governanceRoleSetting resource type</span></span>

<span data-ttu-id="c1898-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c1898-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1898-105">Representa um conjunto de configurações em cada definição de função que precisam ser avaliadas quando as atribuições de função são criadas ou modificadas.</span><span class="sxs-lookup"><span data-stu-id="c1898-105">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="c1898-106">Por exemplo, as configurações de função podem incluir a regra "duração da atribuição máxima", regra "MFA necessária na ativação" e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="c1898-106">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="c1898-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c1898-107">Methods</span></span>

| <span data-ttu-id="c1898-108">Método</span><span class="sxs-lookup"><span data-stu-id="c1898-108">Method</span></span>          | <span data-ttu-id="c1898-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c1898-109">Return Type</span></span> |<span data-ttu-id="c1898-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1898-110">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="c1898-111">List</span><span class="sxs-lookup"><span data-stu-id="c1898-111">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="c1898-112">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="c1898-112">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="c1898-113">Lista uma coleção de configurações de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="c1898-113">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="c1898-114">Get</span><span class="sxs-lookup"><span data-stu-id="c1898-114">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="c1898-115">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="c1898-115">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="c1898-116">Leia as propriedades e as relações de uma configuração de função.</span><span class="sxs-lookup"><span data-stu-id="c1898-116">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="c1898-117">Update</span><span class="sxs-lookup"><span data-stu-id="c1898-117">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="c1898-118">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="c1898-118">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="c1898-119">Atualize um objeto de configuração de função.</span><span class="sxs-lookup"><span data-stu-id="c1898-119">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c1898-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1898-120">Properties</span></span>
|<span data-ttu-id="c1898-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1898-121">Property</span></span>               |<span data-ttu-id="c1898-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1898-122">Type</span></span>                                      |<span data-ttu-id="c1898-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1898-123">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="c1898-124">id</span><span class="sxs-lookup"><span data-stu-id="c1898-124">id</span></span>                   |<span data-ttu-id="c1898-125">String</span><span class="sxs-lookup"><span data-stu-id="c1898-125">String</span></span>                                  |<span data-ttu-id="c1898-126">A ID do roleSetting.</span><span class="sxs-lookup"><span data-stu-id="c1898-126">The id of the roleSetting.</span></span>|
|<span data-ttu-id="c1898-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="c1898-127">resourceId</span></span>           |<span data-ttu-id="c1898-128">String</span><span class="sxs-lookup"><span data-stu-id="c1898-128">String</span></span>                                  |<span data-ttu-id="c1898-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1898-129">Required.</span></span> <span data-ttu-id="c1898-130">A ID do recurso ao qual a configuração de função está associada.</span><span class="sxs-lookup"><span data-stu-id="c1898-130">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="c1898-131">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c1898-131">roleDefinitionId</span></span>     |<span data-ttu-id="c1898-132">String</span><span class="sxs-lookup"><span data-stu-id="c1898-132">String</span></span>                                  |<span data-ttu-id="c1898-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1898-133">Required.</span></span> <span data-ttu-id="c1898-134">A ID da definição de função à qual a configuração de função está associada.</span><span class="sxs-lookup"><span data-stu-id="c1898-134">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="c1898-135">isDefault</span><span class="sxs-lookup"><span data-stu-id="c1898-135">isDefault</span></span>            |<span data-ttu-id="c1898-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="c1898-136">Boolean</span></span>                                 |<span data-ttu-id="c1898-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1898-137">Read-only.</span></span> <span data-ttu-id="c1898-138">Indica se o roleSetting é um padrão roleSetting</span><span class="sxs-lookup"><span data-stu-id="c1898-138">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="c1898-139">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1898-139">lastUpdatedDateTime</span></span>  |<span data-ttu-id="c1898-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1898-140">DateTimeOffset</span></span>                          |<span data-ttu-id="c1898-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1898-141">Read-only.</span></span> <span data-ttu-id="c1898-142">A hora em que a configuração da função foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c1898-142">The time when the role setting was last updated.</span></span> <span data-ttu-id="c1898-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c1898-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c1898-144">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c1898-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c1898-145">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="c1898-145">lastUpdatedBy</span></span>        |<span data-ttu-id="c1898-146">String</span><span class="sxs-lookup"><span data-stu-id="c1898-146">String</span></span>                                  |<span data-ttu-id="c1898-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1898-147">Read-only.</span></span> <span data-ttu-id="c1898-148">O nome de exibição do administrador que atualizou pela última vez o roleSetting.</span><span class="sxs-lookup"><span data-stu-id="c1898-148">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="c1898-149">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="c1898-149">adminEligibleSettings</span></span>|<span data-ttu-id="c1898-150">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="c1898-150">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="c1898-151">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="c1898-151">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="c1898-152">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="c1898-152">adminMemberSettings</span></span>  |<span data-ttu-id="c1898-153">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="c1898-153">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="c1898-154">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="c1898-154">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="c1898-155">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="c1898-155">userEligibleSettings</span></span> |<span data-ttu-id="c1898-156">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="c1898-156">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="c1898-157">As configurações de regra que são avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="c1898-157">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="c1898-158">A configuração não é suportada por enquanto.</span><span class="sxs-lookup"><span data-stu-id="c1898-158">The setting is not supported for now.</span></span>|
|<span data-ttu-id="c1898-159">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="c1898-159">userMemberSettings</span></span>   |<span data-ttu-id="c1898-160">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="c1898-160">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="c1898-161">As configurações de regra que são avaliadas quando um usuário tenta ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c1898-161">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1898-162">Relações</span><span class="sxs-lookup"><span data-stu-id="c1898-162">Relationships</span></span>
| <span data-ttu-id="c1898-163">Relação</span><span class="sxs-lookup"><span data-stu-id="c1898-163">Relationship</span></span> | <span data-ttu-id="c1898-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1898-164">Type</span></span>   |<span data-ttu-id="c1898-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1898-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1898-166">recurso</span><span class="sxs-lookup"><span data-stu-id="c1898-166">resource</span></span>|[<span data-ttu-id="c1898-167">governanceResource</span><span class="sxs-lookup"><span data-stu-id="c1898-167">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="c1898-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1898-168">Read-only.</span></span> <span data-ttu-id="c1898-169">O recurso associado para esta configuração de função.</span><span class="sxs-lookup"><span data-stu-id="c1898-169">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="c1898-170">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c1898-170">roleDefinition</span></span>|[<span data-ttu-id="c1898-171">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c1898-171">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="c1898-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1898-172">Read-only.</span></span> <span data-ttu-id="c1898-173">A definição de função aplicada a essa configuração de função.</span><span class="sxs-lookup"><span data-stu-id="c1898-173">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c1898-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1898-174">JSON representation</span></span>

<span data-ttu-id="c1898-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1898-175">Here is a JSON representation of the resource.</span></span>

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
