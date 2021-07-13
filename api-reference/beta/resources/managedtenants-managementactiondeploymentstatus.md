---
title: tipo de recurso managementActionDeploymentStatus
description: Representa o status de implantação de um determinado locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: efd789a7b4b48098e8d679273da1152f6611a28c
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402011"
---
# <a name="managementactiondeploymentstatus-resource-type"></a><span data-ttu-id="09413-103">tipo de recurso managementActionDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="09413-103">managementActionDeploymentStatus resource type</span></span>

<span data-ttu-id="09413-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="09413-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09413-105">Representa o status de implantação de um determinado locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="09413-105">Represents the deployment status for a given managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="09413-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09413-106">Properties</span></span>
|<span data-ttu-id="09413-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09413-107">Property</span></span>|<span data-ttu-id="09413-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="09413-108">Type</span></span>|<span data-ttu-id="09413-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="09413-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09413-110">managementActionId</span><span class="sxs-lookup"><span data-stu-id="09413-110">managementActionId</span></span>|<span data-ttu-id="09413-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09413-111">String</span></span>|<span data-ttu-id="09413-112">O identificador da ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="09413-112">The identifier for the management action.</span></span> <span data-ttu-id="09413-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09413-113">Required.</span></span> <span data-ttu-id="09413-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="09413-114">Read-only.</span></span>|
|<span data-ttu-id="09413-115">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="09413-115">managementTemplateId</span></span>|<span data-ttu-id="09413-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09413-116">String</span></span>|<span data-ttu-id="09413-117">O identificador de modelo de gerenciamento usado para gerar a ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="09413-117">The management template identifier that was used to generate the management action.</span></span> <span data-ttu-id="09413-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09413-118">Required.</span></span> <span data-ttu-id="09413-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="09413-119">Read-only.</span></span>|
|<span data-ttu-id="09413-120">status</span><span class="sxs-lookup"><span data-stu-id="09413-120">status</span></span>|<span data-ttu-id="09413-121">managementActionStatus</span><span class="sxs-lookup"><span data-stu-id="09413-121">managementActionStatus</span></span>|<span data-ttu-id="09413-122">O status da ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="09413-122">The status of the management action.</span></span> <span data-ttu-id="09413-123">Os valores possíveis são: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, `riskAccepted`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="09413-123">Possible values are: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, `riskAccepted`, `unknownFutureValue`.</span></span> <span data-ttu-id="09413-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09413-124">Required.</span></span>|
|<span data-ttu-id="09413-125">workloadActionDeploymentStatuses</span><span class="sxs-lookup"><span data-stu-id="09413-125">workloadActionDeploymentStatuses</span></span>|<span data-ttu-id="09413-126">[coleção microsoft.graph.managedTenants.workloadActionDeploymentStatus](../resources/managedtenants-workloadactiondeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="09413-126">[microsoft.graph.managedTenants.workloadActionDeploymentStatus](../resources/managedtenants-workloadactiondeploymentstatus.md) collection</span></span>|<span data-ttu-id="09413-127">A coleção de estatuetas de implantação de ação de carga de trabalho para a ação de gerenciamento determinada.</span><span class="sxs-lookup"><span data-stu-id="09413-127">The collection of workload action deployment statues for the given management action.</span></span> <span data-ttu-id="09413-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="09413-128">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09413-129">Relações</span><span class="sxs-lookup"><span data-stu-id="09413-129">Relationships</span></span>
<span data-ttu-id="09413-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09413-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09413-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09413-131">JSON representation</span></span>
<span data-ttu-id="09413-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09413-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionDeploymentStatus",
  "managementTemplateId": "String",
  "managementActionId": "String",
  "status": "String",
  "workloadActionDeploymentStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
    }
  ]
}
```
