---
title: Tipo de recurso conditionalAccessPolicyCoverage
description: Representa informações sobre qualquer política Azure Active Directory que define regras de acesso de um recurso para um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a4bc4f336692166ff032727a6fb13222edd9d7d9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401943"
---
# <a name="conditionalaccesspolicycoverage-resource-type"></a><span data-ttu-id="748f1-103">Tipo de recurso conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="748f1-103">conditionalAccessPolicyCoverage resource type</span></span>

<span data-ttu-id="748f1-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="748f1-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="748f1-105">Representa informações sobre qualquer política Azure Active Directory que define regras de acesso de um recurso para um determinado locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="748f1-105">Represents information about any Azure Active Directory policy that defines access rules of a resource for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="748f1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="748f1-106">Methods</span></span>
|<span data-ttu-id="748f1-107">Método</span><span class="sxs-lookup"><span data-stu-id="748f1-107">Method</span></span>|<span data-ttu-id="748f1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="748f1-108">Return type</span></span>|<span data-ttu-id="748f1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="748f1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="748f1-110">Listar conditionalAccessPolicyCoverages</span><span class="sxs-lookup"><span data-stu-id="748f1-110">List conditionalAccessPolicyCoverages</span></span>](../api/managedtenants-managedtenant-list-conditionalaccesspolicycoverages.md)|<span data-ttu-id="748f1-111">[coleção microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)</span><span class="sxs-lookup"><span data-stu-id="748f1-111">[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) collection</span></span>|<span data-ttu-id="748f1-112">Obter uma lista dos [objetos conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="748f1-112">Get a list of the [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects and their properties.</span></span>|
|[<span data-ttu-id="748f1-113">Obter conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="748f1-113">Get conditionalAccessPolicyCoverage</span></span>](../api/managedtenants-conditionalaccesspolicycoverage-get.md)|[<span data-ttu-id="748f1-114">microsoft.graph.managedTenants.conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="748f1-114">microsoft.graph.managedTenants.conditionalAccessPolicyCoverage</span></span>](../resources/managedtenants-conditionalaccesspolicycoverage.md)|<span data-ttu-id="748f1-115">Leia as propriedades e as relações de [um objeto conditionalAccessPolicyCoverage.](../resources/managedtenants-conditionalaccesspolicycoverage.md)</span><span class="sxs-lookup"><span data-stu-id="748f1-115">Read the properties and relationships of a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="748f1-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="748f1-116">Properties</span></span>
|<span data-ttu-id="748f1-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="748f1-117">Property</span></span>|<span data-ttu-id="748f1-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="748f1-118">Type</span></span>|<span data-ttu-id="748f1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="748f1-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="748f1-120">conditionalAccessPolicyState</span><span class="sxs-lookup"><span data-stu-id="748f1-120">conditionalAccessPolicyState</span></span>|<span data-ttu-id="748f1-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="748f1-121">String</span></span>|<span data-ttu-id="748f1-122">O estado da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="748f1-122">The state for the conditional access policy.</span></span> <span data-ttu-id="748f1-123">Os valores possíveis são: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="748f1-123">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="748f1-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="748f1-124">Required.</span></span> <span data-ttu-id="748f1-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="748f1-125">Read-only.</span></span>|
|<span data-ttu-id="748f1-126">id</span><span class="sxs-lookup"><span data-stu-id="748f1-126">id</span></span>|<span data-ttu-id="748f1-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="748f1-127">String</span></span>|<span data-ttu-id="748f1-128">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="748f1-128">The unique identifier for this entity.</span></span> <span data-ttu-id="748f1-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="748f1-129">Required.</span></span> <span data-ttu-id="748f1-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="748f1-130">Read-only.</span></span>|
|<span data-ttu-id="748f1-131">latestPolicyModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="748f1-131">latestPolicyModifiedDateTime</span></span>|<span data-ttu-id="748f1-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="748f1-132">DateTimeOffset</span></span>|<span data-ttu-id="748f1-133">A data e a hora em que a política de acesso condicional foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="748f1-133">The date and time the conditional access policy was last modified.</span></span> <span data-ttu-id="748f1-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="748f1-134">Required.</span></span> <span data-ttu-id="748f1-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="748f1-135">Read-only.</span></span>|
|<span data-ttu-id="748f1-136">requiresDeviceCompliance</span><span class="sxs-lookup"><span data-stu-id="748f1-136">requiresDeviceCompliance</span></span>|<span data-ttu-id="748f1-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="748f1-137">Boolean</span></span>|<span data-ttu-id="748f1-138">Um sinalizador indicando se a política de acesso condicional requer conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="748f1-138">A flag indicating whether the conditional access policy requires device compliance.</span></span> <span data-ttu-id="748f1-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="748f1-139">Required.</span></span> <span data-ttu-id="748f1-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="748f1-140">Read-only.</span></span>|
|<span data-ttu-id="748f1-141">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="748f1-141">tenantDisplayName</span></span>|<span data-ttu-id="748f1-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="748f1-142">String</span></span>|<span data-ttu-id="748f1-143">O nome de exibição do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="748f1-143">The display name for the managed tenant.</span></span> <span data-ttu-id="748f1-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="748f1-144">Required.</span></span> <span data-ttu-id="748f1-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="748f1-145">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="748f1-146">Relações</span><span class="sxs-lookup"><span data-stu-id="748f1-146">Relationships</span></span>
<span data-ttu-id="748f1-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="748f1-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="748f1-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="748f1-148">JSON representation</span></span>
<span data-ttu-id="748f1-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="748f1-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "String (identifier)",
  "tenantDisplayName": "String",
  "conditionalAccessPolicyState": "String",
  "requiresDeviceCompliance": "Boolean",
  "latestPolicyModifiedDateTime": "String (timestamp)"
}
```
