---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f471a71c10a225f2bb5af77399932402f154538d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872118"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="e59c7-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="e59c7-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="e59c7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e59c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e59c7-105">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="e59c7-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="e59c7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e59c7-106">Properties</span></span>
|<span data-ttu-id="e59c7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e59c7-107">Property</span></span>|<span data-ttu-id="e59c7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e59c7-108">Type</span></span>|<span data-ttu-id="e59c7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e59c7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e59c7-110">validationName</span><span class="sxs-lookup"><span data-stu-id="e59c7-110">validationName</span></span>|<span data-ttu-id="e59c7-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e59c7-111">String</span></span>|<span data-ttu-id="e59c7-112">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="e59c7-112">The validation friendly name</span></span>|
|<span data-ttu-id="e59c7-113">estado</span><span class="sxs-lookup"><span data-stu-id="e59c7-113">state</span></span>|<span data-ttu-id="e59c7-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e59c7-114">String</span></span>|<span data-ttu-id="e59c7-115">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="e59c7-115">The state of the operation</span></span>|
|<span data-ttu-id="e59c7-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="e59c7-116">mitigationInstruction</span></span>|<span data-ttu-id="e59c7-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e59c7-117">String</span></span>|<span data-ttu-id="e59c7-118">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="e59c7-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="e59c7-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e59c7-119">Relationships</span></span>
<span data-ttu-id="e59c7-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e59c7-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e59c7-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e59c7-121">JSON Representation</span></span>
<span data-ttu-id="e59c7-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e59c7-122">Here is a JSON representation of the resource.</span></span>
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



