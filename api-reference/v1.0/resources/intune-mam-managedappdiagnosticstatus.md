---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: tfitzmac
ms.openlocfilehash: 7f0cd0d5b11c4d902f51dd422add2373e8e8df9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340681"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="2dac6-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="2dac6-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="2dac6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2dac6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2dac6-105">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="2dac6-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="2dac6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2dac6-106">Properties</span></span>
|<span data-ttu-id="2dac6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2dac6-107">Property</span></span>|<span data-ttu-id="2dac6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dac6-108">Type</span></span>|<span data-ttu-id="2dac6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dac6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dac6-110">validationName</span><span class="sxs-lookup"><span data-stu-id="2dac6-110">validationName</span></span>|<span data-ttu-id="2dac6-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dac6-111">String</span></span>|<span data-ttu-id="2dac6-112">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="2dac6-112">The validation friendly name</span></span>|
|<span data-ttu-id="2dac6-113">estado</span><span class="sxs-lookup"><span data-stu-id="2dac6-113">state</span></span>|<span data-ttu-id="2dac6-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dac6-114">String</span></span>|<span data-ttu-id="2dac6-115">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="2dac6-115">The state of the operation</span></span>|
|<span data-ttu-id="2dac6-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="2dac6-116">mitigationInstruction</span></span>|<span data-ttu-id="2dac6-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dac6-117">String</span></span>|<span data-ttu-id="2dac6-118">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="2dac6-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dac6-119">Relações</span><span class="sxs-lookup"><span data-stu-id="2dac6-119">Relationships</span></span>
<span data-ttu-id="2dac6-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2dac6-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2dac6-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2dac6-121">JSON Representation</span></span>
<span data-ttu-id="2dac6-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2dac6-122">Here is a JSON representation of the resource.</span></span>
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



