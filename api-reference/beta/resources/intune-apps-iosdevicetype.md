---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2fe1f686052468bbab5d7115541a631b77073d6e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977161"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="0c273-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="0c273-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="0c273-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0c273-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c273-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0c273-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c273-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0c273-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c273-107">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="0c273-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="0c273-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c273-108">Properties</span></span>
|<span data-ttu-id="0c273-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c273-109">Property</span></span>|<span data-ttu-id="0c273-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c273-110">Type</span></span>|<span data-ttu-id="0c273-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c273-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c273-112">iPad</span><span class="sxs-lookup"><span data-stu-id="0c273-112">iPad</span></span>|<span data-ttu-id="0c273-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="0c273-113">Boolean</span></span>|<span data-ttu-id="0c273-114">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="0c273-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="0c273-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="0c273-115">iPhoneAndIPod</span></span>|<span data-ttu-id="0c273-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="0c273-116">Boolean</span></span>|<span data-ttu-id="0c273-117">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="0c273-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c273-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0c273-118">Relationships</span></span>
<span data-ttu-id="0c273-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c273-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c273-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c273-120">JSON Representation</span></span>
<span data-ttu-id="0c273-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c273-121">Here is a JSON representation of the resource.</span></span>
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





