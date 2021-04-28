---
title: Tipo de recurso deploymentSettings
description: Configurações controlar quando e como o serviço implanta uma atualização.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: f7c00ec8e880e7fd7ae9109fd1ac015868da902a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067794"
---
# <a name="deploymentsettings-resource-type"></a><span data-ttu-id="bd2a3-103">Tipo de recurso deploymentSettings</span><span class="sxs-lookup"><span data-stu-id="bd2a3-103">deploymentSettings resource type</span></span>

<span data-ttu-id="bd2a3-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="bd2a3-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd2a3-105">Configurações controlar quando e como o serviço implanta uma atualização.</span><span class="sxs-lookup"><span data-stu-id="bd2a3-105">Settings controlling when and how the service deploys an update.</span></span>

<span data-ttu-id="bd2a3-106">Tipo base [de windowsDeploymentSettings](../resources/windowsupdates-windowsdeploymentsettings.md).</span><span class="sxs-lookup"><span data-stu-id="bd2a3-106">Base type of [windowsDeploymentSettings](../resources/windowsupdates-windowsdeploymentsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bd2a3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd2a3-107">Properties</span></span>
|<span data-ttu-id="bd2a3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd2a3-108">Property</span></span>|<span data-ttu-id="bd2a3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd2a3-109">Type</span></span>|<span data-ttu-id="bd2a3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd2a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd2a3-111">monitoring</span><span class="sxs-lookup"><span data-stu-id="bd2a3-111">monitoring</span></span>|[<span data-ttu-id="bd2a3-112">microsoft.graph.windowsUpdates.monitoringSettings</span><span class="sxs-lookup"><span data-stu-id="bd2a3-112">microsoft.graph.windowsUpdates.monitoringSettings</span></span>](../resources/windowsupdates-monitoringsettings.md)|<span data-ttu-id="bd2a3-113">Configurações condições de controle para monitorar e automatizar ações a ser realizadas.</span><span class="sxs-lookup"><span data-stu-id="bd2a3-113">Settings governing conditions to monitor and automated actions to take.</span></span>|
|<span data-ttu-id="bd2a3-114">lançamento</span><span class="sxs-lookup"><span data-stu-id="bd2a3-114">rollout</span></span>|[<span data-ttu-id="bd2a3-115">microsoft.graph.windowsUpdates.rolloutSettings</span><span class="sxs-lookup"><span data-stu-id="bd2a3-115">microsoft.graph.windowsUpdates.rolloutSettings</span></span>](../resources/windowsupdates-rolloutsettings.md)|<span data-ttu-id="bd2a3-116">Configurações a forma como o conteúdo é lançado.</span><span class="sxs-lookup"><span data-stu-id="bd2a3-116">Settings governing how the content is rolled out.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd2a3-117">Relações</span><span class="sxs-lookup"><span data-stu-id="bd2a3-117">Relationships</span></span>
<span data-ttu-id="bd2a3-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd2a3-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd2a3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd2a3-119">JSON representation</span></span>
<span data-ttu-id="bd2a3-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd2a3-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentSettings",
  "rollout": {
    "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
  },
  "monitoring": {
    "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
  }
}
```

