---
title: Tipo de recurso unifiedRoleManagementPolicy
description: Um unifiedRoleManagementPolicy especifica as várias políticas associadas a um escopo e uma definição de função. Ele é derivado de microsoft.graph.policyBase.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7abeb69f469b9c8b7bec37b240c739774cbd8163
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679873"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a><span data-ttu-id="f1a22-104">Tipo de recurso unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="f1a22-104">unifiedRoleManagementPolicy resource type</span></span>

<span data-ttu-id="f1a22-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a22-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1a22-106">Um unifiedRoleManagementPolicy especifica as várias políticas associadas a um escopo e uma definição de função.</span><span class="sxs-lookup"><span data-stu-id="f1a22-106">A unifiedRoleManagementPolicy specifies the various policies associated with a scope and role definition.</span></span> <span data-ttu-id="f1a22-107">Ele é derivado de microsoft.graph.policyBase.</span><span class="sxs-lookup"><span data-stu-id="f1a22-107">It is derived from microsoft.graph.policyBase.</span></span>

## <a name="methods"></a><span data-ttu-id="f1a22-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f1a22-108">Methods</span></span>
|<span data-ttu-id="f1a22-109">Método</span><span class="sxs-lookup"><span data-stu-id="f1a22-109">Method</span></span>|<span data-ttu-id="f1a22-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f1a22-110">Return type</span></span>|<span data-ttu-id="f1a22-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1a22-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f1a22-112">Listar unifiedRoleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="f1a22-112">List unifiedRoleManagementPolicies</span></span>](../api/unifiedrolemanagementpolicy-list.md)|<span data-ttu-id="f1a22-113">[Coleção unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f1a22-113">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection</span></span>|<span data-ttu-id="f1a22-114">Obter uma lista dos [objetos unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f1a22-114">Get a list of the [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects and their properties.</span></span>|
|[<span data-ttu-id="f1a22-115">Obter unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="f1a22-115">Get unifiedRoleManagementPolicy</span></span>](../api/unifiedrolemanagementpolicy-get.md)|[<span data-ttu-id="f1a22-116">unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="f1a22-116">unifiedRoleManagementPolicy</span></span>](../resources/unifiedrolemanagementpolicy.md)|<span data-ttu-id="f1a22-117">Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicy.](../resources/unifiedrolemanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f1a22-117">Read the properties and relationships of an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object.</span></span>|
|[<span data-ttu-id="f1a22-118">Listar effectiveRules</span><span class="sxs-lookup"><span data-stu-id="f1a22-118">List effectiveRules</span></span>](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|<span data-ttu-id="f1a22-119">[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="f1a22-119">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="f1a22-120">Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação effectiveRules.</span><span class="sxs-lookup"><span data-stu-id="f1a22-120">Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.</span></span>|
|[<span data-ttu-id="f1a22-121">Listar regras</span><span class="sxs-lookup"><span data-stu-id="f1a22-121">List rules</span></span>](../api/unifiedrolemanagementpolicy-list-rules.md)|<span data-ttu-id="f1a22-122">[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="f1a22-122">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="f1a22-123">Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação de regras.</span><span class="sxs-lookup"><span data-stu-id="f1a22-123">Get the unifiedRoleManagementPolicyRule resources from the rules navigation property.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1a22-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1a22-124">Properties</span></span>
|<span data-ttu-id="f1a22-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1a22-125">Property</span></span>|<span data-ttu-id="f1a22-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1a22-126">Type</span></span>|<span data-ttu-id="f1a22-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1a22-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1a22-128">description</span><span class="sxs-lookup"><span data-stu-id="f1a22-128">description</span></span>|<span data-ttu-id="f1a22-129">String</span><span class="sxs-lookup"><span data-stu-id="f1a22-129">String</span></span>|<span data-ttu-id="f1a22-130">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="f1a22-130">Description for the policy.</span></span>|
|<span data-ttu-id="f1a22-131">displayName</span><span class="sxs-lookup"><span data-stu-id="f1a22-131">displayName</span></span>|<span data-ttu-id="f1a22-132">String</span><span class="sxs-lookup"><span data-stu-id="f1a22-132">String</span></span>|<span data-ttu-id="f1a22-133">Nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="f1a22-133">Display name for the policy.</span></span>|
|<span data-ttu-id="f1a22-134">id</span><span class="sxs-lookup"><span data-stu-id="f1a22-134">id</span></span>|<span data-ttu-id="f1a22-135">String</span><span class="sxs-lookup"><span data-stu-id="f1a22-135">String</span></span>|<span data-ttu-id="f1a22-136">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="f1a22-136">Unique identifier for the policy.</span></span>|
|<span data-ttu-id="f1a22-137">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="f1a22-137">isOrganizationDefault</span></span>|<span data-ttu-id="f1a22-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1a22-138">Boolean</span></span>|<span data-ttu-id="f1a22-139">Isso só pode ser definido como true para uma única política de toda a locatário que se aplicará a todos os escopos e funções.</span><span class="sxs-lookup"><span data-stu-id="f1a22-139">This can only be set to true for a single tenant wide policy which will apply to all scopes and roles.</span></span> <span data-ttu-id="f1a22-140">De definir o scopeId como "/" e scopeType como Directory.</span><span class="sxs-lookup"><span data-stu-id="f1a22-140">Set the scopeId to "/" and scopeType to Directory.</span></span>|
|<span data-ttu-id="f1a22-141">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f1a22-141">lastModifiedBy</span></span>|[<span data-ttu-id="f1a22-142">identity</span><span class="sxs-lookup"><span data-stu-id="f1a22-142">identity</span></span>](../resources/identity.md)|<span data-ttu-id="f1a22-143">A identidade que modificou a configuração da função pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f1a22-143">The identity who last modified the role setting.</span></span>|
|<span data-ttu-id="f1a22-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1a22-144">lastModifiedDateTime</span></span>|<span data-ttu-id="f1a22-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1a22-145">DateTimeOffset</span></span>|<span data-ttu-id="f1a22-146">A hora em que a configuração da função foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f1a22-146">The time when the role setting was last modified.</span></span>|
|<span data-ttu-id="f1a22-147">scopeId</span><span class="sxs-lookup"><span data-stu-id="f1a22-147">scopeId</span></span>|<span data-ttu-id="f1a22-148">String</span><span class="sxs-lookup"><span data-stu-id="f1a22-148">String</span></span>|<span data-ttu-id="f1a22-149">A id do escopo em que a política é criada.</span><span class="sxs-lookup"><span data-stu-id="f1a22-149">The id of the scope where the policy is created.</span></span> <span data-ttu-id="f1a22-150">Por exemplo</span><span class="sxs-lookup"><span data-stu-id="f1a22-150">E.g.</span></span> <span data-ttu-id="f1a22-151">"/", groupId, etc.</span><span class="sxs-lookup"><span data-stu-id="f1a22-151">"/", groupId, etc.</span></span>|
|<span data-ttu-id="f1a22-152">scopeType</span><span class="sxs-lookup"><span data-stu-id="f1a22-152">scopeType</span></span>|<span data-ttu-id="f1a22-153">String</span><span class="sxs-lookup"><span data-stu-id="f1a22-153">String</span></span>|<span data-ttu-id="f1a22-154">O tipo do escopo em que a política é criada.</span><span class="sxs-lookup"><span data-stu-id="f1a22-154">The type of the scope where the policy is created.</span></span> <span data-ttu-id="f1a22-155">Um de Directory, DirectoryRole, Group.</span><span class="sxs-lookup"><span data-stu-id="f1a22-155">One of Directory, DirectoryRole, Group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1a22-156">Relações</span><span class="sxs-lookup"><span data-stu-id="f1a22-156">Relationships</span></span>
|<span data-ttu-id="f1a22-157">Relação</span><span class="sxs-lookup"><span data-stu-id="f1a22-157">Relationship</span></span>|<span data-ttu-id="f1a22-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1a22-158">Type</span></span>|<span data-ttu-id="f1a22-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1a22-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1a22-160">effectiveRules</span><span class="sxs-lookup"><span data-stu-id="f1a22-160">effectiveRules</span></span>|<span data-ttu-id="f1a22-161">[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="f1a22-161">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="f1a22-162">A lista de regras efetivas, como regra de aprovação, regra de expiração, etc. avaliada com base em regras referenciadas herdadas.</span><span class="sxs-lookup"><span data-stu-id="f1a22-162">The list of effective rules like approval rule, expiration rule, etc. evaluated based on inherited referenced rules.</span></span> <span data-ttu-id="f1a22-163">Por exemplo</span><span class="sxs-lookup"><span data-stu-id="f1a22-163">E.g.</span></span> <span data-ttu-id="f1a22-164">Se houver uma política de todo o locatário para impor a regra de aprovação de habilitação, a regra efetiva será habilitar a aprovação, mesmo que a política tenha uma regra para desabilitar a aprovação.</span><span class="sxs-lookup"><span data-stu-id="f1a22-164">If there is a tenant wide policy to enforce enabling approval rule, the effective rule will be to enable approval even if the polcy has a rule to disable approval.</span></span>|
|<span data-ttu-id="f1a22-165">rules</span><span class="sxs-lookup"><span data-stu-id="f1a22-165">rules</span></span>|<span data-ttu-id="f1a22-166">[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="f1a22-166">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="f1a22-167">A coleção de regras, como regra de aprovação, regra de expiração, etc.</span><span class="sxs-lookup"><span data-stu-id="f1a22-167">The collection of rules like approval rule, expiration rule, etc.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1a22-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1a22-168">JSON representation</span></span>
<span data-ttu-id="f1a22-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1a22-169">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isOrganizationDefault": "Boolean",
  "scopeId": "String",
  "scopeType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

