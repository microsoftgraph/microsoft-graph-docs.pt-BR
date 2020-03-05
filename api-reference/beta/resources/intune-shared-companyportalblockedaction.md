---
title: tipo de recurso companyPortalBlockedAction
description: Ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 15460de0c53b1b7b383095b7bee50af0192b3462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527481"
---
# <a name="companyportalblockedaction-resource-type"></a><span data-ttu-id="42e7f-103">tipo de recurso companyPortalBlockedAction</span><span class="sxs-lookup"><span data-stu-id="42e7f-103">companyPortalBlockedAction resource type</span></span>

<span data-ttu-id="42e7f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="42e7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42e7f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42e7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42e7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42e7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42e7f-107">Ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo</span><span class="sxs-lookup"><span data-stu-id="42e7f-107">Blocked actions on the company portal as per platform and device ownership types</span></span>

## <a name="properties"></a><span data-ttu-id="42e7f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42e7f-108">Properties</span></span>
|<span data-ttu-id="42e7f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42e7f-109">Property</span></span>|<span data-ttu-id="42e7f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="42e7f-110">Type</span></span>|<span data-ttu-id="42e7f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42e7f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42e7f-112">platform</span><span class="sxs-lookup"><span data-stu-id="42e7f-112">platform</span></span>|[<span data-ttu-id="42e7f-113">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="42e7f-113">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="42e7f-114">Sistema operacional/plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42e7f-114">Device OS/Platform.</span></span> <span data-ttu-id="42e7f-115">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="42e7f-115">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="42e7f-116">ownerType</span><span class="sxs-lookup"><span data-stu-id="42e7f-116">ownerType</span></span>|[<span data-ttu-id="42e7f-117">ownerType</span><span class="sxs-lookup"><span data-stu-id="42e7f-117">ownerType</span></span>](../resources/intune-shared-ownertype.md)|<span data-ttu-id="42e7f-118">Tipo de propriedade de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42e7f-118">Device ownership type.</span></span> <span data-ttu-id="42e7f-119">Os valores possíveis são: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="42e7f-119">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="42e7f-120">ação</span><span class="sxs-lookup"><span data-stu-id="42e7f-120">action</span></span>|[<span data-ttu-id="42e7f-121">companyPortalAction</span><span class="sxs-lookup"><span data-stu-id="42e7f-121">companyPortalAction</span></span>](../resources/intune-shared-companyportalaction.md)|<span data-ttu-id="42e7f-122">Ação de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42e7f-122">Device Action.</span></span> <span data-ttu-id="42e7f-123">Os valores possíveis são: `unknown`, `remove`, `reset`.</span><span class="sxs-lookup"><span data-stu-id="42e7f-123">Possible values are: `unknown`, `remove`, `reset`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42e7f-124">Relações</span><span class="sxs-lookup"><span data-stu-id="42e7f-124">Relationships</span></span>
<span data-ttu-id="42e7f-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42e7f-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42e7f-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42e7f-126">JSON Representation</span></span>
<span data-ttu-id="42e7f-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42e7f-127">Here is a JSON representation of the resource.</span></span>
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



