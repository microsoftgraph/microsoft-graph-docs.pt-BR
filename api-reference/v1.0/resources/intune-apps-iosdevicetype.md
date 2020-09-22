---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8044726067e7208fb5429c02262bf5e698139a14
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069047"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="9087a-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9087a-103">iosDeviceType resource type</span></span>

<span data-ttu-id="9087a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9087a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9087a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9087a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9087a-106">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="9087a-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="9087a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9087a-107">Properties</span></span>
|<span data-ttu-id="9087a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9087a-108">Property</span></span>|<span data-ttu-id="9087a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9087a-109">Type</span></span>|<span data-ttu-id="9087a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9087a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9087a-111">iPad</span><span class="sxs-lookup"><span data-stu-id="9087a-111">iPad</span></span>|<span data-ttu-id="9087a-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="9087a-112">Boolean</span></span>|<span data-ttu-id="9087a-113">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="9087a-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="9087a-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="9087a-114">iPhoneAndIPod</span></span>|<span data-ttu-id="9087a-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="9087a-115">Boolean</span></span>|<span data-ttu-id="9087a-116">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="9087a-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9087a-117">Relações</span><span class="sxs-lookup"><span data-stu-id="9087a-117">Relationships</span></span>
<span data-ttu-id="9087a-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9087a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9087a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9087a-119">JSON Representation</span></span>
<span data-ttu-id="9087a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9087a-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```









