---
title: tipo de recurso managementActionTenantDeploymentStatus
description: Representa o status de implantação de nível de locatário para a ação de gerenciamento.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 1967c3ad96cc9c4e76a718cafab7ba14207753a9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401999"
---
# <a name="managementactiontenantdeploymentstatus-resource-type"></a><span data-ttu-id="c7028-103">tipo de recurso managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c7028-103">managementActionTenantDeploymentStatus resource type</span></span>

<span data-ttu-id="c7028-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c7028-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7028-105">Representa o status de implantação de nível de locatário para a ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c7028-105">Represents tenant level deployment status for the management action.</span></span>

## <a name="methods"></a><span data-ttu-id="c7028-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c7028-106">Methods</span></span>
|<span data-ttu-id="c7028-107">Método</span><span class="sxs-lookup"><span data-stu-id="c7028-107">Method</span></span>|<span data-ttu-id="c7028-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c7028-108">Return type</span></span>|<span data-ttu-id="c7028-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7028-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7028-110">Gerenciamento de listaActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c7028-110">List managementActionTenantDeploymentStatus</span></span>](../api/managedtenants-managedtenant-list-managementactiontenantdeploymentstatuses.md)|<span data-ttu-id="c7028-111">[coleção microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c7028-111">[microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) collection</span></span>|<span data-ttu-id="c7028-112">Obter uma lista dos [objetos managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c7028-112">Get a list of the [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) objects and their properties.</span></span>|
|[<span data-ttu-id="c7028-113">Obter managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c7028-113">Get managementActionTenantDeploymentStatus</span></span>](../api/managedtenants-managementactiontenantdeploymentstatus-get.md)|[<span data-ttu-id="c7028-114">microsoft.graph.managedTenants.managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c7028-114">microsoft.graph.managedTenants.managementActionTenantDeploymentStatus</span></span>](../resources/managedtenants-managementactiontenantdeploymentstatus.md)|<span data-ttu-id="c7028-115">Leia as propriedades e as relações de [um objeto managementActionTenantDeploymentStatus.](../resources/managedtenants-managementactiontenantdeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c7028-115">Read the properties and relationships of a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object.</span></span>|
|[<span data-ttu-id="c7028-116">changeDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c7028-116">changeDeploymentStatus</span></span>](../api/managedtenants-managementactiontenantdeploymentstatus-changedeploymentstatus.md)|[<span data-ttu-id="c7028-117">microsoft.graph.managedTenants.managementActionDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c7028-117">microsoft.graph.managedTenants.managementActionDeploymentStatus</span></span>](../resources/managedtenants-managementactiondeploymentstatus.md)|<span data-ttu-id="c7028-118">Altera o status de implantação da ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c7028-118">Changes the deployment status for the management action.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7028-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7028-119">Properties</span></span>
|<span data-ttu-id="c7028-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7028-120">Property</span></span>|<span data-ttu-id="c7028-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7028-121">Type</span></span>|<span data-ttu-id="c7028-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7028-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7028-123">id</span><span class="sxs-lookup"><span data-stu-id="c7028-123">id</span></span>|<span data-ttu-id="c7028-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7028-124">String</span></span>|<span data-ttu-id="c7028-125">O identificador exclusivo para o status de implantação no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="c7028-125">The unique identifier for the tenant level deployment status.</span></span> <span data-ttu-id="c7028-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7028-126">Required.</span></span> <span data-ttu-id="c7028-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7028-127">Read-only.</span></span>|
|<span data-ttu-id="c7028-128">statuses</span><span class="sxs-lookup"><span data-stu-id="c7028-128">statuses</span></span>|<span data-ttu-id="c7028-129">[coleção microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c7028-129">[microsoft.graph.managedTenants.managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) collection</span></span>|<span data-ttu-id="c7028-130">O conjunto de status de implantação para cada instância de uma ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c7028-130">The collection of deployment status for each instance of a management action.</span></span> <span data-ttu-id="c7028-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c7028-131">Optional.</span></span>|
|<span data-ttu-id="c7028-132">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="c7028-132">tenantGroupId</span></span>|<span data-ttu-id="c7028-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7028-133">String</span></span>|<span data-ttu-id="c7028-134">O identificador do grupo de locatários associado à ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c7028-134">The identifier for the tenant group that is associated with the management action.</span></span> <span data-ttu-id="c7028-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7028-135">Required.</span></span> <span data-ttu-id="c7028-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7028-136">Read-only.</span></span>|
|<span data-ttu-id="c7028-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="c7028-137">tenantId</span></span>|<span data-ttu-id="c7028-138">String</span><span class="sxs-lookup"><span data-stu-id="c7028-138">String</span></span>|<span data-ttu-id="c7028-139">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="c7028-139">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="c7028-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7028-140">Required.</span></span> <span data-ttu-id="c7028-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7028-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7028-142">Relações</span><span class="sxs-lookup"><span data-stu-id="c7028-142">Relationships</span></span>
<span data-ttu-id="c7028-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7028-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7028-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7028-144">JSON representation</span></span>
<span data-ttu-id="c7028-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7028-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementActionTenantDeploymentStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionTenantDeploymentStatus",
  "id": "String (identifier)",
  "tenantGroupId": "String",
  "tenantId": "String",
  "statuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
    }
  ]
}
```
