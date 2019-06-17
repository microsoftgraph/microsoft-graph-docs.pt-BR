---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 907f9940b7cbb4a35f69e0792092e14c99aebdae
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996292"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="fe5fd-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="fe5fd-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="fe5fd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe5fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe5fd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe5fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe5fd-106">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="fe5fd-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="fe5fd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe5fd-107">Properties</span></span>
|<span data-ttu-id="fe5fd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe5fd-108">Property</span></span>|<span data-ttu-id="fe5fd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe5fd-109">Type</span></span>|<span data-ttu-id="fe5fd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe5fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe5fd-111">validationName</span><span class="sxs-lookup"><span data-stu-id="fe5fd-111">validationName</span></span>|<span data-ttu-id="fe5fd-112">String</span><span class="sxs-lookup"><span data-stu-id="fe5fd-112">String</span></span>|<span data-ttu-id="fe5fd-113">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="fe5fd-113">The validation friendly name</span></span>|
|<span data-ttu-id="fe5fd-114">state</span><span class="sxs-lookup"><span data-stu-id="fe5fd-114">state</span></span>|<span data-ttu-id="fe5fd-115">String</span><span class="sxs-lookup"><span data-stu-id="fe5fd-115">String</span></span>|<span data-ttu-id="fe5fd-116">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="fe5fd-116">The state of the operation</span></span>|
|<span data-ttu-id="fe5fd-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="fe5fd-117">mitigationInstruction</span></span>|<span data-ttu-id="fe5fd-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe5fd-118">String</span></span>|<span data-ttu-id="fe5fd-119">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="fe5fd-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe5fd-120">Relações</span><span class="sxs-lookup"><span data-stu-id="fe5fd-120">Relationships</span></span>
<span data-ttu-id="fe5fd-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fe5fd-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe5fd-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe5fd-122">JSON Representation</span></span>
<span data-ttu-id="fe5fd-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe5fd-123">Here is a JSON representation of the resource.</span></span>
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





