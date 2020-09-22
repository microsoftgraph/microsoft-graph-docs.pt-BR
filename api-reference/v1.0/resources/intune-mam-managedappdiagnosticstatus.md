---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c708da33594087b61b1c28e2ebac5b8872541838
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041306"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="b0744-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="b0744-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="b0744-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0744-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0744-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0744-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0744-106">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="b0744-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="b0744-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0744-107">Properties</span></span>
|<span data-ttu-id="b0744-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0744-108">Property</span></span>|<span data-ttu-id="b0744-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0744-109">Type</span></span>|<span data-ttu-id="b0744-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0744-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0744-111">validationName</span><span class="sxs-lookup"><span data-stu-id="b0744-111">validationName</span></span>|<span data-ttu-id="b0744-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0744-112">String</span></span>|<span data-ttu-id="b0744-113">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="b0744-113">The validation friendly name</span></span>|
|<span data-ttu-id="b0744-114">state</span><span class="sxs-lookup"><span data-stu-id="b0744-114">state</span></span>|<span data-ttu-id="b0744-115">String</span><span class="sxs-lookup"><span data-stu-id="b0744-115">String</span></span>|<span data-ttu-id="b0744-116">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="b0744-116">The state of the operation</span></span>|
|<span data-ttu-id="b0744-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="b0744-117">mitigationInstruction</span></span>|<span data-ttu-id="b0744-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0744-118">String</span></span>|<span data-ttu-id="b0744-119">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="b0744-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0744-120">Relações</span><span class="sxs-lookup"><span data-stu-id="b0744-120">Relationships</span></span>
<span data-ttu-id="b0744-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0744-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0744-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0744-122">JSON Representation</span></span>
<span data-ttu-id="b0744-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0744-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```









