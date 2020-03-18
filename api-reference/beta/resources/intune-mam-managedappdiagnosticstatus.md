---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6020b6a8875b8e2aff2e92b007364fc3011da216
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781940"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="1eeea-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="1eeea-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="1eeea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1eeea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1eeea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1eeea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eeea-106">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="1eeea-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="1eeea-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1eeea-107">Properties</span></span>
|<span data-ttu-id="1eeea-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1eeea-108">Property</span></span>|<span data-ttu-id="1eeea-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1eeea-109">Type</span></span>|<span data-ttu-id="1eeea-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eeea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eeea-111">validationName</span><span class="sxs-lookup"><span data-stu-id="1eeea-111">validationName</span></span>|<span data-ttu-id="1eeea-112">String</span><span class="sxs-lookup"><span data-stu-id="1eeea-112">String</span></span>|<span data-ttu-id="1eeea-113">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="1eeea-113">The validation friendly name</span></span>|
|<span data-ttu-id="1eeea-114">state</span><span class="sxs-lookup"><span data-stu-id="1eeea-114">state</span></span>|<span data-ttu-id="1eeea-115">String</span><span class="sxs-lookup"><span data-stu-id="1eeea-115">String</span></span>|<span data-ttu-id="1eeea-116">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="1eeea-116">The state of the operation</span></span>|
|<span data-ttu-id="1eeea-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="1eeea-117">mitigationInstruction</span></span>|<span data-ttu-id="1eeea-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1eeea-118">String</span></span>|<span data-ttu-id="1eeea-119">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="1eeea-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="1eeea-120">Relações</span><span class="sxs-lookup"><span data-stu-id="1eeea-120">Relationships</span></span>
<span data-ttu-id="1eeea-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1eeea-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1eeea-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1eeea-122">JSON Representation</span></span>
<span data-ttu-id="1eeea-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1eeea-123">Here is a JSON representation of the resource.</span></span>
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



