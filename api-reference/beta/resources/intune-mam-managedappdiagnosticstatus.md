---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: tfitzmac
ms.openlocfilehash: 1618c65b46654832fc7706f01cb6d6a9f78926e4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314774"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="cbd46-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="cbd46-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="cbd46-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cbd46-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbd46-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cbd46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbd46-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cbd46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbd46-107">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="cbd46-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="cbd46-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbd46-108">Properties</span></span>
|<span data-ttu-id="cbd46-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbd46-109">Property</span></span>|<span data-ttu-id="cbd46-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbd46-110">Type</span></span>|<span data-ttu-id="cbd46-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbd46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbd46-112">validationName</span><span class="sxs-lookup"><span data-stu-id="cbd46-112">validationName</span></span>|<span data-ttu-id="cbd46-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbd46-113">String</span></span>|<span data-ttu-id="cbd46-114">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="cbd46-114">The validation friendly name</span></span>|
|<span data-ttu-id="cbd46-115">estado</span><span class="sxs-lookup"><span data-stu-id="cbd46-115">state</span></span>|<span data-ttu-id="cbd46-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbd46-116">String</span></span>|<span data-ttu-id="cbd46-117">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="cbd46-117">The state of the operation</span></span>|
|<span data-ttu-id="cbd46-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="cbd46-118">mitigationInstruction</span></span>|<span data-ttu-id="cbd46-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbd46-119">String</span></span>|<span data-ttu-id="cbd46-120">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="cbd46-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbd46-121">Relações</span><span class="sxs-lookup"><span data-stu-id="cbd46-121">Relationships</span></span>
<span data-ttu-id="cbd46-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cbd46-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cbd46-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbd46-123">JSON Representation</span></span>
<span data-ttu-id="cbd46-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cbd46-124">Here is a JSON representation of the resource.</span></span>
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





