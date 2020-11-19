---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df42f0b831480208e3cf70b63aa26d7b11a55486
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266876"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="7a651-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="7a651-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="7a651-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a651-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a651-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a651-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a651-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a651-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a651-107">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="7a651-107">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="7a651-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a651-108">Properties</span></span>
|<span data-ttu-id="7a651-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a651-109">Property</span></span>|<span data-ttu-id="7a651-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a651-110">Type</span></span>|<span data-ttu-id="7a651-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a651-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a651-112">validationName</span><span class="sxs-lookup"><span data-stu-id="7a651-112">validationName</span></span>|<span data-ttu-id="7a651-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a651-113">String</span></span>|<span data-ttu-id="7a651-114">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="7a651-114">The validation friendly name</span></span>|
|<span data-ttu-id="7a651-115">state</span><span class="sxs-lookup"><span data-stu-id="7a651-115">state</span></span>|<span data-ttu-id="7a651-116">String</span><span class="sxs-lookup"><span data-stu-id="7a651-116">String</span></span>|<span data-ttu-id="7a651-117">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="7a651-117">The state of the operation</span></span>|
|<span data-ttu-id="7a651-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="7a651-118">mitigationInstruction</span></span>|<span data-ttu-id="7a651-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a651-119">String</span></span>|<span data-ttu-id="7a651-120">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="7a651-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a651-121">Relações</span><span class="sxs-lookup"><span data-stu-id="7a651-121">Relationships</span></span>
<span data-ttu-id="7a651-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a651-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a651-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a651-123">JSON Representation</span></span>
<span data-ttu-id="7a651-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a651-124">Here is a JSON representation of the resource.</span></span>
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




