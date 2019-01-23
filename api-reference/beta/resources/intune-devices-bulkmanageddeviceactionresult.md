---
title: tipo de recurso de bulkManagedDeviceActionResult
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d1b23efdb5b8eed16c6c66d72a13efaef9e38d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425838"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="3dffb-103">tipo de recurso de bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="3dffb-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="3dffb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="3dffb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3dffb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3dffb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3dffb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="3dffb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dffb-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3dffb-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3dffb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3dffb-108">Properties</span></span>
|<span data-ttu-id="3dffb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3dffb-109">Property</span></span>|<span data-ttu-id="3dffb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3dffb-110">Type</span></span>|<span data-ttu-id="3dffb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3dffb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dffb-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="3dffb-112">successfulDeviceIds</span></span>|<span data-ttu-id="3dffb-113">String collection</span><span class="sxs-lookup"><span data-stu-id="3dffb-113">String collection</span></span>|<span data-ttu-id="3dffb-114">Dispositivos bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="3dffb-114">Successful devices</span></span>|
|<span data-ttu-id="3dffb-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="3dffb-115">failedDeviceIds</span></span>|<span data-ttu-id="3dffb-116">String collection</span><span class="sxs-lookup"><span data-stu-id="3dffb-116">String collection</span></span>|<span data-ttu-id="3dffb-117">Dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="3dffb-117">Failed devices</span></span>|
|<span data-ttu-id="3dffb-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="3dffb-118">notFoundDeviceIds</span></span>|<span data-ttu-id="3dffb-119">String collection</span><span class="sxs-lookup"><span data-stu-id="3dffb-119">String collection</span></span>|<span data-ttu-id="3dffb-120">Não encontrado dispositivos</span><span class="sxs-lookup"><span data-stu-id="3dffb-120">Not found devices</span></span>|
|<span data-ttu-id="3dffb-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="3dffb-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="3dffb-122">String collection</span><span class="sxs-lookup"><span data-stu-id="3dffb-122">String collection</span></span>|<span data-ttu-id="3dffb-123">Dispositivos não suportados</span><span class="sxs-lookup"><span data-stu-id="3dffb-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="3dffb-124">Relações</span><span class="sxs-lookup"><span data-stu-id="3dffb-124">Relationships</span></span>
<span data-ttu-id="3dffb-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3dffb-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3dffb-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3dffb-126">JSON Representation</span></span>
<span data-ttu-id="3dffb-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3dffb-127">Here is a JSON representation of the resource.</span></span>
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




