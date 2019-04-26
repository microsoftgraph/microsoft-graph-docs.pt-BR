---
title: tipo de recurso mobileAppTroubleshootingAppTargetHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a19399788462b6dc7cae995971ddb443051b6959
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570705"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="c938a-103">tipo de recurso mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="c938a-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="c938a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c938a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c938a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c938a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c938a-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c938a-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="c938a-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c938a-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c938a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c938a-108">Properties</span></span>
|<span data-ttu-id="c938a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c938a-109">Property</span></span>|<span data-ttu-id="c938a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c938a-110">Type</span></span>|<span data-ttu-id="c938a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c938a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c938a-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="c938a-112">occurrenceDateTime</span></span>|<span data-ttu-id="c938a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c938a-113">DateTimeOffset</span></span>|<span data-ttu-id="c938a-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="c938a-114">Time when the history item occurred.</span></span> <span data-ttu-id="c938a-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c938a-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="c938a-116">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="c938a-116">securityGroupId</span></span>|<span data-ttu-id="c938a-117">String</span><span class="sxs-lookup"><span data-stu-id="c938a-117">String</span></span>|<span data-ttu-id="c938a-118">ID do grupo de segurança do AAD para o qual foi direcionado.</span><span class="sxs-lookup"><span data-stu-id="c938a-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="c938a-119">runState</span><span class="sxs-lookup"><span data-stu-id="c938a-119">runState</span></span>|[<span data-ttu-id="c938a-120">runState</span><span class="sxs-lookup"><span data-stu-id="c938a-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="c938a-121">Status do item.</span><span class="sxs-lookup"><span data-stu-id="c938a-121">Status of the item.</span></span> <span data-ttu-id="c938a-122">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="c938a-122">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="c938a-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="c938a-123">errorCode</span></span>|<span data-ttu-id="c938a-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c938a-124">String</span></span>|<span data-ttu-id="c938a-125">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="c938a-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c938a-126">Relações</span><span class="sxs-lookup"><span data-stu-id="c938a-126">Relationships</span></span>
<span data-ttu-id="c938a-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c938a-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c938a-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c938a-128">JSON Representation</span></span>
<span data-ttu-id="c938a-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c938a-129">Here is a JSON representation of the resource.</span></span>
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



