---
title: Tipo de recurso expeditedWindowsQualityUpdateSettings
description: Um tipo complexo para armazenar as configurações de atualização de qualidade aceleradas, como data de lançamento e dias até a reinicialização forçada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 700b86d15737c75cbf10679ea6e944726d667431
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160071"
---
# <a name="expeditedwindowsqualityupdatesettings-resource-type"></a><span data-ttu-id="2caef-103">Tipo de recurso expeditedWindowsQualityUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="2caef-103">expeditedWindowsQualityUpdateSettings resource type</span></span>

<span data-ttu-id="2caef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2caef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2caef-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2caef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2caef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2caef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2caef-107">Um tipo complexo para armazenar as configurações de atualização de qualidade aceleradas, como data de lançamento e dias até a reinicialização forçada.</span><span class="sxs-lookup"><span data-stu-id="2caef-107">A complex type to store the expedited quality update settings such as release date and days until forced reboot.</span></span>

## <a name="properties"></a><span data-ttu-id="2caef-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2caef-108">Properties</span></span>
|<span data-ttu-id="2caef-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2caef-109">Property</span></span>|<span data-ttu-id="2caef-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2caef-110">Type</span></span>|<span data-ttu-id="2caef-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2caef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2caef-112">qualityUpdateRelease</span><span class="sxs-lookup"><span data-stu-id="2caef-112">qualityUpdateRelease</span></span>|<span data-ttu-id="2caef-113">String</span><span class="sxs-lookup"><span data-stu-id="2caef-113">String</span></span>|<span data-ttu-id="2caef-114">A data de lançamento para identificar uma atualização de qualidade.</span><span class="sxs-lookup"><span data-stu-id="2caef-114">The release date to identify a quality update.</span></span>|
|<span data-ttu-id="2caef-115">daysUntilForcedReboot</span><span class="sxs-lookup"><span data-stu-id="2caef-115">daysUntilForcedReboot</span></span>|<span data-ttu-id="2caef-116">Int32</span><span class="sxs-lookup"><span data-stu-id="2caef-116">Int32</span></span>|<span data-ttu-id="2caef-117">O número de dias após a instalação que a reinicialização forçada ocorrerá.</span><span class="sxs-lookup"><span data-stu-id="2caef-117">The number of days after installation that forced reboot will happen.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2caef-118">Relações</span><span class="sxs-lookup"><span data-stu-id="2caef-118">Relationships</span></span>
<span data-ttu-id="2caef-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2caef-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2caef-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2caef-120">JSON Representation</span></span>
<span data-ttu-id="2caef-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2caef-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expeditedWindowsQualityUpdateSettings",
  "qualityUpdateRelease": "String",
  "daysUntilForcedReboot": 1024
}
```




