---
title: tipo de recurso bulkManagedDeviceActionResult
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 330972424697aed731cd3f1a646505c51cd3f52c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528702"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="ae265-103">tipo de recurso bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="ae265-103">bulkManagedDeviceActionResult resource type</span></span>

<span data-ttu-id="ae265-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ae265-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae265-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae265-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae265-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae265-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae265-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ae265-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ae265-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae265-108">Properties</span></span>
|<span data-ttu-id="ae265-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae265-109">Property</span></span>|<span data-ttu-id="ae265-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae265-110">Type</span></span>|<span data-ttu-id="ae265-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae265-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae265-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="ae265-112">successfulDeviceIds</span></span>|<span data-ttu-id="ae265-113">String collection</span><span class="sxs-lookup"><span data-stu-id="ae265-113">String collection</span></span>|<span data-ttu-id="ae265-114">Dispositivos bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="ae265-114">Successful devices</span></span>|
|<span data-ttu-id="ae265-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="ae265-115">failedDeviceIds</span></span>|<span data-ttu-id="ae265-116">String collection</span><span class="sxs-lookup"><span data-stu-id="ae265-116">String collection</span></span>|<span data-ttu-id="ae265-117">Dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="ae265-117">Failed devices</span></span>|
|<span data-ttu-id="ae265-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="ae265-118">notFoundDeviceIds</span></span>|<span data-ttu-id="ae265-119">String collection</span><span class="sxs-lookup"><span data-stu-id="ae265-119">String collection</span></span>|<span data-ttu-id="ae265-120">Dispositivos não encontrados</span><span class="sxs-lookup"><span data-stu-id="ae265-120">Not found devices</span></span>|
|<span data-ttu-id="ae265-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="ae265-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="ae265-122">String collection</span><span class="sxs-lookup"><span data-stu-id="ae265-122">String collection</span></span>|<span data-ttu-id="ae265-123">Dispositivos não suportados</span><span class="sxs-lookup"><span data-stu-id="ae265-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae265-124">Relações</span><span class="sxs-lookup"><span data-stu-id="ae265-124">Relationships</span></span>
<span data-ttu-id="ae265-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae265-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae265-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae265-126">JSON Representation</span></span>
<span data-ttu-id="ae265-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae265-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "successfulDeviceIds": [
    "String"
  ],
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ]
}
```



