---
title: tipo de recurso de mobileAppTroubleshootingAppPolicyCreationHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd7880a6d931fafda46ab4adf0668835438ddcb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870102"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="2a5f4-103">tipo de recurso de mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="2a5f4-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="2a5f4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2a5f4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a5f4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2a5f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a5f4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2a5f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a5f4-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="2a5f4-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="2a5f4-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="2a5f4-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2a5f4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a5f4-109">Properties</span></span>
|<span data-ttu-id="2a5f4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a5f4-110">Property</span></span>|<span data-ttu-id="2a5f4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a5f4-111">Type</span></span>|<span data-ttu-id="2a5f4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a5f4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a5f4-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="2a5f4-113">occurrenceDateTime</span></span>|<span data-ttu-id="2a5f4-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a5f4-114">DateTimeOffset</span></span>|<span data-ttu-id="2a5f4-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="2a5f4-115">Time when the history item occurred.</span></span> <span data-ttu-id="2a5f4-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="2a5f4-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="2a5f4-117">runState</span><span class="sxs-lookup"><span data-stu-id="2a5f4-117">runState</span></span>|[<span data-ttu-id="2a5f4-118">runState</span><span class="sxs-lookup"><span data-stu-id="2a5f4-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="2a5f4-119">Status do item.</span><span class="sxs-lookup"><span data-stu-id="2a5f4-119">Status of the item.</span></span> <span data-ttu-id="2a5f4-120">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="2a5f4-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="2a5f4-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="2a5f4-121">errorCode</span></span>|<span data-ttu-id="2a5f4-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a5f4-122">String</span></span>|<span data-ttu-id="2a5f4-123">Código de erro da falha, vazia se nenhum falha.</span><span class="sxs-lookup"><span data-stu-id="2a5f4-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a5f4-124">Relações</span><span class="sxs-lookup"><span data-stu-id="2a5f4-124">Relationships</span></span>
<span data-ttu-id="2a5f4-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2a5f4-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a5f4-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a5f4-126">JSON Representation</span></span>
<span data-ttu-id="2a5f4-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2a5f4-127">Here is a JSON representation of the resource.</span></span>
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





