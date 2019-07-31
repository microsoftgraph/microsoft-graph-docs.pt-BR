---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0804b83f819a2f083493418e0cd1240702c2e425
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998426"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="96095-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="96095-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="96095-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96095-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96095-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96095-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96095-106">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="96095-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="96095-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96095-107">Properties</span></span>
|<span data-ttu-id="96095-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96095-108">Property</span></span>|<span data-ttu-id="96095-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="96095-109">Type</span></span>|<span data-ttu-id="96095-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="96095-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96095-111">validationName</span><span class="sxs-lookup"><span data-stu-id="96095-111">validationName</span></span>|<span data-ttu-id="96095-112">String</span><span class="sxs-lookup"><span data-stu-id="96095-112">String</span></span>|<span data-ttu-id="96095-113">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="96095-113">The validation friendly name</span></span>|
|<span data-ttu-id="96095-114">state</span><span class="sxs-lookup"><span data-stu-id="96095-114">state</span></span>|<span data-ttu-id="96095-115">String</span><span class="sxs-lookup"><span data-stu-id="96095-115">String</span></span>|<span data-ttu-id="96095-116">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="96095-116">The state of the operation</span></span>|
|<span data-ttu-id="96095-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="96095-117">mitigationInstruction</span></span>|<span data-ttu-id="96095-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96095-118">String</span></span>|<span data-ttu-id="96095-119">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="96095-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="96095-120">Relações</span><span class="sxs-lookup"><span data-stu-id="96095-120">Relationships</span></span>
<span data-ttu-id="96095-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96095-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96095-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96095-122">JSON Representation</span></span>
<span data-ttu-id="96095-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96095-123">Here is a JSON representation of the resource.</span></span>
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





