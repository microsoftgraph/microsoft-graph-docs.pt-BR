---
title: tipo de recurso de mobileAppTroubleshootingHistoryItem
description: Item de histórico contido no evento Mobile App solução de problemas.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 28245267a7c05f03bedd21c8dc0de17198de213c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400064"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="87ec6-103">tipo de recurso de mobileAppTroubleshootingHistoryItem</span><span class="sxs-lookup"><span data-stu-id="87ec6-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="87ec6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="87ec6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="87ec6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87ec6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87ec6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="87ec6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87ec6-107">Item de histórico contido no evento Mobile App solução de problemas.</span><span class="sxs-lookup"><span data-stu-id="87ec6-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="87ec6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87ec6-108">Properties</span></span>
|<span data-ttu-id="87ec6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87ec6-109">Property</span></span>|<span data-ttu-id="87ec6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="87ec6-110">Type</span></span>|<span data-ttu-id="87ec6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="87ec6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87ec6-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="87ec6-112">occurrenceDateTime</span></span>|<span data-ttu-id="87ec6-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ec6-113">DateTimeOffset</span></span>|<span data-ttu-id="87ec6-114">Hora de quando o item de histórico ocorreu.</span><span class="sxs-lookup"><span data-stu-id="87ec6-114">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87ec6-115">Relações</span><span class="sxs-lookup"><span data-stu-id="87ec6-115">Relationships</span></span>
<span data-ttu-id="87ec6-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87ec6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87ec6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87ec6-117">JSON Representation</span></span>
<span data-ttu-id="87ec6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87ec6-118">Here is a JSON representation of the resource.</span></span>
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




