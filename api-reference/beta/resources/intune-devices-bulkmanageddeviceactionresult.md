---
title: tipo de recurso bulkManagedDeviceActionResult
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a7b5e719e837dbd175fa634aea2082f5b0b142b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999987"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="8965e-103">tipo de recurso bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="8965e-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="8965e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8965e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8965e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8965e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8965e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8965e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8965e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8965e-107">Properties</span></span>
|<span data-ttu-id="8965e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8965e-108">Property</span></span>|<span data-ttu-id="8965e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8965e-109">Type</span></span>|<span data-ttu-id="8965e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8965e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8965e-111">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="8965e-111">successfulDeviceIds</span></span>|<span data-ttu-id="8965e-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8965e-112">String collection</span></span>|<span data-ttu-id="8965e-113">Dispositivos bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="8965e-113">Successful devices</span></span>|
|<span data-ttu-id="8965e-114">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="8965e-114">failedDeviceIds</span></span>|<span data-ttu-id="8965e-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8965e-115">String collection</span></span>|<span data-ttu-id="8965e-116">Dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="8965e-116">Failed devices</span></span>|
|<span data-ttu-id="8965e-117">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="8965e-117">notFoundDeviceIds</span></span>|<span data-ttu-id="8965e-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8965e-118">String collection</span></span>|<span data-ttu-id="8965e-119">Dispositivos não encontrados</span><span class="sxs-lookup"><span data-stu-id="8965e-119">Not found devices</span></span>|
|<span data-ttu-id="8965e-120">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="8965e-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="8965e-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8965e-121">String collection</span></span>|<span data-ttu-id="8965e-122">Dispositivos não suportados</span><span class="sxs-lookup"><span data-stu-id="8965e-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="8965e-123">Relações</span><span class="sxs-lookup"><span data-stu-id="8965e-123">Relationships</span></span>
<span data-ttu-id="8965e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8965e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8965e-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8965e-125">JSON Representation</span></span>
<span data-ttu-id="8965e-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8965e-126">Here is a JSON representation of the resource.</span></span>
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





