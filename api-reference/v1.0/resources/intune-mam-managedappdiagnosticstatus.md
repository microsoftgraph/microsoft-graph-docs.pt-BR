---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 33a975318854ab8bfec35ca257ee0c59fc29c188
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356363"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="91bf2-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="91bf2-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="91bf2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91bf2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91bf2-105">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="91bf2-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="91bf2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91bf2-106">Properties</span></span>
|<span data-ttu-id="91bf2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91bf2-107">Property</span></span>|<span data-ttu-id="91bf2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="91bf2-108">Type</span></span>|<span data-ttu-id="91bf2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="91bf2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91bf2-110">validationName</span><span class="sxs-lookup"><span data-stu-id="91bf2-110">validationName</span></span>|<span data-ttu-id="91bf2-111">String</span><span class="sxs-lookup"><span data-stu-id="91bf2-111">String</span></span>|<span data-ttu-id="91bf2-112">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="91bf2-112">The validation friendly name</span></span>|
|<span data-ttu-id="91bf2-113">state</span><span class="sxs-lookup"><span data-stu-id="91bf2-113">state</span></span>|<span data-ttu-id="91bf2-114">String</span><span class="sxs-lookup"><span data-stu-id="91bf2-114">String</span></span>|<span data-ttu-id="91bf2-115">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="91bf2-115">The state of the operation</span></span>|
|<span data-ttu-id="91bf2-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="91bf2-116">mitigationInstruction</span></span>|<span data-ttu-id="91bf2-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91bf2-117">String</span></span>|<span data-ttu-id="91bf2-118">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="91bf2-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="91bf2-119">Relações</span><span class="sxs-lookup"><span data-stu-id="91bf2-119">Relationships</span></span>
<span data-ttu-id="91bf2-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91bf2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91bf2-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91bf2-121">JSON Representation</span></span>
<span data-ttu-id="91bf2-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91bf2-122">Here is a JSON representation of the resource.</span></span>
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




