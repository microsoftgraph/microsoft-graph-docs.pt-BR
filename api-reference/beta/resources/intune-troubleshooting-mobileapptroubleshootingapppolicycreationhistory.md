---
title: tipo de recurso mobileAppTroubleshootingAppPolicyCreationHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a93b88f850e2fa220903362375774d8a6dded59c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160498"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="28475-103">tipo de recurso mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="28475-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="28475-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28475-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28475-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28475-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28475-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="28475-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="28475-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="28475-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="28475-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28475-108">Properties</span></span>
|<span data-ttu-id="28475-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28475-109">Property</span></span>|<span data-ttu-id="28475-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="28475-110">Type</span></span>|<span data-ttu-id="28475-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="28475-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28475-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="28475-112">occurrenceDateTime</span></span>|<span data-ttu-id="28475-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28475-113">DateTimeOffset</span></span>|<span data-ttu-id="28475-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="28475-114">Time when the history item occurred.</span></span> <span data-ttu-id="28475-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="28475-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="28475-116">runState</span><span class="sxs-lookup"><span data-stu-id="28475-116">runState</span></span>|[<span data-ttu-id="28475-117">runState</span><span class="sxs-lookup"><span data-stu-id="28475-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="28475-118">Status do item.</span><span class="sxs-lookup"><span data-stu-id="28475-118">Status of the item.</span></span> <span data-ttu-id="28475-119">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="28475-119">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="28475-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="28475-120">errorCode</span></span>|<span data-ttu-id="28475-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28475-121">String</span></span>|<span data-ttu-id="28475-122">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="28475-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28475-123">Relações</span><span class="sxs-lookup"><span data-stu-id="28475-123">Relationships</span></span>
<span data-ttu-id="28475-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28475-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28475-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28475-125">JSON Representation</span></span>
<span data-ttu-id="28475-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28475-126">Here is a JSON representation of the resource.</span></span>
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




