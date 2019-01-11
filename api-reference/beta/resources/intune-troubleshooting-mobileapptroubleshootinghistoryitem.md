---
title: tipo de recurso de mobileAppTroubleshootingHistoryItem
description: Item de histórico contido no evento Mobile App solução de problemas.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4db29e7badc8748e4aa64f318b68e0f21d0da5db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867925"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="c569b-103">tipo de recurso de mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="c569b-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="c569b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c569b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c569b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c569b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c569b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c569b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c569b-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="c569b-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>
## <a name="properties"></a><span data-ttu-id="c569b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c569b-108">Properties</span></span>
|<span data-ttu-id="c569b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c569b-109">Property</span></span>|<span data-ttu-id="c569b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c569b-110">Type</span></span>|<span data-ttu-id="c569b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c569b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c569b-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="c569b-112">occurrenceDateTime</span></span>|<span data-ttu-id="c569b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c569b-113">DateTimeOffset</span></span>|<span data-ttu-id="c569b-114">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="c569b-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c569b-115">Relações</span><span class="sxs-lookup"><span data-stu-id="c569b-115">Relationships</span></span>
<span data-ttu-id="c569b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c569b-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c569b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c569b-117">JSON Representation</span></span>
<span data-ttu-id="c569b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c569b-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)"
}
```





