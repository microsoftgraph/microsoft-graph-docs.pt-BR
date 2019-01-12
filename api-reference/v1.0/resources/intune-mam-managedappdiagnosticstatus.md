---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a5204a4704eefc2d4e7c8e0d5b3b709e1750667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937478"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="18629-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="18629-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="18629-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="18629-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18629-105">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="18629-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="18629-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18629-106">Properties</span></span>
|<span data-ttu-id="18629-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18629-107">Property</span></span>|<span data-ttu-id="18629-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="18629-108">Type</span></span>|<span data-ttu-id="18629-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="18629-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18629-110">validationName</span><span class="sxs-lookup"><span data-stu-id="18629-110">validationName</span></span>|<span data-ttu-id="18629-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18629-111">String</span></span>|<span data-ttu-id="18629-112">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="18629-112">The validation friendly name</span></span>|
|<span data-ttu-id="18629-113">estado</span><span class="sxs-lookup"><span data-stu-id="18629-113">state</span></span>|<span data-ttu-id="18629-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18629-114">String</span></span>|<span data-ttu-id="18629-115">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="18629-115">The state of the operation</span></span>|
|<span data-ttu-id="18629-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="18629-116">mitigationInstruction</span></span>|<span data-ttu-id="18629-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18629-117">String</span></span>|<span data-ttu-id="18629-118">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="18629-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="18629-119">Relações</span><span class="sxs-lookup"><span data-stu-id="18629-119">Relationships</span></span>
<span data-ttu-id="18629-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18629-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="18629-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18629-121">JSON Representation</span></span>
<span data-ttu-id="18629-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18629-122">Here is a JSON representation of the resource.</span></span>
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



