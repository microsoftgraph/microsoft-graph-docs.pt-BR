---
title: tipo de recurso de mobileAppTroubleshootingAppTargetHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0a1d37f86ebb43b7d697a9407ce0e3a479b2350
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402962"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="7dfe9-103">tipo de recurso de mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="7dfe9-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="7dfe9-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7dfe9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7dfe9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7dfe9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7dfe9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7dfe9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dfe9-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="7dfe9-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="7dfe9-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7dfe9-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7dfe9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7dfe9-109">Properties</span></span>
|<span data-ttu-id="7dfe9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7dfe9-110">Property</span></span>|<span data-ttu-id="7dfe9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dfe9-111">Type</span></span>|<span data-ttu-id="7dfe9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dfe9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dfe9-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="7dfe9-113">occurrenceDateTime</span></span>|<span data-ttu-id="7dfe9-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dfe9-114">DateTimeOffset</span></span>|<span data-ttu-id="7dfe9-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="7dfe9-115">Time when the history item occurred.</span></span> <span data-ttu-id="7dfe9-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="7dfe9-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="7dfe9-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="7dfe9-117">securityGroupId</span></span>|<span data-ttu-id="7dfe9-118">String</span><span class="sxs-lookup"><span data-stu-id="7dfe9-118">String</span></span>|<span data-ttu-id="7dfe9-119">Identificação de grupo de segurança AAD ao qual ele estava direcionado.</span><span class="sxs-lookup"><span data-stu-id="7dfe9-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="7dfe9-120">runState</span><span class="sxs-lookup"><span data-stu-id="7dfe9-120">runState</span></span>|[<span data-ttu-id="7dfe9-121">runState</span><span class="sxs-lookup"><span data-stu-id="7dfe9-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="7dfe9-122">Status do item.</span><span class="sxs-lookup"><span data-stu-id="7dfe9-122">Status of the item.</span></span> <span data-ttu-id="7dfe9-123">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="7dfe9-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="7dfe9-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="7dfe9-124">errorCode</span></span>|<span data-ttu-id="7dfe9-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7dfe9-125">String</span></span>|<span data-ttu-id="7dfe9-126">Código de erro da falha, vazia se nenhum falha.</span><span class="sxs-lookup"><span data-stu-id="7dfe9-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dfe9-127">Relações</span><span class="sxs-lookup"><span data-stu-id="7dfe9-127">Relationships</span></span>
<span data-ttu-id="7dfe9-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7dfe9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7dfe9-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7dfe9-129">JSON Representation</span></span>
<span data-ttu-id="7dfe9-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7dfe9-130">Here is a JSON representation of the resource.</span></span>
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




