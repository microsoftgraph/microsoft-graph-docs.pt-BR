---
title: tipo de recurso managedDeviceSummarizedAppState
description: Evento representando os dispositivos de um usuário com falha ou aplicativos pendentes.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 957d25e9b5dfe333529f228eecddb937b1752c2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43385712"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="01093-103">tipo de recurso managedDeviceSummarizedAppState</span><span class="sxs-lookup"><span data-stu-id="01093-103">managedDeviceSummarizedAppState resource type</span></span>

<span data-ttu-id="01093-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01093-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01093-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01093-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01093-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01093-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01093-107">Evento representando os dispositivos de um usuário com falha ou aplicativos pendentes.</span><span class="sxs-lookup"><span data-stu-id="01093-107">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="01093-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01093-108">Properties</span></span>
|<span data-ttu-id="01093-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01093-109">Property</span></span>|<span data-ttu-id="01093-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="01093-110">Type</span></span>|<span data-ttu-id="01093-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="01093-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01093-112">summarizedAppState</span><span class="sxs-lookup"><span data-stu-id="01093-112">summarizedAppState</span></span>|[<span data-ttu-id="01093-113">runState</span><span class="sxs-lookup"><span data-stu-id="01093-113">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="01093-114">runState para o objeto.</span><span class="sxs-lookup"><span data-stu-id="01093-114">runState for the object.</span></span> <span data-ttu-id="01093-115">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="01093-115">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="01093-116">deviceId</span><span class="sxs-lookup"><span data-stu-id="01093-116">deviceId</span></span>|<span data-ttu-id="01093-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01093-117">String</span></span>|<span data-ttu-id="01093-118">DeviceID do dispositivo representado por este objeto</span><span class="sxs-lookup"><span data-stu-id="01093-118">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="01093-119">Relações</span><span class="sxs-lookup"><span data-stu-id="01093-119">Relationships</span></span>
<span data-ttu-id="01093-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="01093-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01093-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01093-121">JSON Representation</span></span>
<span data-ttu-id="01093-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01093-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceSummarizedAppState",
  "summarizedAppState": "String",
  "deviceId": "String"
}
```



