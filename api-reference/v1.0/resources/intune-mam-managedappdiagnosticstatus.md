---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79a89b7084ea006352ad0bc423d0833acfaae86e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038042"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="73308-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="73308-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="73308-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73308-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73308-105">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="73308-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="73308-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73308-106">Properties</span></span>
|<span data-ttu-id="73308-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73308-107">Property</span></span>|<span data-ttu-id="73308-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="73308-108">Type</span></span>|<span data-ttu-id="73308-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73308-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73308-110">validationName</span><span class="sxs-lookup"><span data-stu-id="73308-110">validationName</span></span>|<span data-ttu-id="73308-111">String</span><span class="sxs-lookup"><span data-stu-id="73308-111">String</span></span>|<span data-ttu-id="73308-112">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="73308-112">The validation friendly name</span></span>|
|<span data-ttu-id="73308-113">state</span><span class="sxs-lookup"><span data-stu-id="73308-113">state</span></span>|<span data-ttu-id="73308-114">String</span><span class="sxs-lookup"><span data-stu-id="73308-114">String</span></span>|<span data-ttu-id="73308-115">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="73308-115">The state of the operation</span></span>|
|<span data-ttu-id="73308-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="73308-116">mitigationInstruction</span></span>|<span data-ttu-id="73308-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73308-117">String</span></span>|<span data-ttu-id="73308-118">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="73308-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="73308-119">Relações</span><span class="sxs-lookup"><span data-stu-id="73308-119">Relationships</span></span>
<span data-ttu-id="73308-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73308-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73308-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73308-121">JSON Representation</span></span>
<span data-ttu-id="73308-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73308-122">Here is a JSON representation of the resource.</span></span>
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



