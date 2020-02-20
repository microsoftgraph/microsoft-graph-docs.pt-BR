---
title: tipo de recurso managedDeviceSummarizedAppState
description: Evento representando os dispositivos de um usuário com falha ou aplicativos pendentes.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 76020e9028207d15cf198d9c4401abc4819a1ffd
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160785"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="06b56-103">tipo de recurso managedDeviceSummarizedAppState</span><span class="sxs-lookup"><span data-stu-id="06b56-103">managedDeviceSummarizedAppState resource type</span></span>

> <span data-ttu-id="06b56-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06b56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06b56-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06b56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06b56-106">Evento representando os dispositivos de um usuário com falha ou aplicativos pendentes.</span><span class="sxs-lookup"><span data-stu-id="06b56-106">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="06b56-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06b56-107">Properties</span></span>
|<span data-ttu-id="06b56-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06b56-108">Property</span></span>|<span data-ttu-id="06b56-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="06b56-109">Type</span></span>|<span data-ttu-id="06b56-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="06b56-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06b56-111">summarizedAppState</span><span class="sxs-lookup"><span data-stu-id="06b56-111">summarizedAppState</span></span>|[<span data-ttu-id="06b56-112">runState</span><span class="sxs-lookup"><span data-stu-id="06b56-112">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="06b56-113">runState para o objeto.</span><span class="sxs-lookup"><span data-stu-id="06b56-113">runState for the object.</span></span> <span data-ttu-id="06b56-114">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="06b56-114">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="06b56-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="06b56-115">deviceId</span></span>|<span data-ttu-id="06b56-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06b56-116">String</span></span>|<span data-ttu-id="06b56-117">DeviceID do dispositivo representado por este objeto</span><span class="sxs-lookup"><span data-stu-id="06b56-117">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="06b56-118">Relações</span><span class="sxs-lookup"><span data-stu-id="06b56-118">Relationships</span></span>
<span data-ttu-id="06b56-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06b56-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06b56-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06b56-120">JSON Representation</span></span>
<span data-ttu-id="06b56-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06b56-121">Here is a JSON representation of the resource.</span></span>
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



