---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 74743a345688699ac25399e92af53f17afe86626
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030336"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="37e9f-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="37e9f-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="37e9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37e9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37e9f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37e9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37e9f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37e9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37e9f-107">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="37e9f-107">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="37e9f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37e9f-108">Properties</span></span>
|<span data-ttu-id="37e9f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37e9f-109">Property</span></span>|<span data-ttu-id="37e9f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="37e9f-110">Type</span></span>|<span data-ttu-id="37e9f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37e9f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37e9f-112">validationName</span><span class="sxs-lookup"><span data-stu-id="37e9f-112">validationName</span></span>|<span data-ttu-id="37e9f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37e9f-113">String</span></span>|<span data-ttu-id="37e9f-114">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="37e9f-114">The validation friendly name</span></span>|
|<span data-ttu-id="37e9f-115">state</span><span class="sxs-lookup"><span data-stu-id="37e9f-115">state</span></span>|<span data-ttu-id="37e9f-116">String</span><span class="sxs-lookup"><span data-stu-id="37e9f-116">String</span></span>|<span data-ttu-id="37e9f-117">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="37e9f-117">The state of the operation</span></span>|
|<span data-ttu-id="37e9f-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="37e9f-118">mitigationInstruction</span></span>|<span data-ttu-id="37e9f-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37e9f-119">String</span></span>|<span data-ttu-id="37e9f-120">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="37e9f-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="37e9f-121">Relações</span><span class="sxs-lookup"><span data-stu-id="37e9f-121">Relationships</span></span>
<span data-ttu-id="37e9f-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37e9f-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37e9f-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37e9f-123">JSON Representation</span></span>
<span data-ttu-id="37e9f-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37e9f-124">Here is a JSON representation of the resource.</span></span>
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






