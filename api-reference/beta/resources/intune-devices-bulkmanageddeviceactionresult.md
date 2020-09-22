---
title: tipo de recurso bulkManagedDeviceActionResult
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97b56db5eb906d16b344e9e8c0a2bbb920cf5e46
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060837"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="b15de-103">tipo de recurso bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="b15de-103">bulkManagedDeviceActionResult resource type</span></span>

<span data-ttu-id="b15de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b15de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b15de-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b15de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b15de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b15de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b15de-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b15de-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b15de-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b15de-108">Properties</span></span>
|<span data-ttu-id="b15de-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b15de-109">Property</span></span>|<span data-ttu-id="b15de-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b15de-110">Type</span></span>|<span data-ttu-id="b15de-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b15de-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b15de-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="b15de-112">successfulDeviceIds</span></span>|<span data-ttu-id="b15de-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b15de-113">String collection</span></span>|<span data-ttu-id="b15de-114">Dispositivos bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="b15de-114">Successful devices</span></span>|
|<span data-ttu-id="b15de-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="b15de-115">failedDeviceIds</span></span>|<span data-ttu-id="b15de-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b15de-116">String collection</span></span>|<span data-ttu-id="b15de-117">Dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="b15de-117">Failed devices</span></span>|
|<span data-ttu-id="b15de-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="b15de-118">notFoundDeviceIds</span></span>|<span data-ttu-id="b15de-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b15de-119">String collection</span></span>|<span data-ttu-id="b15de-120">Dispositivos não encontrados</span><span class="sxs-lookup"><span data-stu-id="b15de-120">Not found devices</span></span>|
|<span data-ttu-id="b15de-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="b15de-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="b15de-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b15de-122">String collection</span></span>|<span data-ttu-id="b15de-123">Dispositivos não suportados</span><span class="sxs-lookup"><span data-stu-id="b15de-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="b15de-124">Relações</span><span class="sxs-lookup"><span data-stu-id="b15de-124">Relationships</span></span>
<span data-ttu-id="b15de-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b15de-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b15de-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b15de-126">JSON Representation</span></span>
<span data-ttu-id="b15de-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b15de-127">Here is a JSON representation of the resource.</span></span>
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






