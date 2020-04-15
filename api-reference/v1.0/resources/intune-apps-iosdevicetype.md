---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77533c24fe08d6d949c2b50776c92295ac2ad0d1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397288"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="10785-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="10785-103">iosDeviceType resource type</span></span>

<span data-ttu-id="10785-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10785-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10785-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10785-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10785-106">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="10785-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="10785-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10785-107">Properties</span></span>
|<span data-ttu-id="10785-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10785-108">Property</span></span>|<span data-ttu-id="10785-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="10785-109">Type</span></span>|<span data-ttu-id="10785-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="10785-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10785-111">iPad</span><span class="sxs-lookup"><span data-stu-id="10785-111">iPad</span></span>|<span data-ttu-id="10785-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="10785-112">Boolean</span></span>|<span data-ttu-id="10785-113">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="10785-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="10785-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="10785-114">iPhoneAndIPod</span></span>|<span data-ttu-id="10785-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="10785-115">Boolean</span></span>|<span data-ttu-id="10785-116">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="10785-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10785-117">Relações</span><span class="sxs-lookup"><span data-stu-id="10785-117">Relationships</span></span>
<span data-ttu-id="10785-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10785-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10785-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10785-119">JSON Representation</span></span>
<span data-ttu-id="10785-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10785-120">Here is a JSON representation of the resource.</span></span>
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







