---
title: tipo de recurso de mobileAppTroubleshootingAppUpdateHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 606fe9dcf282dd75992f5a936aa5f49dfbb61dc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414204"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="7c749-103">tipo de recurso de mobileAppTroubleshootingAppUpdateHistory</span><span class="sxs-lookup"><span data-stu-id="7c749-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="7c749-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7c749-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c749-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7c749-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c749-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7c749-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c749-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="7c749-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="7c749-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7c749-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7c749-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c749-109">Properties</span></span>
|<span data-ttu-id="7c749-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c749-110">Property</span></span>|<span data-ttu-id="7c749-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c749-111">Type</span></span>|<span data-ttu-id="7c749-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c749-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c749-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="7c749-113">occurrenceDateTime</span></span>|<span data-ttu-id="7c749-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c749-114">DateTimeOffset</span></span>|<span data-ttu-id="7c749-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="7c749-115">Time when the history item occurred.</span></span> <span data-ttu-id="7c749-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7c749-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c749-117">Relações</span><span class="sxs-lookup"><span data-stu-id="7c749-117">Relationships</span></span>
<span data-ttu-id="7c749-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c749-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c749-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c749-119">JSON Representation</span></span>
<span data-ttu-id="7c749-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c749-120">Here is a JSON representation of the resource.</span></span>
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




