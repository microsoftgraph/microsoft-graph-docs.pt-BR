---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 98bd1353156c99861749bdb7eac2e686cf96532e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869787"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="74ac8-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="74ac8-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="74ac8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="74ac8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74ac8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="74ac8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74ac8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="74ac8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74ac8-107">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="74ac8-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="74ac8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74ac8-108">Properties</span></span>
|<span data-ttu-id="74ac8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74ac8-109">Property</span></span>|<span data-ttu-id="74ac8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="74ac8-110">Type</span></span>|<span data-ttu-id="74ac8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="74ac8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74ac8-112">validationName</span><span class="sxs-lookup"><span data-stu-id="74ac8-112">validationName</span></span>|<span data-ttu-id="74ac8-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74ac8-113">String</span></span>|<span data-ttu-id="74ac8-114">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="74ac8-114">The validation friendly name</span></span>|
|<span data-ttu-id="74ac8-115">estado</span><span class="sxs-lookup"><span data-stu-id="74ac8-115">state</span></span>|<span data-ttu-id="74ac8-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74ac8-116">String</span></span>|<span data-ttu-id="74ac8-117">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="74ac8-117">The state of the operation</span></span>|
|<span data-ttu-id="74ac8-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="74ac8-118">mitigationInstruction</span></span>|<span data-ttu-id="74ac8-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74ac8-119">String</span></span>|<span data-ttu-id="74ac8-120">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="74ac8-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="74ac8-121">Relações</span><span class="sxs-lookup"><span data-stu-id="74ac8-121">Relationships</span></span>
<span data-ttu-id="74ac8-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74ac8-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="74ac8-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74ac8-123">JSON Representation</span></span>
<span data-ttu-id="74ac8-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74ac8-124">Here is a JSON representation of the resource.</span></span>
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





