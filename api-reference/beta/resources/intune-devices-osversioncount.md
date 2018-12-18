---
title: tipo de recurso de osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
author: tfitzmac
ms.openlocfilehash: ccc031c6060604b36166b4869d02f08854dfdd2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331994"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="a41f0-103">tipo de recurso de osVersionCount</span><span class="sxs-lookup"><span data-stu-id="a41f0-103">osVersionCount resource type</span></span>

> <span data-ttu-id="a41f0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a41f0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a41f0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a41f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a41f0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a41f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a41f0-107">Contagem de dispositivos com malware para cada versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a41f0-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="a41f0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a41f0-108">Properties</span></span>
|<span data-ttu-id="a41f0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a41f0-109">Property</span></span>|<span data-ttu-id="a41f0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a41f0-110">Type</span></span>|<span data-ttu-id="a41f0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a41f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a41f0-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="a41f0-112">osVersion</span></span>|<span data-ttu-id="a41f0-113">String</span><span class="sxs-lookup"><span data-stu-id="a41f0-113">String</span></span>|<span data-ttu-id="a41f0-114">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a41f0-114">OS version</span></span>|
|<span data-ttu-id="a41f0-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a41f0-115">deviceCount</span></span>|<span data-ttu-id="a41f0-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a41f0-116">Int32</span></span>|<span data-ttu-id="a41f0-117">Contagem de dispositivos com malware para a versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a41f0-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="a41f0-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a41f0-118">lastUpdateDateTime</span></span>|<span data-ttu-id="a41f0-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a41f0-119">DateTimeOffset</span></span>|<span data-ttu-id="a41f0-120">O carimbo de hora da última atualização do dispositivo contar em UTC</span><span class="sxs-lookup"><span data-stu-id="a41f0-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="a41f0-121">Relações</span><span class="sxs-lookup"><span data-stu-id="a41f0-121">Relationships</span></span>
<span data-ttu-id="a41f0-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a41f0-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a41f0-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a41f0-123">JSON Representation</span></span>
<span data-ttu-id="a41f0-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a41f0-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```





