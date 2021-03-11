---
title: Tipo de recurso governanceRoleSetting
description: Representa um conjunto de configurações em cada definição de função que precisa ser avaliada quando as atribuições de função são criadas ou modificadas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: cdc2889624dd9b23920c5cd04ed2c41344cb951c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722277"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="49439-103">Tipo de recurso governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="49439-103">governanceRoleSetting resource type</span></span>

<span data-ttu-id="49439-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49439-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49439-105">Representa um conjunto de configurações em cada definição de função que precisa ser avaliada quando as atribuições de função são criadas ou modificadas.</span><span class="sxs-lookup"><span data-stu-id="49439-105">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="49439-106">Por exemplo, as configurações de função podem incluir a regra "duração máxima da atribuição", a regra "MFA necessária na ativação" e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="49439-106">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="49439-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="49439-107">Methods</span></span>

| <span data-ttu-id="49439-108">Método</span><span class="sxs-lookup"><span data-stu-id="49439-108">Method</span></span>          | <span data-ttu-id="49439-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="49439-109">Return Type</span></span> |<span data-ttu-id="49439-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="49439-110">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="49439-111">List</span><span class="sxs-lookup"><span data-stu-id="49439-111">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="49439-112">[Coleção governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="49439-112">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="49439-113">Listar uma coleção de configurações de função em um recurso.</span><span class="sxs-lookup"><span data-stu-id="49439-113">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="49439-114">Get</span><span class="sxs-lookup"><span data-stu-id="49439-114">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="49439-115">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="49439-115">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="49439-116">Ler propriedades e relações de uma configuração de função.</span><span class="sxs-lookup"><span data-stu-id="49439-116">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="49439-117">Atualizar</span><span class="sxs-lookup"><span data-stu-id="49439-117">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="49439-118">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="49439-118">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="49439-119">Atualizar um objeto de configuração de função.</span><span class="sxs-lookup"><span data-stu-id="49439-119">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="49439-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49439-120">Properties</span></span>
|<span data-ttu-id="49439-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49439-121">Property</span></span>               |<span data-ttu-id="49439-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="49439-122">Type</span></span>                                      |<span data-ttu-id="49439-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="49439-123">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="49439-124">id</span><span class="sxs-lookup"><span data-stu-id="49439-124">id</span></span>                   |<span data-ttu-id="49439-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49439-125">String</span></span>                                  |<span data-ttu-id="49439-126">A id da roleSetting.</span><span class="sxs-lookup"><span data-stu-id="49439-126">The id of the roleSetting.</span></span>|
|<span data-ttu-id="49439-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="49439-127">resourceId</span></span>           |<span data-ttu-id="49439-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49439-128">String</span></span>                                  |<span data-ttu-id="49439-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49439-129">Required.</span></span> <span data-ttu-id="49439-130">A id do recurso ao que a configuração de função está associada.</span><span class="sxs-lookup"><span data-stu-id="49439-130">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="49439-131">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="49439-131">roleDefinitionId</span></span>     |<span data-ttu-id="49439-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49439-132">String</span></span>                                  |<span data-ttu-id="49439-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49439-133">Required.</span></span> <span data-ttu-id="49439-134">A id da definição de função à que a configuração de função está associada.</span><span class="sxs-lookup"><span data-stu-id="49439-134">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="49439-135">isDefault</span><span class="sxs-lookup"><span data-stu-id="49439-135">isDefault</span></span>            |<span data-ttu-id="49439-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="49439-136">Boolean</span></span>                                 |<span data-ttu-id="49439-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49439-137">Read-only.</span></span> <span data-ttu-id="49439-138">Indicar se roleSetting é uma roleSetting padrão</span><span class="sxs-lookup"><span data-stu-id="49439-138">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="49439-139">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="49439-139">lastUpdatedDateTime</span></span>  |<span data-ttu-id="49439-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49439-140">DateTimeOffset</span></span>                          |<span data-ttu-id="49439-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49439-141">Read-only.</span></span> <span data-ttu-id="49439-142">A hora em que a configuração de função foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="49439-142">The time when the role setting was last updated.</span></span> <span data-ttu-id="49439-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="49439-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="49439-144">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="49439-144">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="49439-145">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="49439-145">lastUpdatedBy</span></span>        |<span data-ttu-id="49439-146">String</span><span class="sxs-lookup"><span data-stu-id="49439-146">String</span></span>                                  |<span data-ttu-id="49439-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49439-147">Read-only.</span></span> <span data-ttu-id="49439-148">O nome de exibição do administrador que atualizou pela última vez a funçãoSetting.</span><span class="sxs-lookup"><span data-stu-id="49439-148">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="49439-149">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="49439-149">adminEligibleSettings</span></span>|<span data-ttu-id="49439-150">[Coleção governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="49439-150">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="49439-151">As configurações de regra avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="49439-151">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="49439-152">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="49439-152">adminMemberSettings</span></span>  |<span data-ttu-id="49439-153">[Coleção governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="49439-153">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="49439-154">As configurações de regra avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="49439-154">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="49439-155">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="49439-155">userEligibleSettings</span></span> |<span data-ttu-id="49439-156">[Coleção governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="49439-156">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="49439-157">As configurações de regra avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="49439-157">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="49439-158">A configuração não tem suporte por enquanto.</span><span class="sxs-lookup"><span data-stu-id="49439-158">The setting is not supported for now.</span></span>|
|<span data-ttu-id="49439-159">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="49439-159">userMemberSettings</span></span>   |<span data-ttu-id="49439-160">[Coleção governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="49439-160">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="49439-161">As configurações de regra avaliadas quando um usuário tenta ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="49439-161">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49439-162">Relações</span><span class="sxs-lookup"><span data-stu-id="49439-162">Relationships</span></span>
| <span data-ttu-id="49439-163">Relação</span><span class="sxs-lookup"><span data-stu-id="49439-163">Relationship</span></span> | <span data-ttu-id="49439-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="49439-164">Type</span></span>   |<span data-ttu-id="49439-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="49439-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49439-166">recurso</span><span class="sxs-lookup"><span data-stu-id="49439-166">resource</span></span>|[<span data-ttu-id="49439-167">governanceResource</span><span class="sxs-lookup"><span data-stu-id="49439-167">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="49439-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49439-168">Read-only.</span></span> <span data-ttu-id="49439-169">O recurso associado para essa configuração de função.</span><span class="sxs-lookup"><span data-stu-id="49439-169">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="49439-170">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="49439-170">roleDefinition</span></span>|[<span data-ttu-id="49439-171">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="49439-171">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="49439-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49439-172">Read-only.</span></span> <span data-ttu-id="49439-173">A definição de função que é imposta com essa configuração de função.</span><span class="sxs-lookup"><span data-stu-id="49439-173">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="49439-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49439-174">JSON representation</span></span>

<span data-ttu-id="49439-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49439-175">Here is a JSON representation of the resource.</span></span>

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


