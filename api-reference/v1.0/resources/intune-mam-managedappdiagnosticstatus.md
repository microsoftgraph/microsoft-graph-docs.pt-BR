---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9bb957258f43eeb9303876bcc0fa41a4b622cc45
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448407"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="58ee5-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="58ee5-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="58ee5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="58ee5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58ee5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58ee5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58ee5-106">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="58ee5-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="58ee5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58ee5-107">Properties</span></span>
|<span data-ttu-id="58ee5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58ee5-108">Property</span></span>|<span data-ttu-id="58ee5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="58ee5-109">Type</span></span>|<span data-ttu-id="58ee5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="58ee5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58ee5-111">validationName</span><span class="sxs-lookup"><span data-stu-id="58ee5-111">validationName</span></span>|<span data-ttu-id="58ee5-112">String</span><span class="sxs-lookup"><span data-stu-id="58ee5-112">String</span></span>|<span data-ttu-id="58ee5-113">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="58ee5-113">The validation friendly name</span></span>|
|<span data-ttu-id="58ee5-114">state</span><span class="sxs-lookup"><span data-stu-id="58ee5-114">state</span></span>|<span data-ttu-id="58ee5-115">String</span><span class="sxs-lookup"><span data-stu-id="58ee5-115">String</span></span>|<span data-ttu-id="58ee5-116">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="58ee5-116">The state of the operation</span></span>|
|<span data-ttu-id="58ee5-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="58ee5-117">mitigationInstruction</span></span>|<span data-ttu-id="58ee5-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58ee5-118">String</span></span>|<span data-ttu-id="58ee5-119">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="58ee5-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="58ee5-120">Relações</span><span class="sxs-lookup"><span data-stu-id="58ee5-120">Relationships</span></span>
<span data-ttu-id="58ee5-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58ee5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58ee5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58ee5-122">JSON Representation</span></span>
<span data-ttu-id="58ee5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58ee5-123">Here is a JSON representation of the resource.</span></span>
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




