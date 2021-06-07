---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 824bcb13741240b1f5bc462312004892ccd5c051
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751318"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="799dd-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="799dd-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="799dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="799dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="799dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="799dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="799dd-106">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="799dd-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="799dd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="799dd-107">Properties</span></span>
|<span data-ttu-id="799dd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="799dd-108">Property</span></span>|<span data-ttu-id="799dd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="799dd-109">Type</span></span>|<span data-ttu-id="799dd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="799dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="799dd-111">validationName</span><span class="sxs-lookup"><span data-stu-id="799dd-111">validationName</span></span>|<span data-ttu-id="799dd-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="799dd-112">String</span></span>|<span data-ttu-id="799dd-113">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="799dd-113">The validation friendly name</span></span>|
|<span data-ttu-id="799dd-114">estado</span><span class="sxs-lookup"><span data-stu-id="799dd-114">state</span></span>|<span data-ttu-id="799dd-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="799dd-115">String</span></span>|<span data-ttu-id="799dd-116">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="799dd-116">The state of the operation</span></span>|
|<span data-ttu-id="799dd-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="799dd-117">mitigationInstruction</span></span>|<span data-ttu-id="799dd-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="799dd-118">String</span></span>|<span data-ttu-id="799dd-119">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="799dd-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="799dd-120">Relações</span><span class="sxs-lookup"><span data-stu-id="799dd-120">Relationships</span></span>
<span data-ttu-id="799dd-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="799dd-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="799dd-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="799dd-122">JSON Representation</span></span>
<span data-ttu-id="799dd-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="799dd-123">Here is a JSON representation of the resource.</span></span>
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




