---
title: Tipo de recurso workloadActionDeploymentStatus
description: Representa o status de implantação da ação de carga de trabalho.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a8c14b821ceabf8c8196a25c141ad8730f7151d6
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401963"
---
# <a name="workloadactiondeploymentstatus-resource-type"></a><span data-ttu-id="3d94a-103">Tipo de recurso workloadActionDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="3d94a-103">workloadActionDeploymentStatus resource type</span></span>

<span data-ttu-id="3d94a-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="3d94a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d94a-105">Representa o status de implantação da ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="3d94a-105">Represents the deployment status for the workload action.</span></span>

## <a name="properties"></a><span data-ttu-id="3d94a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d94a-106">Properties</span></span>
|<span data-ttu-id="3d94a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d94a-107">Property</span></span>|<span data-ttu-id="3d94a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d94a-108">Type</span></span>|<span data-ttu-id="3d94a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d94a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d94a-110">actionId</span><span class="sxs-lookup"><span data-stu-id="3d94a-110">actionId</span></span>|<span data-ttu-id="3d94a-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d94a-111">String</span></span>|<span data-ttu-id="3d94a-112">O identificador exclusivo da ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="3d94a-112">The unique identifier for the workload action.</span></span> <span data-ttu-id="3d94a-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d94a-113">Required.</span></span> <span data-ttu-id="3d94a-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d94a-114">Read-only.</span></span>|
|<span data-ttu-id="3d94a-115">deployedPolicyId</span><span class="sxs-lookup"><span data-stu-id="3d94a-115">deployedPolicyId</span></span>|<span data-ttu-id="3d94a-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d94a-116">String</span></span>|<span data-ttu-id="3d94a-117">O identificador de qualquer política que foi criada aplicando a ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="3d94a-117">The identifier of any policy that was created by applying the workload action.</span></span> <span data-ttu-id="3d94a-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d94a-118">Optional.</span></span> <span data-ttu-id="3d94a-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d94a-119">Read-only.</span></span>|
|<span data-ttu-id="3d94a-120">erro</span><span class="sxs-lookup"><span data-stu-id="3d94a-120">error</span></span>|[<span data-ttu-id="3d94a-121">microsoft.graph.genericError</span><span class="sxs-lookup"><span data-stu-id="3d94a-121">microsoft.graph.genericError</span></span>](../resources/genericerror.md)|<span data-ttu-id="3d94a-122">As informações detalhadas para exceções que ocorrem ao implantar a ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="3d94a-122">The detailed information for exceptions that occur when deploying the workload action.</span></span> <span data-ttu-id="3d94a-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d94a-123">Optional.</span></span> <span data-ttu-id="3d94a-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d94a-124">Required.</span></span>|
|<span data-ttu-id="3d94a-125">lastDeploymentDateTime</span><span class="sxs-lookup"><span data-stu-id="3d94a-125">lastDeploymentDateTime</span></span>|<span data-ttu-id="3d94a-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d94a-126">DateTimeOffset</span></span>|<span data-ttu-id="3d94a-127">A data e a hora em que a ação de carga de trabalho foi implantada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3d94a-127">The date and time the workload action was last deployed.</span></span> <span data-ttu-id="3d94a-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d94a-128">Optional.</span></span>|
|<span data-ttu-id="3d94a-129">status</span><span class="sxs-lookup"><span data-stu-id="3d94a-129">status</span></span>|<span data-ttu-id="3d94a-130">workloadActionStatus</span><span class="sxs-lookup"><span data-stu-id="3d94a-130">workloadActionStatus</span></span>|<span data-ttu-id="3d94a-131">O status da implantação da ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="3d94a-131">The status of the workload action deployment.</span></span> <span data-ttu-id="3d94a-132">Os possíveis valores são: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3d94a-132">Possible values are: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `unknownFutureValue`.</span></span> <span data-ttu-id="3d94a-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d94a-133">Required.</span></span> <span data-ttu-id="3d94a-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d94a-134">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d94a-135">Relações</span><span class="sxs-lookup"><span data-stu-id="3d94a-135">Relationships</span></span>
<span data-ttu-id="3d94a-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d94a-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d94a-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d94a-137">JSON representation</span></span>
<span data-ttu-id="3d94a-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d94a-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadActionDeploymentStatus",
  "actionId": "String",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.genericError"
  },
  "deployedPolicyId": "String",
  "lastDeploymentDateTime": "String (timestamp)"
}
```
