---
title: tipo de recurso governanceRoleSetting
description: " regra e assim por diante."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1bd1821bbb3336386b54b62ebe7b4787c85d1ebf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006420"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="9a562-103">tipo de recurso governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="9a562-103">governanceRoleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a562-104">Representa um conjunto de configurações em cada definição de função que precisam ser avaliadas quando as atribuições de função são criadas ou modificadas.</span><span class="sxs-lookup"><span data-stu-id="9a562-104">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="9a562-105">Por exemplo, as configurações de função podem incluir a regra "duração da atribuição máxima", regra "MFA necessária na ativação" e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="9a562-105">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="9a562-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9a562-106">Methods</span></span>

| <span data-ttu-id="9a562-107">Método</span><span class="sxs-lookup"><span data-stu-id="9a562-107">Method</span></span>          | <span data-ttu-id="9a562-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9a562-108">Return Type</span></span> |<span data-ttu-id="9a562-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a562-109">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="9a562-110">List</span><span class="sxs-lookup"><span data-stu-id="9a562-110">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="9a562-111">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="9a562-111">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="9a562-112">Lista uma coleção de configurações de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="9a562-112">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="9a562-113">Get</span><span class="sxs-lookup"><span data-stu-id="9a562-113">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="9a562-114">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="9a562-114">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="9a562-115">Leia as propriedades e as relações de uma configuração de função.</span><span class="sxs-lookup"><span data-stu-id="9a562-115">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="9a562-116">Atualização</span><span class="sxs-lookup"><span data-stu-id="9a562-116">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="9a562-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="9a562-117">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="9a562-118">Atualize um objeto de configuração de função.</span><span class="sxs-lookup"><span data-stu-id="9a562-118">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9a562-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a562-119">Properties</span></span>
|<span data-ttu-id="9a562-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a562-120">Property</span></span>               |<span data-ttu-id="9a562-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a562-121">Type</span></span>                                      |<span data-ttu-id="9a562-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a562-122">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="9a562-123">id</span><span class="sxs-lookup"><span data-stu-id="9a562-123">id</span></span>                   |<span data-ttu-id="9a562-124">String</span><span class="sxs-lookup"><span data-stu-id="9a562-124">String</span></span>                                  |<span data-ttu-id="9a562-125">A ID do roleSetting.</span><span class="sxs-lookup"><span data-stu-id="9a562-125">The id of the roleSetting.</span></span>|
|<span data-ttu-id="9a562-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="9a562-126">resourceId</span></span>           |<span data-ttu-id="9a562-127">String</span><span class="sxs-lookup"><span data-stu-id="9a562-127">String</span></span>                                  |<span data-ttu-id="9a562-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a562-128">Required.</span></span> <span data-ttu-id="9a562-129">A ID do recurso ao qual a configuração de função está associada.</span><span class="sxs-lookup"><span data-stu-id="9a562-129">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="9a562-130">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9a562-130">roleDefinitionId</span></span>     |<span data-ttu-id="9a562-131">String</span><span class="sxs-lookup"><span data-stu-id="9a562-131">String</span></span>                                  |<span data-ttu-id="9a562-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a562-132">Required.</span></span> <span data-ttu-id="9a562-133">A ID da definição de função à qual a configuração de função está associada.</span><span class="sxs-lookup"><span data-stu-id="9a562-133">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="9a562-134">isDefault</span><span class="sxs-lookup"><span data-stu-id="9a562-134">isDefault</span></span>            |<span data-ttu-id="9a562-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a562-135">Boolean</span></span>                                 |<span data-ttu-id="9a562-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a562-136">Read-only.</span></span> <span data-ttu-id="9a562-137">Indica se o roleSetting é um padrão roleSetting</span><span class="sxs-lookup"><span data-stu-id="9a562-137">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="9a562-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a562-138">lastUpdatedDateTime</span></span>  |<span data-ttu-id="9a562-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a562-139">DateTimeOffset</span></span>                          |<span data-ttu-id="9a562-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a562-140">Read-only.</span></span> <span data-ttu-id="9a562-141">A hora em que a configuração da função foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9a562-141">The time when the role setting was last updated.</span></span> <span data-ttu-id="9a562-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9a562-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9a562-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9a562-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9a562-144">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="9a562-144">lastUpdatedBy</span></span>        |<span data-ttu-id="9a562-145">String</span><span class="sxs-lookup"><span data-stu-id="9a562-145">String</span></span>                                  |<span data-ttu-id="9a562-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a562-146">Read-only.</span></span> <span data-ttu-id="9a562-147">O nome de exibição do administrador que atualizou pela última vez o roleSetting.</span><span class="sxs-lookup"><span data-stu-id="9a562-147">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="9a562-148">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="9a562-148">adminEligibleSettings</span></span>|<span data-ttu-id="9a562-149">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="9a562-149">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="9a562-150">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="9a562-150">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="9a562-151">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="9a562-151">adminMemberSettings</span></span>  |<span data-ttu-id="9a562-152">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="9a562-152">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="9a562-153">As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="9a562-153">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="9a562-154">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="9a562-154">userEligibleSettings</span></span> |<span data-ttu-id="9a562-155">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="9a562-155">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="9a562-156">As configurações de regra que são avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="9a562-156">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="9a562-157">A configuração não é suportada por enquanto.</span><span class="sxs-lookup"><span data-stu-id="9a562-157">The setting is not supported for now.</span></span>|
|<span data-ttu-id="9a562-158">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="9a562-158">userMemberSettings</span></span>   |<span data-ttu-id="9a562-159">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="9a562-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="9a562-160">As configurações de regra que são avaliadas quando um usuário tenta ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9a562-160">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a562-161">Relações</span><span class="sxs-lookup"><span data-stu-id="9a562-161">Relationships</span></span>
| <span data-ttu-id="9a562-162">Relação</span><span class="sxs-lookup"><span data-stu-id="9a562-162">Relationship</span></span> | <span data-ttu-id="9a562-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a562-163">Type</span></span>   |<span data-ttu-id="9a562-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a562-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a562-165">recurso</span><span class="sxs-lookup"><span data-stu-id="9a562-165">resource</span></span>|[<span data-ttu-id="9a562-166">Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="9a562-166">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="9a562-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a562-167">Read-only.</span></span> <span data-ttu-id="9a562-168">O recurso associado para esta configuração de função.</span><span class="sxs-lookup"><span data-stu-id="9a562-168">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="9a562-169">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9a562-169">roleDefinition</span></span>|[<span data-ttu-id="9a562-170">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9a562-170">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="9a562-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a562-171">Read-only.</span></span> <span data-ttu-id="9a562-172">A definição de função aplicada a essa configuração de função.</span><span class="sxs-lookup"><span data-stu-id="9a562-172">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9a562-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a562-173">JSON representation</span></span>

<span data-ttu-id="9a562-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a562-174">Here is a JSON representation of the resource.</span></span>

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
