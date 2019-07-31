---
title: tipo de recurso mobileAppTroubleshootingAppTargetHistory
description: Item de histórico contido no evento de solução de problemas de aplicativo móvel.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47a00ec29f91c81c513ef509e763c4071c106b1e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010207"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="225c0-103">tipo de recurso mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="225c0-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="225c0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="225c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="225c0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="225c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="225c0-106">Item de histórico contido no evento de solução de problemas de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="225c0-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="225c0-107">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="225c0-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="225c0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="225c0-108">Properties</span></span>
|<span data-ttu-id="225c0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="225c0-109">Property</span></span>|<span data-ttu-id="225c0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="225c0-110">Type</span></span>|<span data-ttu-id="225c0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="225c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="225c0-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="225c0-112">occurrenceDateTime</span></span>|<span data-ttu-id="225c0-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="225c0-113">DateTimeOffset</span></span>|<span data-ttu-id="225c0-114">Hora em que o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="225c0-114">Time when the history item occurred.</span></span> <span data-ttu-id="225c0-115">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="225c0-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="225c0-116">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="225c0-116">securityGroupId</span></span>|<span data-ttu-id="225c0-117">String</span><span class="sxs-lookup"><span data-stu-id="225c0-117">String</span></span>|<span data-ttu-id="225c0-118">ID do grupo de segurança do AAD para o qual foi direcionado.</span><span class="sxs-lookup"><span data-stu-id="225c0-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="225c0-119">runState</span><span class="sxs-lookup"><span data-stu-id="225c0-119">runState</span></span>|[<span data-ttu-id="225c0-120">runState</span><span class="sxs-lookup"><span data-stu-id="225c0-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="225c0-121">Status do item.</span><span class="sxs-lookup"><span data-stu-id="225c0-121">Status of the item.</span></span> <span data-ttu-id="225c0-122">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="225c0-122">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="225c0-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="225c0-123">errorCode</span></span>|<span data-ttu-id="225c0-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="225c0-124">String</span></span>|<span data-ttu-id="225c0-125">Código de erro para a falha, vazio se não houver falha.</span><span class="sxs-lookup"><span data-stu-id="225c0-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="225c0-126">Relações</span><span class="sxs-lookup"><span data-stu-id="225c0-126">Relationships</span></span>
<span data-ttu-id="225c0-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="225c0-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="225c0-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="225c0-128">JSON Representation</span></span>
<span data-ttu-id="225c0-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="225c0-129">Here is a JSON representation of the resource.</span></span>
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





