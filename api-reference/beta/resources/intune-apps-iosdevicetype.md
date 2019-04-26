---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 121e297355d0d5734f7c4e23087bf14773c598c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553061"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="a5abb-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="a5abb-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="a5abb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a5abb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5abb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5abb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5abb-106">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="a5abb-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="a5abb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5abb-107">Properties</span></span>
|<span data-ttu-id="a5abb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5abb-108">Property</span></span>|<span data-ttu-id="a5abb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5abb-109">Type</span></span>|<span data-ttu-id="a5abb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5abb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5abb-111">iPad</span><span class="sxs-lookup"><span data-stu-id="a5abb-111">iPad</span></span>|<span data-ttu-id="a5abb-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5abb-112">Boolean</span></span>|<span data-ttu-id="a5abb-113">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="a5abb-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="a5abb-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="a5abb-114">iPhoneAndIPod</span></span>|<span data-ttu-id="a5abb-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5abb-115">Boolean</span></span>|<span data-ttu-id="a5abb-116">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="a5abb-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5abb-117">Relações</span><span class="sxs-lookup"><span data-stu-id="a5abb-117">Relationships</span></span>
<span data-ttu-id="a5abb-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5abb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5abb-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5abb-119">JSON Representation</span></span>
<span data-ttu-id="a5abb-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5abb-120">Here is a JSON representation of the resource.</span></span>
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





