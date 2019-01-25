---
title: tipo de recurso de governanceRoleSetting
description: " regra e assim por diante."
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508164"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="51ea7-103">tipo de recurso de governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="51ea7-103">governanceRoleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51ea7-104">Representa um conjunto de configurações em cada definição de função que precisa ser avaliada quando as atribuições de função são criadas ou modificadas.</span><span class="sxs-lookup"><span data-stu-id="51ea7-104">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="51ea7-105">Por exemplo, configurações de função podem incluir "Duração máxima de atribuição" regra, a regra "MFA necessários na ativação" e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="51ea7-105">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="51ea7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="51ea7-106">Methods</span></span>

| <span data-ttu-id="51ea7-107">Método</span><span class="sxs-lookup"><span data-stu-id="51ea7-107">Method</span></span>          | <span data-ttu-id="51ea7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="51ea7-108">Return Type</span></span> |<span data-ttu-id="51ea7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="51ea7-109">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="51ea7-110">List</span><span class="sxs-lookup"><span data-stu-id="51ea7-110">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="51ea7-111">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="51ea7-111">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="51ea7-112">Uma coleção de definições de função em um recurso de lista.</span><span class="sxs-lookup"><span data-stu-id="51ea7-112">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="51ea7-113">Get</span><span class="sxs-lookup"><span data-stu-id="51ea7-113">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="51ea7-114">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="51ea7-114">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="51ea7-115">Leia as propriedades e os relacionamentos de uma configuração de função.</span><span class="sxs-lookup"><span data-stu-id="51ea7-115">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="51ea7-116">Update</span><span class="sxs-lookup"><span data-stu-id="51ea7-116">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="51ea7-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="51ea7-117">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="51ea7-118">Atualize um objeto de configuração de função.</span><span class="sxs-lookup"><span data-stu-id="51ea7-118">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="51ea7-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51ea7-119">Properties</span></span>
|<span data-ttu-id="51ea7-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51ea7-120">Property</span></span>               |<span data-ttu-id="51ea7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="51ea7-121">Type</span></span>                                      |<span data-ttu-id="51ea7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="51ea7-122">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="51ea7-123">id</span><span class="sxs-lookup"><span data-stu-id="51ea7-123">id</span></span>                   |<span data-ttu-id="51ea7-124">String</span><span class="sxs-lookup"><span data-stu-id="51ea7-124">String</span></span>                                  |<span data-ttu-id="51ea7-125">A identificação do roleSetting.</span><span class="sxs-lookup"><span data-stu-id="51ea7-125">The id of the roleSetting.</span></span>|
|<span data-ttu-id="51ea7-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="51ea7-126">resourceId</span></span>           |<span data-ttu-id="51ea7-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51ea7-127">String</span></span>                                  |<span data-ttu-id="51ea7-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51ea7-128">Required.</span></span> <span data-ttu-id="51ea7-129">A identificação do recurso que a configuração da função está associada.</span><span class="sxs-lookup"><span data-stu-id="51ea7-129">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="51ea7-130">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="51ea7-130">roleDefinitionId</span></span>     |<span data-ttu-id="51ea7-131">String</span><span class="sxs-lookup"><span data-stu-id="51ea7-131">String</span></span>                                  |<span data-ttu-id="51ea7-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51ea7-132">Required.</span></span> <span data-ttu-id="51ea7-133">A id da definição de função que a configuração da função está associada.</span><span class="sxs-lookup"><span data-stu-id="51ea7-133">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="51ea7-134">isDefault</span><span class="sxs-lookup"><span data-stu-id="51ea7-134">isDefault</span></span>            |<span data-ttu-id="51ea7-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="51ea7-135">Boolean</span></span>                                 |<span data-ttu-id="51ea7-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51ea7-136">Read-only.</span></span> <span data-ttu-id="51ea7-137">Indique se o roleSetting é um roleSetting padrão</span><span class="sxs-lookup"><span data-stu-id="51ea7-137">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="51ea7-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="51ea7-138">lastUpdatedDateTime</span></span>  |<span data-ttu-id="51ea7-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51ea7-139">DateTimeOffset</span></span>                          |<span data-ttu-id="51ea7-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51ea7-140">Read-only.</span></span> <span data-ttu-id="51ea7-141">A hora em que a configuração de funções foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="51ea7-141">The time when the role setting was last updated.</span></span> <span data-ttu-id="51ea7-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="51ea7-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="51ea7-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="51ea7-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="51ea7-144">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="51ea7-144">lastUpdatedBy</span></span>        |<span data-ttu-id="51ea7-145">String</span><span class="sxs-lookup"><span data-stu-id="51ea7-145">String</span></span>                                  |<span data-ttu-id="51ea7-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51ea7-146">Read-only.</span></span> <span data-ttu-id="51ea7-147">O nome de exibição do administrador que atualizada pela última vez o roleSetting.</span><span class="sxs-lookup"><span data-stu-id="51ea7-147">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="51ea7-148">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="51ea7-148">adminEligibleSettings</span></span>|<span data-ttu-id="51ea7-149">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="51ea7-149">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="51ea7-150">As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função elegíveis.</span><span class="sxs-lookup"><span data-stu-id="51ea7-150">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="51ea7-151">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="51ea7-151">adminMemberSettings</span></span>  |<span data-ttu-id="51ea7-152">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="51ea7-152">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="51ea7-153">As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="51ea7-153">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="51ea7-154">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="51ea7-154">userEligibleSettings</span></span> |<span data-ttu-id="51ea7-155">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="51ea7-155">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="51ea7-156">As definições de regra que são avaliadas quando um usuário tentar adicionar uma atribuição de função elegíveis.</span><span class="sxs-lookup"><span data-stu-id="51ea7-156">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="51ea7-157">A configuração não é suportada por enquanto.</span><span class="sxs-lookup"><span data-stu-id="51ea7-157">The setting is not supported for now.</span></span>|
|<span data-ttu-id="51ea7-158">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="51ea7-158">userMemberSettings</span></span>   |<span data-ttu-id="51ea7-159">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="51ea7-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="51ea7-160">As definições de regra que são avaliadas quando um usuário tentar ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="51ea7-160">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51ea7-161">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="51ea7-161">Relationships</span></span>
| <span data-ttu-id="51ea7-162">Relação</span><span class="sxs-lookup"><span data-stu-id="51ea7-162">Relationship</span></span> | <span data-ttu-id="51ea7-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="51ea7-163">Type</span></span>   |<span data-ttu-id="51ea7-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="51ea7-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51ea7-165">recurso</span><span class="sxs-lookup"><span data-stu-id="51ea7-165">resource</span></span>|[<span data-ttu-id="51ea7-166">governanceResource</span><span class="sxs-lookup"><span data-stu-id="51ea7-166">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="51ea7-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51ea7-167">Read-only.</span></span> <span data-ttu-id="51ea7-168">O recurso associado para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="51ea7-168">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="51ea7-169">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="51ea7-169">roleDefinition</span></span>|[<span data-ttu-id="51ea7-170">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="51ea7-170">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="51ea7-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51ea7-171">Read-only.</span></span> <span data-ttu-id="51ea7-172">A definição de função que é imposta com essa definição de função.</span><span class="sxs-lookup"><span data-stu-id="51ea7-172">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51ea7-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51ea7-173">JSON representation</span></span>

<span data-ttu-id="51ea7-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51ea7-174">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerolesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
