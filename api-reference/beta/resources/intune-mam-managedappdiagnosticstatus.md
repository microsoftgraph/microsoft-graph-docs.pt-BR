---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a896a17a2a79db6eea2ac2ece0973175506bac4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940761"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="b45fa-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="b45fa-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="b45fa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b45fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b45fa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b45fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b45fa-106">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="b45fa-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="b45fa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b45fa-107">Properties</span></span>
|<span data-ttu-id="b45fa-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b45fa-108">Property</span></span>|<span data-ttu-id="b45fa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b45fa-109">Type</span></span>|<span data-ttu-id="b45fa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b45fa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b45fa-111">validationName</span><span class="sxs-lookup"><span data-stu-id="b45fa-111">validationName</span></span>|<span data-ttu-id="b45fa-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b45fa-112">String</span></span>|<span data-ttu-id="b45fa-113">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="b45fa-113">The validation friendly name</span></span>|
|<span data-ttu-id="b45fa-114">state</span><span class="sxs-lookup"><span data-stu-id="b45fa-114">state</span></span>|<span data-ttu-id="b45fa-115">String</span><span class="sxs-lookup"><span data-stu-id="b45fa-115">String</span></span>|<span data-ttu-id="b45fa-116">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="b45fa-116">The state of the operation</span></span>|
|<span data-ttu-id="b45fa-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="b45fa-117">mitigationInstruction</span></span>|<span data-ttu-id="b45fa-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b45fa-118">String</span></span>|<span data-ttu-id="b45fa-119">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="b45fa-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="b45fa-120">Relações</span><span class="sxs-lookup"><span data-stu-id="b45fa-120">Relationships</span></span>
<span data-ttu-id="b45fa-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b45fa-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b45fa-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b45fa-122">JSON Representation</span></span>
<span data-ttu-id="b45fa-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b45fa-123">Here is a JSON representation of the resource.</span></span>
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




