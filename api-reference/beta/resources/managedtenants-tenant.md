---
title: tipo de recurso de locatário
description: Representa um locatário associado à entidade de gerenciamento.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: ee4bd57aa4e7fa2ea15c86376389d3b6e12198ea
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402140"
---
# <a name="tenant-resource-type"></a><span data-ttu-id="af47e-103">tipo de recurso de locatário</span><span class="sxs-lookup"><span data-stu-id="af47e-103">tenant resource type</span></span>

<span data-ttu-id="af47e-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="af47e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af47e-105">Representa um locatário associado à entidade de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="af47e-105">Represents a tenant associated with the managing entity.</span></span>

## <a name="methods"></a><span data-ttu-id="af47e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="af47e-106">Methods</span></span>
|<span data-ttu-id="af47e-107">Método</span><span class="sxs-lookup"><span data-stu-id="af47e-107">Method</span></span>|<span data-ttu-id="af47e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="af47e-108">Return type</span></span>|<span data-ttu-id="af47e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="af47e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af47e-110">Listar locatários</span><span class="sxs-lookup"><span data-stu-id="af47e-110">List tenants</span></span>](../api/managedtenants-managedtenant-list-tenants.md)|<span data-ttu-id="af47e-111">[coleção microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="af47e-111">[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md) collection</span></span>|<span data-ttu-id="af47e-112">Obter uma lista dos objetos [de locatário](../resources/managedtenants-tenant.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="af47e-112">Get a list of the [tenant](../resources/managedtenants-tenant.md) objects and their properties.</span></span>|
|[<span data-ttu-id="af47e-113">Obter locatário</span><span class="sxs-lookup"><span data-stu-id="af47e-113">Get tenant</span></span>](../api/managedtenants-tenant-get.md)|[<span data-ttu-id="af47e-114">microsoft.graph.managedTenants.tenant</span><span class="sxs-lookup"><span data-stu-id="af47e-114">microsoft.graph.managedTenants.tenant</span></span>](../resources/managedtenants-tenant.md)|<span data-ttu-id="af47e-115">Leia as propriedades e as relações de um [objeto tenant.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="af47e-115">Read the properties and relationships of a [tenant](../resources/managedtenants-tenant.md) object.</span></span>|
|[<span data-ttu-id="af47e-116">offboardTenant</span><span class="sxs-lookup"><span data-stu-id="af47e-116">offboardTenant</span></span>](../api/managedtenants-tenant-offboardtenant.md)|[<span data-ttu-id="af47e-117">microsoft.graph.managedTenants.tenant</span><span class="sxs-lookup"><span data-stu-id="af47e-117">microsoft.graph.managedTenants.tenant</span></span>](../resources/managedtenants-tenant.md)|<span data-ttu-id="af47e-118">Desempla um locatário da plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="af47e-118">Off boards a tenant from the multi-tenant management platform.</span></span>|
|[<span data-ttu-id="af47e-119">resetTenantOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="af47e-119">resetTenantOnboardingStatus</span></span>](../api/managedtenants-tenant-resettenantonboardingstatus.md)|[<span data-ttu-id="af47e-120">microsoft.graph.managedTenants.tenant</span><span class="sxs-lookup"><span data-stu-id="af47e-120">microsoft.graph.managedTenants.tenant</span></span>](../resources/managedtenants-tenant.md)|<span data-ttu-id="af47e-121">Redefine o status de integração do locatário com a plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="af47e-121">Resets the tenant onboarding status with the multi-tenant management platform.</span></span>|

## <a name="properties"></a><span data-ttu-id="af47e-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af47e-122">Properties</span></span>
|<span data-ttu-id="af47e-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af47e-123">Property</span></span>|<span data-ttu-id="af47e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="af47e-124">Type</span></span>|<span data-ttu-id="af47e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="af47e-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af47e-126">contrato</span><span class="sxs-lookup"><span data-stu-id="af47e-126">contract</span></span>|[<span data-ttu-id="af47e-127">microsoft.graph.managedTenants.tenantContract</span><span class="sxs-lookup"><span data-stu-id="af47e-127">microsoft.graph.managedTenants.tenantContract</span></span>](../resources/managedtenants-tenantcontract.md)|<span data-ttu-id="af47e-128">Os detalhes do relacionamento do locatário com a entidade de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="af47e-128">The relationship details for the tenant with the managing entity.</span></span>|
|<span data-ttu-id="af47e-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af47e-129">createdDateTime</span></span>|<span data-ttu-id="af47e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af47e-130">DateTimeOffset</span></span>|<span data-ttu-id="af47e-131">A data e a hora em que o locatário foi criado na plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="af47e-131">The date and time the tenant was created in the multi-tenant management platform.</span></span> <span data-ttu-id="af47e-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="af47e-132">Optional.</span></span> <span data-ttu-id="af47e-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af47e-133">Read-only.</span></span>|
|<span data-ttu-id="af47e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="af47e-134">displayName</span></span>|<span data-ttu-id="af47e-135">String</span><span class="sxs-lookup"><span data-stu-id="af47e-135">String</span></span>|<span data-ttu-id="af47e-136">O nome de exibição do locatário.</span><span class="sxs-lookup"><span data-stu-id="af47e-136">The display name for the tenant.</span></span> <span data-ttu-id="af47e-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af47e-137">Required.</span></span> <span data-ttu-id="af47e-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af47e-138">Read-only.</span></span>|
|<span data-ttu-id="af47e-139">id</span><span class="sxs-lookup"><span data-stu-id="af47e-139">id</span></span>|<span data-ttu-id="af47e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af47e-140">String</span></span>|<span data-ttu-id="af47e-141">O Azure Active Directory do locatário para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af47e-141">The Azure Active Directory tenant identifier for the tenant.</span></span> <span data-ttu-id="af47e-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af47e-142">Required.</span></span> <span data-ttu-id="af47e-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af47e-143">Read-only.</span></span>|
|<span data-ttu-id="af47e-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="af47e-144">lastUpdatedDateTime</span></span>|<span data-ttu-id="af47e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af47e-145">DateTimeOffset</span></span>|<span data-ttu-id="af47e-146">A data e a hora em que o locatário foi atualizado pela última vez na plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="af47e-146">The date and time the tenant was last updated within the multi-tenant management platform.</span></span> <span data-ttu-id="af47e-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="af47e-147">Optional.</span></span> <span data-ttu-id="af47e-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af47e-148">Read-only.</span></span>|
|<span data-ttu-id="af47e-149">tenantId</span><span class="sxs-lookup"><span data-stu-id="af47e-149">tenantId</span></span>|<span data-ttu-id="af47e-150">String</span><span class="sxs-lookup"><span data-stu-id="af47e-150">String</span></span>|<span data-ttu-id="af47e-151">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="af47e-151">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="af47e-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="af47e-152">Optional.</span></span> <span data-ttu-id="af47e-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af47e-153">Read-only.</span></span>|
|<span data-ttu-id="af47e-154">tenantStatusInformation</span><span class="sxs-lookup"><span data-stu-id="af47e-154">tenantStatusInformation</span></span>|[<span data-ttu-id="af47e-155">microsoft.graph.managedTenants.tenantStatusInformation</span><span class="sxs-lookup"><span data-stu-id="af47e-155">microsoft.graph.managedTenants.tenantStatusInformation</span></span>](../resources/managedtenants-tenantstatusinformation.md)|<span data-ttu-id="af47e-156">As informações de status de integração do locatário.</span><span class="sxs-lookup"><span data-stu-id="af47e-156">The onboarding status information for the tenant.</span></span> <span data-ttu-id="af47e-157">Opcional.</span><span class="sxs-lookup"><span data-stu-id="af47e-157">Optional.</span></span> <span data-ttu-id="af47e-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af47e-158">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af47e-159">Relações</span><span class="sxs-lookup"><span data-stu-id="af47e-159">Relationships</span></span>
<span data-ttu-id="af47e-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af47e-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af47e-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af47e-161">JSON representation</span></span>
<span data-ttu-id="af47e-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af47e-162">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenant",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenant",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "contract": {
    "@odata.type": "microsoft.graph.managedTenants.tenantContract"
  },
  "tenantStatusInformation": {
    "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
  },
  "lastUpdatedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)"
}
```
