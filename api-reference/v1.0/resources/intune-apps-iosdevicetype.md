---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f3bd1d0aff7e09d5828496de348805075d0b330
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503524"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="88f66-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="88f66-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="88f66-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88f66-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88f66-105">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="88f66-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="88f66-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88f66-106">Properties</span></span>
|<span data-ttu-id="88f66-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88f66-107">Property</span></span>|<span data-ttu-id="88f66-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="88f66-108">Type</span></span>|<span data-ttu-id="88f66-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="88f66-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88f66-110">iPad</span><span class="sxs-lookup"><span data-stu-id="88f66-110">iPad</span></span>|<span data-ttu-id="88f66-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="88f66-111">Boolean</span></span>|<span data-ttu-id="88f66-112">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="88f66-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="88f66-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="88f66-113">iPhoneAndIPod</span></span>|<span data-ttu-id="88f66-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="88f66-114">Boolean</span></span>|<span data-ttu-id="88f66-115">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="88f66-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88f66-116">Relações</span><span class="sxs-lookup"><span data-stu-id="88f66-116">Relationships</span></span>
<span data-ttu-id="88f66-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="88f66-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88f66-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88f66-118">JSON Representation</span></span>
<span data-ttu-id="88f66-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88f66-119">Here is a JSON representation of the resource.</span></span>
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



