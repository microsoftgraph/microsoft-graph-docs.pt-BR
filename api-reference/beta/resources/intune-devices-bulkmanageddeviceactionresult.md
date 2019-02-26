---
title: tipo de recurso bulkManagedDeviceActionResult
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 199fe08b4eaf339f17fdb67bb6dbcc0243fd90f9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168331"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="2d165-103">tipo de recurso bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="2d165-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="2d165-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d165-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d165-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d165-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d165-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2d165-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2d165-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d165-107">Properties</span></span>
|<span data-ttu-id="2d165-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d165-108">Property</span></span>|<span data-ttu-id="2d165-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d165-109">Type</span></span>|<span data-ttu-id="2d165-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d165-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d165-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="2d165-111">successfulDeviceIds</span></span>|<span data-ttu-id="2d165-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d165-112">String collection</span></span>|<span data-ttu-id="2d165-113">Dispositivos bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="2d165-113">Successful devices</span></span>|
|<span data-ttu-id="2d165-114">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="2d165-114">failedDeviceIds</span></span>|<span data-ttu-id="2d165-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d165-115">String collection</span></span>|<span data-ttu-id="2d165-116">Dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="2d165-116">Failed devices</span></span>|
|<span data-ttu-id="2d165-117">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="2d165-117">notFoundDeviceIds</span></span>|<span data-ttu-id="2d165-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d165-118">String collection</span></span>|<span data-ttu-id="2d165-119">Dispositivos não encontrados</span><span class="sxs-lookup"><span data-stu-id="2d165-119">Not found devices</span></span>|
|<span data-ttu-id="2d165-120">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="2d165-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="2d165-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d165-121">String collection</span></span>|<span data-ttu-id="2d165-122">Dispositivos não suportados</span><span class="sxs-lookup"><span data-stu-id="2d165-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d165-123">Relações</span><span class="sxs-lookup"><span data-stu-id="2d165-123">Relationships</span></span>
<span data-ttu-id="2d165-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d165-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d165-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d165-125">JSON Representation</span></span>
<span data-ttu-id="2d165-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d165-126">Here is a JSON representation of the resource.</span></span>
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




