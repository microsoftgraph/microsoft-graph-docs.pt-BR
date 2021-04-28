---
title: Tipo de recurso userExperienceSettings
description: Configurações controlar a experiência de atualização do usuário em um dispositivo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a5d920d1618cb6d212baf0487a39960638859cef
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067227"
---
# <a name="userexperiencesettings-resource-type"></a><span data-ttu-id="b4fc8-103">Tipo de recurso userExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="b4fc8-103">userExperienceSettings resource type</span></span>

<span data-ttu-id="b4fc8-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="b4fc8-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4fc8-105">Configurações controlar a experiência de atualização do usuário em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4fc8-105">Settings controlling the user's update experience on a device.</span></span>

## <a name="properties"></a><span data-ttu-id="b4fc8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4fc8-106">Properties</span></span>
|<span data-ttu-id="b4fc8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4fc8-107">Property</span></span>|<span data-ttu-id="b4fc8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4fc8-108">Type</span></span>|<span data-ttu-id="b4fc8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4fc8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4fc8-110">daysUntilForcedReboot</span><span class="sxs-lookup"><span data-stu-id="b4fc8-110">daysUntilForcedReboot</span></span>|<span data-ttu-id="b4fc8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="b4fc8-111">Int32</span></span>|<span data-ttu-id="b4fc8-112">Especifica o número de dias após a instalação de uma atualização, durante o qual o usuário do dispositivo pode controlar quando o dispositivo é reiniciado.</span><span class="sxs-lookup"><span data-stu-id="b4fc8-112">Specifies the number of days after an update is installed, during which the user of the device can control when the device restarts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4fc8-113">Relações</span><span class="sxs-lookup"><span data-stu-id="b4fc8-113">Relationships</span></span>
<span data-ttu-id="b4fc8-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4fc8-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4fc8-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4fc8-115">JSON representation</span></span>
<span data-ttu-id="b4fc8-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4fc8-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.userExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.userExperienceSettings",
  "daysUntilForcedReboot": "Integer"
}
```

