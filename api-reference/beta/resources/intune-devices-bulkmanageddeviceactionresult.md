---
title: tipo de recurso bulkManagedDeviceActionResult
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e6993d7b55397320ad8cae8d669db59651827235
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725516"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="1c9d3-103">tipo de recurso bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="1c9d3-103">bulkManagedDeviceActionResult resource type</span></span>

<span data-ttu-id="1c9d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c9d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c9d3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c9d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c9d3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c9d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c9d3-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1c9d3-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1c9d3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c9d3-108">Properties</span></span>
|<span data-ttu-id="1c9d3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c9d3-109">Property</span></span>|<span data-ttu-id="1c9d3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c9d3-110">Type</span></span>|<span data-ttu-id="1c9d3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c9d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c9d3-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="1c9d3-112">successfulDeviceIds</span></span>|<span data-ttu-id="1c9d3-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c9d3-113">String collection</span></span>|<span data-ttu-id="1c9d3-114">Dispositivos bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="1c9d3-114">Successful devices</span></span>|
|<span data-ttu-id="1c9d3-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="1c9d3-115">failedDeviceIds</span></span>|<span data-ttu-id="1c9d3-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c9d3-116">String collection</span></span>|<span data-ttu-id="1c9d3-117">Dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="1c9d3-117">Failed devices</span></span>|
|<span data-ttu-id="1c9d3-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="1c9d3-118">notFoundDeviceIds</span></span>|<span data-ttu-id="1c9d3-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c9d3-119">String collection</span></span>|<span data-ttu-id="1c9d3-120">Dispositivos não encontrados</span><span class="sxs-lookup"><span data-stu-id="1c9d3-120">Not found devices</span></span>|
|<span data-ttu-id="1c9d3-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="1c9d3-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="1c9d3-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c9d3-122">String collection</span></span>|<span data-ttu-id="1c9d3-123">Dispositivos não suportados</span><span class="sxs-lookup"><span data-stu-id="1c9d3-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c9d3-124">Relações</span><span class="sxs-lookup"><span data-stu-id="1c9d3-124">Relationships</span></span>
<span data-ttu-id="1c9d3-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c9d3-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c9d3-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c9d3-126">JSON Representation</span></span>
<span data-ttu-id="1c9d3-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c9d3-127">Here is a JSON representation of the resource.</span></span>
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





