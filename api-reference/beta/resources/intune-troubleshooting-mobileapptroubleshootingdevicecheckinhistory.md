---
title: tipo de recurso de mobileAppTroubleshootingDeviceCheckinHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6b9d900e712e3c3b126dd36671049e8935f09a83
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844944"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="187a3-103">tipo de recurso de mobileAppTroubleshootingDeviceCheckinHistory</span><span class="sxs-lookup"><span data-stu-id="187a3-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="187a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="187a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="187a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="187a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="187a3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="187a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="187a3-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="187a3-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="187a3-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="187a3-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="187a3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="187a3-109">Properties</span></span>
|<span data-ttu-id="187a3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="187a3-110">Property</span></span>|<span data-ttu-id="187a3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="187a3-111">Type</span></span>|<span data-ttu-id="187a3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="187a3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="187a3-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="187a3-113">occurrenceDateTime</span></span>|<span data-ttu-id="187a3-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="187a3-114">DateTimeOffset</span></span>|<span data-ttu-id="187a3-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="187a3-115">Time when the history item occurred.</span></span> <span data-ttu-id="187a3-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="187a3-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="187a3-117">Relações</span><span class="sxs-lookup"><span data-stu-id="187a3-117">Relationships</span></span>
<span data-ttu-id="187a3-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="187a3-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="187a3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="187a3-119">JSON Representation</span></span>
<span data-ttu-id="187a3-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="187a3-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```





