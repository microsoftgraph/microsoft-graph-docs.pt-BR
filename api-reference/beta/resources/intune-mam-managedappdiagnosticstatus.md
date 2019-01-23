---
title: Tipo de recurso managedAppDiagnosticStatus
description: Representa o status de diagnóstico.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 665ca55c67f5facb22eaf976e81737fed3dacf76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407358"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="1447d-103">Tipo de recurso managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="1447d-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="1447d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="1447d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1447d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1447d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1447d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="1447d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1447d-107">Representa o status de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="1447d-107">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="1447d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1447d-108">Properties</span></span>
|<span data-ttu-id="1447d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1447d-109">Property</span></span>|<span data-ttu-id="1447d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1447d-110">Type</span></span>|<span data-ttu-id="1447d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1447d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1447d-112">validationName</span><span class="sxs-lookup"><span data-stu-id="1447d-112">validationName</span></span>|<span data-ttu-id="1447d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1447d-113">String</span></span>|<span data-ttu-id="1447d-114">O nome amigável da validação</span><span class="sxs-lookup"><span data-stu-id="1447d-114">The validation friendly name</span></span>|
|<span data-ttu-id="1447d-115">estado</span><span class="sxs-lookup"><span data-stu-id="1447d-115">state</span></span>|<span data-ttu-id="1447d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1447d-116">String</span></span>|<span data-ttu-id="1447d-117">O estado da operação</span><span class="sxs-lookup"><span data-stu-id="1447d-117">The state of the operation</span></span>|
|<span data-ttu-id="1447d-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="1447d-118">mitigationInstruction</span></span>|<span data-ttu-id="1447d-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1447d-119">String</span></span>|<span data-ttu-id="1447d-120">Instruções sobre como atenuar uma falha de validação</span><span class="sxs-lookup"><span data-stu-id="1447d-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="1447d-121">Relações</span><span class="sxs-lookup"><span data-stu-id="1447d-121">Relationships</span></span>
<span data-ttu-id="1447d-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1447d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1447d-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1447d-123">JSON Representation</span></span>
<span data-ttu-id="1447d-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1447d-124">Here is a JSON representation of the resource.</span></span>
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




