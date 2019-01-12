---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 210edaf8eb039db928d612337aa7c8e0642c9ee3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987185"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="6d7a1-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="6d7a1-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="6d7a1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6d7a1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d7a1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6d7a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d7a1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6d7a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d7a1-107">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="6d7a1-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="6d7a1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d7a1-108">Properties</span></span>
|<span data-ttu-id="6d7a1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d7a1-109">Property</span></span>|<span data-ttu-id="6d7a1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d7a1-110">Type</span></span>|<span data-ttu-id="6d7a1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d7a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d7a1-112">validationName</span><span class="sxs-lookup"><span data-stu-id="6d7a1-112">validationName</span></span>|<span data-ttu-id="6d7a1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d7a1-113">String</span></span>|<span data-ttu-id="6d7a1-114">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="6d7a1-114">The validation friendly name</span></span>|
|<span data-ttu-id="6d7a1-115">estado</span><span class="sxs-lookup"><span data-stu-id="6d7a1-115">state</span></span>|<span data-ttu-id="6d7a1-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d7a1-116">String</span></span>|<span data-ttu-id="6d7a1-117">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="6d7a1-117">The state of the operation</span></span>|
|<span data-ttu-id="6d7a1-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="6d7a1-118">mitigationInstruction</span></span>|<span data-ttu-id="6d7a1-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d7a1-119">String</span></span>|<span data-ttu-id="6d7a1-120">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="6d7a1-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d7a1-121">Relações</span><span class="sxs-lookup"><span data-stu-id="6d7a1-121">Relationships</span></span>
<span data-ttu-id="6d7a1-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d7a1-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d7a1-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d7a1-123">JSON Representation</span></span>
<span data-ttu-id="6d7a1-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d7a1-124">Here is a JSON representation of the resource.</span></span>
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





