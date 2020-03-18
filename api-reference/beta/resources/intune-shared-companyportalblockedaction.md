---
title: tipo de recurso companyPortalBlockedAction
description: Ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ac1bebe15948c0088ee2d4d9355650fc435a1eb9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771667"
---
# <a name="companyportalblockedaction-resource-type"></a><span data-ttu-id="e58bc-103">tipo de recurso companyPortalBlockedAction</span><span class="sxs-lookup"><span data-stu-id="e58bc-103">companyPortalBlockedAction resource type</span></span>

> <span data-ttu-id="e58bc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e58bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e58bc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e58bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e58bc-106">Ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo</span><span class="sxs-lookup"><span data-stu-id="e58bc-106">Blocked actions on the company portal as per platform and device ownership types</span></span>

## <a name="properties"></a><span data-ttu-id="e58bc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e58bc-107">Properties</span></span>
|<span data-ttu-id="e58bc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e58bc-108">Property</span></span>|<span data-ttu-id="e58bc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e58bc-109">Type</span></span>|<span data-ttu-id="e58bc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e58bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e58bc-111">platform</span><span class="sxs-lookup"><span data-stu-id="e58bc-111">platform</span></span>|[<span data-ttu-id="e58bc-112">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="e58bc-112">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="e58bc-113">Sistema operacional/plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e58bc-113">Device OS/Platform.</span></span> <span data-ttu-id="e58bc-114">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e58bc-114">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="e58bc-115">ownerType</span><span class="sxs-lookup"><span data-stu-id="e58bc-115">ownerType</span></span>|[<span data-ttu-id="e58bc-116">ownerType</span><span class="sxs-lookup"><span data-stu-id="e58bc-116">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="e58bc-117">Tipo de propriedade de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e58bc-117">Device ownership type.</span></span> <span data-ttu-id="e58bc-118">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="e58bc-118">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="e58bc-119">ação</span><span class="sxs-lookup"><span data-stu-id="e58bc-119">action</span></span>|[<span data-ttu-id="e58bc-120">companyPortalAction</span><span class="sxs-lookup"><span data-stu-id="e58bc-120">companyPortalAction</span></span>](../resources/intune-shared-companyportalaction.md)|<span data-ttu-id="e58bc-121">Ação de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e58bc-121">Device Action.</span></span> <span data-ttu-id="e58bc-122">Os valores possíveis são: `unknown`, `remove`, `reset`.</span><span class="sxs-lookup"><span data-stu-id="e58bc-122">Possible values are: `unknown`, `remove`, `reset`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e58bc-123">Relações</span><span class="sxs-lookup"><span data-stu-id="e58bc-123">Relationships</span></span>
<span data-ttu-id="e58bc-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e58bc-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e58bc-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e58bc-125">JSON Representation</span></span>
<span data-ttu-id="e58bc-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e58bc-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyPortalBlockedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyPortalBlockedAction",
  "platform": "String",
  "ownerType": "String",
  "action": "String"
}
```



