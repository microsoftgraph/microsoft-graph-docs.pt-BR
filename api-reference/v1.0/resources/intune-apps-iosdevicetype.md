---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 522ca687f9169066575d1bd8fb3db1e4345d9981
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755599"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="b9e12-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b9e12-103">iosDeviceType resource type</span></span>

<span data-ttu-id="b9e12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9e12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9e12-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9e12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9e12-106">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="b9e12-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="b9e12-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9e12-107">Properties</span></span>
|<span data-ttu-id="b9e12-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9e12-108">Property</span></span>|<span data-ttu-id="b9e12-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9e12-109">Type</span></span>|<span data-ttu-id="b9e12-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9e12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9e12-111">iPad</span><span class="sxs-lookup"><span data-stu-id="b9e12-111">iPad</span></span>|<span data-ttu-id="b9e12-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="b9e12-112">Boolean</span></span>|<span data-ttu-id="b9e12-113">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="b9e12-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="b9e12-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="b9e12-114">iPhoneAndIPod</span></span>|<span data-ttu-id="b9e12-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="b9e12-115">Boolean</span></span>|<span data-ttu-id="b9e12-116">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="b9e12-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9e12-117">Relações</span><span class="sxs-lookup"><span data-stu-id="b9e12-117">Relationships</span></span>
<span data-ttu-id="b9e12-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b9e12-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9e12-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9e12-119">JSON Representation</span></span>
<span data-ttu-id="b9e12-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9e12-120">Here is a JSON representation of the resource.</span></span>
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




