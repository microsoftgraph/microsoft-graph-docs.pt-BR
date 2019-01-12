---
title: tipo de recurso de mobileAppTroubleshootingAppPolicyCreationHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0ee2088856c9c47771b3e647615f82fe26dfd552
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924388"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="d1e7e-103">tipo de recurso de mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="d1e7e-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="d1e7e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d1e7e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1e7e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d1e7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1e7e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d1e7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1e7e-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="d1e7e-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="d1e7e-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d1e7e-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1e7e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1e7e-109">Properties</span></span>
|<span data-ttu-id="d1e7e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1e7e-110">Property</span></span>|<span data-ttu-id="d1e7e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1e7e-111">Type</span></span>|<span data-ttu-id="d1e7e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1e7e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1e7e-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d1e7e-113">occurrenceDateTime</span></span>|<span data-ttu-id="d1e7e-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1e7e-114">DateTimeOffset</span></span>|<span data-ttu-id="d1e7e-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="d1e7e-115">Time when the history item occurred.</span></span> <span data-ttu-id="d1e7e-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d1e7e-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="d1e7e-117">runState</span><span class="sxs-lookup"><span data-stu-id="d1e7e-117">runState</span></span>|[<span data-ttu-id="d1e7e-118">runState</span><span class="sxs-lookup"><span data-stu-id="d1e7e-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="d1e7e-119">Status do item.</span><span class="sxs-lookup"><span data-stu-id="d1e7e-119">Status of the item.</span></span> <span data-ttu-id="d1e7e-120">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="d1e7e-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="d1e7e-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="d1e7e-121">errorCode</span></span>|<span data-ttu-id="d1e7e-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1e7e-122">String</span></span>|<span data-ttu-id="d1e7e-123">Código de erro da falha, vazia se nenhum falha.</span><span class="sxs-lookup"><span data-stu-id="d1e7e-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1e7e-124">Relações</span><span class="sxs-lookup"><span data-stu-id="d1e7e-124">Relationships</span></span>
<span data-ttu-id="d1e7e-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1e7e-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d1e7e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1e7e-126">JSON Representation</span></span>
<span data-ttu-id="d1e7e-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1e7e-127">Here is a JSON representation of the resource.</span></span>
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





