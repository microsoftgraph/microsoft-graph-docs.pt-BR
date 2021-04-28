---
title: Tipo de recurso windowsDeploymentSettings
description: Configurações controlar quando e como o serviço implanta uma Windows 10 atualização.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: bc55f0643e789c802254064797bf8a5c2047cb64
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067234"
---
# <a name="windowsdeploymentsettings-resource-type"></a><span data-ttu-id="c5a1c-103">Tipo de recurso windowsDeploymentSettings</span><span class="sxs-lookup"><span data-stu-id="c5a1c-103">windowsDeploymentSettings resource type</span></span>

<span data-ttu-id="c5a1c-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c5a1c-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5a1c-105">Configurações controlar quando e como o serviço implanta uma Windows 10 atualização.</span><span class="sxs-lookup"><span data-stu-id="c5a1c-105">Settings controlling when and how the service deploys a Windows 10 update.</span></span>

<span data-ttu-id="c5a1c-106">Herda de [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span><span class="sxs-lookup"><span data-stu-id="c5a1c-106">Inherits from [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c5a1c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5a1c-107">Properties</span></span>
|<span data-ttu-id="c5a1c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5a1c-108">Property</span></span>|<span data-ttu-id="c5a1c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5a1c-109">Type</span></span>|<span data-ttu-id="c5a1c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5a1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a1c-111">monitoring</span><span class="sxs-lookup"><span data-stu-id="c5a1c-111">monitoring</span></span>|[<span data-ttu-id="c5a1c-112">microsoft.graph.windowsUpdates.monitoringSettings</span><span class="sxs-lookup"><span data-stu-id="c5a1c-112">microsoft.graph.windowsUpdates.monitoringSettings</span></span>](../resources/windowsupdates-monitoringsettings.md)|<span data-ttu-id="c5a1c-113">Configurações condições de controle para monitorar e automatizar ações a ser realizadas.</span><span class="sxs-lookup"><span data-stu-id="c5a1c-113">Settings governing conditions to monitor and automated actions to take.</span></span> <span data-ttu-id="c5a1c-114">Herdado [de deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span><span class="sxs-lookup"><span data-stu-id="c5a1c-114">Inherited from [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span></span>|
|<span data-ttu-id="c5a1c-115">lançamento</span><span class="sxs-lookup"><span data-stu-id="c5a1c-115">rollout</span></span>|[<span data-ttu-id="c5a1c-116">microsoft.graph.windowsUpdates.rolloutSettings</span><span class="sxs-lookup"><span data-stu-id="c5a1c-116">microsoft.graph.windowsUpdates.rolloutSettings</span></span>](../resources/windowsupdates-rolloutsettings.md)|<span data-ttu-id="c5a1c-117">Configurações a forma como o conteúdo é lançado. Herdado [de deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span><span class="sxs-lookup"><span data-stu-id="c5a1c-117">Settings governing how the content is rolled out. Inherited from [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span></span>|
|<span data-ttu-id="c5a1c-118">userExperience</span><span class="sxs-lookup"><span data-stu-id="c5a1c-118">userExperience</span></span>|[<span data-ttu-id="c5a1c-119">microsoft.graph.windowsUpdates.userExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c5a1c-119">microsoft.graph.windowsUpdates.userExperienceSettings</span></span>](../resources/windowsupdates-userexperiencesettings.md)|<span data-ttu-id="c5a1c-120">Configurações a experiência de atualização do usuário em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c5a1c-120">Settings governing the user's update experience on a device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5a1c-121">Relações</span><span class="sxs-lookup"><span data-stu-id="c5a1c-121">Relationships</span></span>
<span data-ttu-id="c5a1c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5a1c-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5a1c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5a1c-123">JSON representation</span></span>
<span data-ttu-id="c5a1c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5a1c-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windowsDeploymentSettings",
  "rollout": {
    "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
  },
  "monitoring": {
    "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
  },
  "userExperience": {
    "@odata.type": "microsoft.graph.windowsUpdates.userExperienceSettings"
  }
}
```

