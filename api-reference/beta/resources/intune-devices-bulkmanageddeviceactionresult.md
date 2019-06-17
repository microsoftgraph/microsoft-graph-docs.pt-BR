---
title: tipo de recurso bulkManagedDeviceActionResult
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8190071f5ed6e239c2452bc53d802125b71339f5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983362"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="8c0c3-103">tipo de recurso bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="8c0c3-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="8c0c3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c0c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c0c3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c0c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c0c3-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8c0c3-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8c0c3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c0c3-107">Properties</span></span>
|<span data-ttu-id="8c0c3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c0c3-108">Property</span></span>|<span data-ttu-id="8c0c3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c0c3-109">Type</span></span>|<span data-ttu-id="8c0c3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c0c3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c0c3-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="8c0c3-111">successfulDeviceIds</span></span>|<span data-ttu-id="8c0c3-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c0c3-112">String collection</span></span>|<span data-ttu-id="8c0c3-113">Dispositivos bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="8c0c3-113">Successful devices</span></span>|
|<span data-ttu-id="8c0c3-114">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="8c0c3-114">failedDeviceIds</span></span>|<span data-ttu-id="8c0c3-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c0c3-115">String collection</span></span>|<span data-ttu-id="8c0c3-116">Dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="8c0c3-116">Failed devices</span></span>|
|<span data-ttu-id="8c0c3-117">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="8c0c3-117">notFoundDeviceIds</span></span>|<span data-ttu-id="8c0c3-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c0c3-118">String collection</span></span>|<span data-ttu-id="8c0c3-119">Dispositivos não encontrados</span><span class="sxs-lookup"><span data-stu-id="8c0c3-119">Not found devices</span></span>|
|<span data-ttu-id="8c0c3-120">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="8c0c3-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="8c0c3-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c0c3-121">String collection</span></span>|<span data-ttu-id="8c0c3-122">Dispositivos não suportados</span><span class="sxs-lookup"><span data-stu-id="8c0c3-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c0c3-123">Relações</span><span class="sxs-lookup"><span data-stu-id="8c0c3-123">Relationships</span></span>
<span data-ttu-id="8c0c3-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c0c3-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c0c3-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c0c3-125">JSON Representation</span></span>
<span data-ttu-id="8c0c3-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c0c3-126">Here is a JSON representation of the resource.</span></span>
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





