---
title: tipo de recurso de mobileAppTroubleshootingAppUpdateHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c938aa30667f28e65285cfdb365f4b0eab55104a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922267"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="d6086-103">tipo de recurso de mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="d6086-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="d6086-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d6086-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6086-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d6086-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6086-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d6086-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6086-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="d6086-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="d6086-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d6086-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6086-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6086-109">Properties</span></span>
|<span data-ttu-id="d6086-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6086-110">Property</span></span>|<span data-ttu-id="d6086-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6086-111">Type</span></span>|<span data-ttu-id="d6086-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6086-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6086-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d6086-113">occurrenceDateTime</span></span>|<span data-ttu-id="d6086-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6086-114">DateTimeOffset</span></span>|<span data-ttu-id="d6086-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="d6086-115">Time when the history item occurred.</span></span> <span data-ttu-id="d6086-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d6086-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6086-117">Relações</span><span class="sxs-lookup"><span data-stu-id="d6086-117">Relationships</span></span>
<span data-ttu-id="d6086-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6086-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6086-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6086-119">JSON Representation</span></span>
<span data-ttu-id="d6086-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6086-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```





