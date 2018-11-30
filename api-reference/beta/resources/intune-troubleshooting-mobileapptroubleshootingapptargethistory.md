---
title: tipo de recurso de mobileAppTroubleshootingAppTargetHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
ms.openlocfilehash: c7397e182c1af4c01753623a655579f5f8c6ee08
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036388"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="251de-103">tipo de recurso de mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="251de-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="251de-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="251de-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="251de-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="251de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="251de-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="251de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="251de-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="251de-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="251de-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="251de-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="251de-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="251de-109">Properties</span></span>
|<span data-ttu-id="251de-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="251de-110">Property</span></span>|<span data-ttu-id="251de-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="251de-111">Type</span></span>|<span data-ttu-id="251de-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="251de-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="251de-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="251de-113">occurrenceDateTime</span></span>|<span data-ttu-id="251de-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="251de-114">DateTimeOffset</span></span>|<span data-ttu-id="251de-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="251de-115">Time when the history item occurred.</span></span> <span data-ttu-id="251de-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="251de-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="251de-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="251de-117">securityGroupId</span></span>|<span data-ttu-id="251de-118">String</span><span class="sxs-lookup"><span data-stu-id="251de-118">String</span></span>|<span data-ttu-id="251de-119">Identificação de grupo de segurança AAD ao qual ele estava direcionado.</span><span class="sxs-lookup"><span data-stu-id="251de-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="251de-120">runState</span><span class="sxs-lookup"><span data-stu-id="251de-120">runState</span></span>|[<span data-ttu-id="251de-121">runState</span><span class="sxs-lookup"><span data-stu-id="251de-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="251de-122">Status do item.</span><span class="sxs-lookup"><span data-stu-id="251de-122">Status of the item.</span></span> <span data-ttu-id="251de-123">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="251de-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="251de-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="251de-124">errorCode</span></span>|<span data-ttu-id="251de-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="251de-125">String</span></span>|<span data-ttu-id="251de-126">Código de erro da falha, vazia se nenhum falha.</span><span class="sxs-lookup"><span data-stu-id="251de-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="251de-127">Relações</span><span class="sxs-lookup"><span data-stu-id="251de-127">Relationships</span></span>
<span data-ttu-id="251de-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="251de-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="251de-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="251de-129">JSON Representation</span></span>
<span data-ttu-id="251de-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="251de-130">Here is a JSON representation of the resource.</span></span>
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





