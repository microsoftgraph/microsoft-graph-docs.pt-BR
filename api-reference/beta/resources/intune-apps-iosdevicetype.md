---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b68c7ce163dbf0f9232bf53d919ae84c7906c997
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395381"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="8a011-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="8a011-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="8a011-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="8a011-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8a011-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8a011-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a011-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="8a011-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a011-107">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="8a011-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="8a011-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a011-108">Properties</span></span>
|<span data-ttu-id="8a011-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a011-109">Property</span></span>|<span data-ttu-id="8a011-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a011-110">Type</span></span>|<span data-ttu-id="8a011-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a011-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a011-112">iPad</span><span class="sxs-lookup"><span data-stu-id="8a011-112">iPad</span></span>|<span data-ttu-id="8a011-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a011-113">Boolean</span></span>|<span data-ttu-id="8a011-114">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="8a011-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="8a011-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="8a011-115">iPhoneAndIPod</span></span>|<span data-ttu-id="8a011-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a011-116">Boolean</span></span>|<span data-ttu-id="8a011-117">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="8a011-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a011-118">Relações</span><span class="sxs-lookup"><span data-stu-id="8a011-118">Relationships</span></span>
<span data-ttu-id="8a011-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a011-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a011-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a011-120">JSON Representation</span></span>
<span data-ttu-id="8a011-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8a011-121">Here is a JSON representation of the resource.</span></span>
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




