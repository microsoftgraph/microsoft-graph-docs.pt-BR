---
title: tipo de recurso bulkManagedDeviceActionResult
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1f260b032078bdcd60000ecbde315a91cfcf492
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337591"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="453d6-103">tipo de recurso bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="453d6-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="453d6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="453d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="453d6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="453d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="453d6-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="453d6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="453d6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="453d6-107">Properties</span></span>
|<span data-ttu-id="453d6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="453d6-108">Property</span></span>|<span data-ttu-id="453d6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="453d6-109">Type</span></span>|<span data-ttu-id="453d6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="453d6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="453d6-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="453d6-111">successfulDeviceIds</span></span>|<span data-ttu-id="453d6-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="453d6-112">String collection</span></span>|<span data-ttu-id="453d6-113">Dispositivos bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="453d6-113">Successful devices</span></span>|
|<span data-ttu-id="453d6-114">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="453d6-114">failedDeviceIds</span></span>|<span data-ttu-id="453d6-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="453d6-115">String collection</span></span>|<span data-ttu-id="453d6-116">Dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="453d6-116">Failed devices</span></span>|
|<span data-ttu-id="453d6-117">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="453d6-117">notFoundDeviceIds</span></span>|<span data-ttu-id="453d6-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="453d6-118">String collection</span></span>|<span data-ttu-id="453d6-119">Dispositivos não encontrados</span><span class="sxs-lookup"><span data-stu-id="453d6-119">Not found devices</span></span>|
|<span data-ttu-id="453d6-120">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="453d6-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="453d6-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="453d6-121">String collection</span></span>|<span data-ttu-id="453d6-122">Dispositivos não suportados</span><span class="sxs-lookup"><span data-stu-id="453d6-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="453d6-123">Relações</span><span class="sxs-lookup"><span data-stu-id="453d6-123">Relationships</span></span>
<span data-ttu-id="453d6-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="453d6-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="453d6-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="453d6-125">JSON Representation</span></span>
<span data-ttu-id="453d6-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="453d6-126">Here is a JSON representation of the resource.</span></span>
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



