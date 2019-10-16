---
title: tipo de recurso win32LobAppRestartSettings
description: Contém propriedades que descrevem a coordenação de reinicialização após uma instalação de aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84e4b231c189f02cf1e19401933ae517d8955263
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538760"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="96824-103">tipo de recurso win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="96824-103">win32LobAppRestartSettings resource type</span></span>

> <span data-ttu-id="96824-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96824-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96824-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96824-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96824-106">Contém propriedades que descrevem a coordenação de reinicialização após uma instalação de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96824-106">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="96824-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96824-107">Properties</span></span>
|<span data-ttu-id="96824-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96824-108">Property</span></span>|<span data-ttu-id="96824-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="96824-109">Type</span></span>|<span data-ttu-id="96824-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="96824-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96824-111">gracePeriodInMinutes</span><span class="sxs-lookup"><span data-stu-id="96824-111">gracePeriodInMinutes</span></span>|<span data-ttu-id="96824-112">Int32</span><span class="sxs-lookup"><span data-stu-id="96824-112">Int32</span></span>|<span data-ttu-id="96824-113">O número de minutos de espera antes de reiniciar o dispositivo após uma instalação de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96824-113">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="96824-114">countdownDisplayBeforeRestartInMinutes</span><span class="sxs-lookup"><span data-stu-id="96824-114">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="96824-115">Int32</span><span class="sxs-lookup"><span data-stu-id="96824-115">Int32</span></span>|<span data-ttu-id="96824-116">O número de minutos antes do tempo de reinicialização para exibir a caixa de diálogo de contagem regressiva de reinicializações pendentes.</span><span class="sxs-lookup"><span data-stu-id="96824-116">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="96824-117">restartNotificationSnoozeDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="96824-117">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="96824-118">Int32</span><span class="sxs-lookup"><span data-stu-id="96824-118">Int32</span></span>|<span data-ttu-id="96824-119">O número de minutos para adiar a caixa de diálogo de notificação de reinicialização quando o botão adiar estiver selecionado.</span><span class="sxs-lookup"><span data-stu-id="96824-119">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96824-120">Relações</span><span class="sxs-lookup"><span data-stu-id="96824-120">Relationships</span></span>
<span data-ttu-id="96824-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96824-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96824-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96824-122">JSON Representation</span></span>
<span data-ttu-id="96824-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96824-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRestartSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRestartSettings",
  "gracePeriodInMinutes": 1024,
  "countdownDisplayBeforeRestartInMinutes": 1024,
  "restartNotificationSnoozeDurationInMinutes": 1024
}
```



