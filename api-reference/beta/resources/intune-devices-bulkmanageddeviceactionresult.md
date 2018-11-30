---
title: tipo de recurso de bulkManagedDeviceActionResult
description: Ainda não documentado
ms.openlocfilehash: 856054f293dca0ae86681246d4783aae6a0373c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036766"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="31682-103">tipo de recurso de bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="31682-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="31682-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="31682-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31682-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="31682-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31682-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="31682-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31682-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="31682-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="31682-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31682-108">Properties</span></span>
|<span data-ttu-id="31682-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31682-109">Property</span></span>|<span data-ttu-id="31682-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="31682-110">Type</span></span>|<span data-ttu-id="31682-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="31682-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31682-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="31682-112">successfulDeviceIds</span></span>|<span data-ttu-id="31682-113">String collection</span><span class="sxs-lookup"><span data-stu-id="31682-113">String collection</span></span>|<span data-ttu-id="31682-114">Dispositivos bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="31682-114">Successful devices</span></span>|
|<span data-ttu-id="31682-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="31682-115">failedDeviceIds</span></span>|<span data-ttu-id="31682-116">String collection</span><span class="sxs-lookup"><span data-stu-id="31682-116">String collection</span></span>|<span data-ttu-id="31682-117">Dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="31682-117">Failed devices</span></span>|
|<span data-ttu-id="31682-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="31682-118">notFoundDeviceIds</span></span>|<span data-ttu-id="31682-119">String collection</span><span class="sxs-lookup"><span data-stu-id="31682-119">String collection</span></span>|<span data-ttu-id="31682-120">Não encontrado dispositivos</span><span class="sxs-lookup"><span data-stu-id="31682-120">Not found devices</span></span>|
|<span data-ttu-id="31682-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="31682-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="31682-122">String collection</span><span class="sxs-lookup"><span data-stu-id="31682-122">String collection</span></span>|<span data-ttu-id="31682-123">Dispositivos não suportados</span><span class="sxs-lookup"><span data-stu-id="31682-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="31682-124">Relações</span><span class="sxs-lookup"><span data-stu-id="31682-124">Relationships</span></span>
<span data-ttu-id="31682-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31682-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31682-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31682-126">JSON Representation</span></span>
<span data-ttu-id="31682-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31682-127">Here is a JSON representation of the resource.</span></span>
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





