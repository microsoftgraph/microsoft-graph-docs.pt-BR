---
title: tipo de recurso mobileAppTroubleshootingAppPolicyCreationHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4cbbdd3159982ac82031e654890d90741fd48d15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010193"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="bd1b2-103">tipo de recurso mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="bd1b2-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="bd1b2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bd1b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd1b2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd1b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd1b2-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="bd1b2-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="bd1b2-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="bd1b2-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd1b2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd1b2-108">Properties</span></span>
|<span data-ttu-id="bd1b2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd1b2-109">Property</span></span>|<span data-ttu-id="bd1b2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd1b2-110">Type</span></span>|<span data-ttu-id="bd1b2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd1b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd1b2-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="bd1b2-112">occurrenceDateTime</span></span>|<span data-ttu-id="bd1b2-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd1b2-113">DateTimeOffset</span></span>|<span data-ttu-id="bd1b2-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="bd1b2-114">Time when the history item occurred.</span></span> <span data-ttu-id="bd1b2-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="bd1b2-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="bd1b2-116">runState</span><span class="sxs-lookup"><span data-stu-id="bd1b2-116">runState</span></span>|[<span data-ttu-id="bd1b2-117">runState</span><span class="sxs-lookup"><span data-stu-id="bd1b2-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="bd1b2-118">Status do item.</span><span class="sxs-lookup"><span data-stu-id="bd1b2-118">Status of the item.</span></span> <span data-ttu-id="bd1b2-119">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="bd1b2-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="bd1b2-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="bd1b2-120">errorCode</span></span>|<span data-ttu-id="bd1b2-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bd1b2-121">String</span></span>|<span data-ttu-id="bd1b2-122">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="bd1b2-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd1b2-123">Relações</span><span class="sxs-lookup"><span data-stu-id="bd1b2-123">Relationships</span></span>
<span data-ttu-id="bd1b2-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd1b2-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd1b2-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd1b2-125">JSON Representation</span></span>
<span data-ttu-id="bd1b2-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd1b2-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
  "occurrenceDateTime": "String (timestamp)",
  "runState": "String",
  "errorCode": "String"
}
```





