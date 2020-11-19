---
title: tipo de recurso managedDeviceSummarizedAppState
description: Evento representando os dispositivos de um usuário com falha ou aplicativos pendentes.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4727477497657a917906f9b778fa76647fc394d9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271601"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="d28a3-103">tipo de recurso managedDeviceSummarizedAppState</span><span class="sxs-lookup"><span data-stu-id="d28a3-103">managedDeviceSummarizedAppState resource type</span></span>

<span data-ttu-id="d28a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d28a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d28a3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d28a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d28a3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d28a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d28a3-107">Evento representando os dispositivos de um usuário com falha ou aplicativos pendentes.</span><span class="sxs-lookup"><span data-stu-id="d28a3-107">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="d28a3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d28a3-108">Properties</span></span>
|<span data-ttu-id="d28a3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d28a3-109">Property</span></span>|<span data-ttu-id="d28a3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d28a3-110">Type</span></span>|<span data-ttu-id="d28a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d28a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d28a3-112">summarizedAppState</span><span class="sxs-lookup"><span data-stu-id="d28a3-112">summarizedAppState</span></span>|[<span data-ttu-id="d28a3-113">runState</span><span class="sxs-lookup"><span data-stu-id="d28a3-113">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="d28a3-114">runState para o objeto.</span><span class="sxs-lookup"><span data-stu-id="d28a3-114">runState for the object.</span></span> <span data-ttu-id="d28a3-115">Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="d28a3-115">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="d28a3-116">deviceId</span><span class="sxs-lookup"><span data-stu-id="d28a3-116">deviceId</span></span>|<span data-ttu-id="d28a3-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d28a3-117">String</span></span>|<span data-ttu-id="d28a3-118">DeviceID do dispositivo representado por este objeto</span><span class="sxs-lookup"><span data-stu-id="d28a3-118">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="d28a3-119">Relações</span><span class="sxs-lookup"><span data-stu-id="d28a3-119">Relationships</span></span>
<span data-ttu-id="d28a3-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d28a3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d28a3-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d28a3-121">JSON Representation</span></span>
<span data-ttu-id="d28a3-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d28a3-122">Here is a JSON representation of the resource.</span></span>
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




