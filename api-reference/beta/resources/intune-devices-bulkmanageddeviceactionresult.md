---
title: tipo de recurso de bulkManagedDeviceActionResult
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: adc2b2a6b139ad428cb191fe45a3ca7f4192092a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981774"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="c217d-103">tipo de recurso de bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="c217d-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="c217d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c217d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c217d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c217d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c217d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c217d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c217d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c217d-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c217d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c217d-108">Properties</span></span>
|<span data-ttu-id="c217d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c217d-109">Property</span></span>|<span data-ttu-id="c217d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c217d-110">Type</span></span>|<span data-ttu-id="c217d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c217d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c217d-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="c217d-112">successfulDeviceIds</span></span>|<span data-ttu-id="c217d-113">String collection</span><span class="sxs-lookup"><span data-stu-id="c217d-113">String collection</span></span>|<span data-ttu-id="c217d-114">Dispositivos bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="c217d-114">Successful devices</span></span>|
|<span data-ttu-id="c217d-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="c217d-115">failedDeviceIds</span></span>|<span data-ttu-id="c217d-116">String collection</span><span class="sxs-lookup"><span data-stu-id="c217d-116">String collection</span></span>|<span data-ttu-id="c217d-117">Dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="c217d-117">Failed devices</span></span>|
|<span data-ttu-id="c217d-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="c217d-118">notFoundDeviceIds</span></span>|<span data-ttu-id="c217d-119">String collection</span><span class="sxs-lookup"><span data-stu-id="c217d-119">String collection</span></span>|<span data-ttu-id="c217d-120">Não encontrado dispositivos</span><span class="sxs-lookup"><span data-stu-id="c217d-120">Not found devices</span></span>|
|<span data-ttu-id="c217d-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="c217d-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="c217d-122">String collection</span><span class="sxs-lookup"><span data-stu-id="c217d-122">String collection</span></span>|<span data-ttu-id="c217d-123">Dispositivos não suportados</span><span class="sxs-lookup"><span data-stu-id="c217d-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c217d-124">Relações</span><span class="sxs-lookup"><span data-stu-id="c217d-124">Relationships</span></span>
<span data-ttu-id="c217d-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c217d-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c217d-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c217d-126">JSON Representation</span></span>
<span data-ttu-id="c217d-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c217d-127">Here is a JSON representation of the resource.</span></span>
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





