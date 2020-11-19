---
title: tipo de recurso companyPortalBlockedAction
description: Ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a733f93f64a62f9afca92fce1a8c16c06ab7f57e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258987"
---
# <a name="companyportalblockedaction-resource-type"></a><span data-ttu-id="9d4c2-103">tipo de recurso companyPortalBlockedAction</span><span class="sxs-lookup"><span data-stu-id="9d4c2-103">companyPortalBlockedAction resource type</span></span>

<span data-ttu-id="9d4c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d4c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d4c2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d4c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d4c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d4c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d4c2-107">Ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo</span><span class="sxs-lookup"><span data-stu-id="9d4c2-107">Blocked actions on the company portal as per platform and device ownership types</span></span>

## <a name="properties"></a><span data-ttu-id="9d4c2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d4c2-108">Properties</span></span>
|<span data-ttu-id="9d4c2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d4c2-109">Property</span></span>|<span data-ttu-id="9d4c2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d4c2-110">Type</span></span>|<span data-ttu-id="9d4c2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d4c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d4c2-112">plataforma</span><span class="sxs-lookup"><span data-stu-id="9d4c2-112">platform</span></span>|[<span data-ttu-id="9d4c2-113">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="9d4c2-113">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="9d4c2-114">Sistema operacional/plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d4c2-114">Device OS/Platform.</span></span> <span data-ttu-id="9d4c2-115">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="9d4c2-115">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="9d4c2-116">ownerType</span><span class="sxs-lookup"><span data-stu-id="9d4c2-116">ownerType</span></span>|[<span data-ttu-id="9d4c2-117">ownerType</span><span class="sxs-lookup"><span data-stu-id="9d4c2-117">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="9d4c2-118">Tipo de propriedade de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d4c2-118">Device ownership type.</span></span> <span data-ttu-id="9d4c2-119">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="9d4c2-119">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="9d4c2-120">ação</span><span class="sxs-lookup"><span data-stu-id="9d4c2-120">action</span></span>|[<span data-ttu-id="9d4c2-121">companyPortalAction</span><span class="sxs-lookup"><span data-stu-id="9d4c2-121">companyPortalAction</span></span>](../resources/intune-shared-companyportalaction.md)|<span data-ttu-id="9d4c2-122">Ação de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d4c2-122">Device Action.</span></span> <span data-ttu-id="9d4c2-123">Os valores possíveis são: `unknown`, `remove`, `reset`.</span><span class="sxs-lookup"><span data-stu-id="9d4c2-123">Possible values are: `unknown`, `remove`, `reset`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d4c2-124">Relações</span><span class="sxs-lookup"><span data-stu-id="9d4c2-124">Relationships</span></span>
<span data-ttu-id="9d4c2-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d4c2-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d4c2-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d4c2-126">JSON Representation</span></span>
<span data-ttu-id="9d4c2-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d4c2-127">Here is a JSON representation of the resource.</span></span>
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




