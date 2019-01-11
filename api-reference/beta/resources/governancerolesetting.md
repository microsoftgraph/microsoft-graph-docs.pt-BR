---
title: tipo de recurso de governanceRoleSetting
description: " regra e assim por diante."
localization_priority: Normal
ms.openlocfilehash: d63685ae1a4383ce7ab245dda0fd7d1207c57f88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805884"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="1dcaf-103">tipo de recurso de governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="1dcaf-103">governanceRoleSetting resource type</span></span>

> <span data-ttu-id="1dcaf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dcaf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1dcaf-106">Representa um conjunto de configurações em cada definição de função que precisa ser avaliada quando as atribuições de função são criadas ou modificadas.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-106">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="1dcaf-107">Por exemplo, configurações de função podem incluir "Duração máxima de atribuição" regra, a regra "MFA necessários na ativação" e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-107">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="1dcaf-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="1dcaf-108">Methods</span></span>

| <span data-ttu-id="1dcaf-109">Método</span><span class="sxs-lookup"><span data-stu-id="1dcaf-109">Method</span></span>          | <span data-ttu-id="1dcaf-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1dcaf-110">Return Type</span></span> |<span data-ttu-id="1dcaf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dcaf-111">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="1dcaf-112">List</span><span class="sxs-lookup"><span data-stu-id="1dcaf-112">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="1dcaf-113">coleção [governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="1dcaf-113">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="1dcaf-114">Uma coleção de definições de função em um recurso de lista.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-114">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="1dcaf-115">Get</span><span class="sxs-lookup"><span data-stu-id="1dcaf-115">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="1dcaf-116">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="1dcaf-116">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="1dcaf-117">Leia as propriedades e os relacionamentos de uma configuração de função.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-117">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="1dcaf-118">Update</span><span class="sxs-lookup"><span data-stu-id="1dcaf-118">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="1dcaf-119">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="1dcaf-119">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="1dcaf-120">Atualize um objeto de configuração de função.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-120">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1dcaf-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1dcaf-121">Properties</span></span>
|<span data-ttu-id="1dcaf-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dcaf-122">Property</span></span>               |<span data-ttu-id="1dcaf-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dcaf-123">Type</span></span>                                      |<span data-ttu-id="1dcaf-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dcaf-124">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="1dcaf-125">id</span><span class="sxs-lookup"><span data-stu-id="1dcaf-125">id</span></span>                   |<span data-ttu-id="1dcaf-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dcaf-126">String</span></span>                                  |<span data-ttu-id="1dcaf-127">A identificação do roleSetting.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-127">The id of the roleSetting.</span></span>|
|<span data-ttu-id="1dcaf-128">resourceId</span><span class="sxs-lookup"><span data-stu-id="1dcaf-128">resourceId</span></span>           |<span data-ttu-id="1dcaf-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dcaf-129">String</span></span>                                  |<span data-ttu-id="1dcaf-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-130">Required.</span></span> <span data-ttu-id="1dcaf-131">A identificação do recurso que a configuração da função está associada.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-131">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="1dcaf-132">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1dcaf-132">roleDefinitionId</span></span>     |<span data-ttu-id="1dcaf-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dcaf-133">String</span></span>                                  |<span data-ttu-id="1dcaf-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-134">Required.</span></span> <span data-ttu-id="1dcaf-135">A id da definição de função que a configuração da função está associada.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-135">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="1dcaf-136">isDefault</span><span class="sxs-lookup"><span data-stu-id="1dcaf-136">isDefault</span></span>            |<span data-ttu-id="1dcaf-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="1dcaf-137">Boolean</span></span>                                 |<span data-ttu-id="1dcaf-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-138">Read-only.</span></span> <span data-ttu-id="1dcaf-139">Indique se o roleSetting é um roleSetting padrão</span><span class="sxs-lookup"><span data-stu-id="1dcaf-139">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="1dcaf-140">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dcaf-140">lastUpdatedDateTime</span></span>  |<span data-ttu-id="1dcaf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dcaf-141">DateTimeOffset</span></span>                          |<span data-ttu-id="1dcaf-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-142">Read-only.</span></span> <span data-ttu-id="1dcaf-143">A hora em que a configuração de funções foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-143">The time when the role setting was last updated.</span></span> <span data-ttu-id="1dcaf-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1dcaf-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1dcaf-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1dcaf-146">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="1dcaf-146">lastUpdatedBy</span></span>        |<span data-ttu-id="1dcaf-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1dcaf-147">String</span></span>                                  |<span data-ttu-id="1dcaf-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-148">Read-only.</span></span> <span data-ttu-id="1dcaf-149">O nome de exibição do administrador que atualizada pela última vez o roleSetting.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-149">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="1dcaf-150">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="1dcaf-150">adminEligibleSettings</span></span>|<span data-ttu-id="1dcaf-151">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="1dcaf-151">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="1dcaf-152">As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função elegíveis.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-152">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="1dcaf-153">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="1dcaf-153">adminMemberSettings</span></span>  |<span data-ttu-id="1dcaf-154">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="1dcaf-154">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="1dcaf-155">As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-155">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="1dcaf-156">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="1dcaf-156">userEligibleSettings</span></span> |<span data-ttu-id="1dcaf-157">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="1dcaf-157">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="1dcaf-158">As definições de regra que são avaliadas quando um usuário tentar adicionar uma atribuição de função elegíveis.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-158">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="1dcaf-159">A configuração não é suportada por enquanto.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-159">The setting is not supported for now.</span></span>|
|<span data-ttu-id="1dcaf-160">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="1dcaf-160">userMemberSettings</span></span>   |<span data-ttu-id="1dcaf-161">coleção [governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="1dcaf-161">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="1dcaf-162">As definições de regra que são avaliadas quando um usuário tentar ativar sua atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-162">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dcaf-163">Relações</span><span class="sxs-lookup"><span data-stu-id="1dcaf-163">Relationships</span></span>
| <span data-ttu-id="1dcaf-164">Relação</span><span class="sxs-lookup"><span data-stu-id="1dcaf-164">Relationship</span></span> | <span data-ttu-id="1dcaf-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dcaf-165">Type</span></span>   |<span data-ttu-id="1dcaf-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dcaf-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dcaf-167">recurso</span><span class="sxs-lookup"><span data-stu-id="1dcaf-167">resource</span></span>|[<span data-ttu-id="1dcaf-168">governanceResource</span><span class="sxs-lookup"><span data-stu-id="1dcaf-168">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="1dcaf-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-169">Read-only.</span></span> <span data-ttu-id="1dcaf-170">O recurso associado para esta definição de função.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-170">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="1dcaf-171">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="1dcaf-171">roleDefinition</span></span>|[<span data-ttu-id="1dcaf-172">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1dcaf-172">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="1dcaf-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-173">Read-only.</span></span> <span data-ttu-id="1dcaf-174">A definição de função que é imposta com essa definição de função.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-174">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1dcaf-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1dcaf-175">JSON representation</span></span>

<span data-ttu-id="1dcaf-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1dcaf-176">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
