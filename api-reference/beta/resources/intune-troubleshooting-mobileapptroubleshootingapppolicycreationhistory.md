---
title: tipo de recurso de mobileAppTroubleshootingAppPolicyCreationHistory
description: Item de histórico contido no evento Mobile App solução de problemas.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e81f7f39cac934a89cf06d77fbcb80581267097b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394555"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="884f6-103">tipo de recurso de mobileAppTroubleshootingAppPolicyCreationHistory</span><span class="sxs-lookup"><span data-stu-id="884f6-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="884f6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="884f6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="884f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="884f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="884f6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="884f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="884f6-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="884f6-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="884f6-108">Herda de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="884f6-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="884f6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="884f6-109">Properties</span></span>
|<span data-ttu-id="884f6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="884f6-110">Property</span></span>|<span data-ttu-id="884f6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="884f6-111">Type</span></span>|<span data-ttu-id="884f6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="884f6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="884f6-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="884f6-113">occurrenceDateTime</span></span>|<span data-ttu-id="884f6-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="884f6-114">DateTimeOffset</span></span>|<span data-ttu-id="884f6-115">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="884f6-115">Time when the history item occurred.</span></span> <span data-ttu-id="884f6-116">Herdado de [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="884f6-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="884f6-117">runState</span><span class="sxs-lookup"><span data-stu-id="884f6-117">runState</span></span>|[<span data-ttu-id="884f6-118">runState</span><span class="sxs-lookup"><span data-stu-id="884f6-118">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="884f6-119">Status do item.</span><span class="sxs-lookup"><span data-stu-id="884f6-119">Status of the item.</span></span> <span data-ttu-id="884f6-120">Os valores possíveis são: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="884f6-120">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="884f6-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="884f6-121">errorCode</span></span>|<span data-ttu-id="884f6-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="884f6-122">String</span></span>|<span data-ttu-id="884f6-123">Código de erro da falha, vazia se nenhum falha.</span><span class="sxs-lookup"><span data-stu-id="884f6-123">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="884f6-124">Relações</span><span class="sxs-lookup"><span data-stu-id="884f6-124">Relationships</span></span>
<span data-ttu-id="884f6-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="884f6-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="884f6-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="884f6-126">JSON Representation</span></span>
<span data-ttu-id="884f6-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="884f6-127">Here is a JSON representation of the resource.</span></span>
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




