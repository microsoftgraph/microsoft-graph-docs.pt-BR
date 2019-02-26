---
title: tipo de recurso mobileAppTroubleshootingAppTargetHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a7171cdde4889ba97a9cd29c4cc8c81ab1a9d58
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159350"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="42145-103">tipo de recurso mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="42145-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="42145-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42145-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42145-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42145-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42145-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="42145-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="42145-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="42145-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42145-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42145-108">Properties</span></span>
|<span data-ttu-id="42145-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42145-109">Property</span></span>|<span data-ttu-id="42145-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="42145-110">Type</span></span>|<span data-ttu-id="42145-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42145-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42145-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="42145-112">occurrenceDateTime</span></span>|<span data-ttu-id="42145-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42145-113">DateTimeOffset</span></span>|<span data-ttu-id="42145-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="42145-114">Time when the history item occurred.</span></span> <span data-ttu-id="42145-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="42145-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="42145-116">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="42145-116">securityGroupId</span></span>|<span data-ttu-id="42145-117">String</span><span class="sxs-lookup"><span data-stu-id="42145-117">String</span></span>|<span data-ttu-id="42145-118">ID do grupo de segurança do AAD para o qual foi direcionado.</span><span class="sxs-lookup"><span data-stu-id="42145-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="42145-119">runState</span><span class="sxs-lookup"><span data-stu-id="42145-119">runState</span></span>|[<span data-ttu-id="42145-120">runState</span><span class="sxs-lookup"><span data-stu-id="42145-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="42145-121">Status do item.</span><span class="sxs-lookup"><span data-stu-id="42145-121">Status of the item.</span></span> <span data-ttu-id="42145-122">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="42145-122">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="42145-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="42145-123">errorCode</span></span>|<span data-ttu-id="42145-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42145-124">String</span></span>|<span data-ttu-id="42145-125">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="42145-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42145-126">Relações</span><span class="sxs-lookup"><span data-stu-id="42145-126">Relationships</span></span>
<span data-ttu-id="42145-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42145-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42145-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42145-128">JSON Representation</span></span>
<span data-ttu-id="42145-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42145-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```




