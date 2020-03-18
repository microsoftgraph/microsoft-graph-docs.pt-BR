---
title: tipo de recurso win32LobAppRestartSettings
description: Contém propriedades que descrevem a coordenação de reinicialização após uma instalação de aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 66e5bbfe925dfc6ee023e06d58b70aa4ed680ee4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42766907"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="ca503-103">tipo de recurso win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="ca503-103">win32LobAppRestartSettings resource type</span></span>

> <span data-ttu-id="ca503-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca503-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca503-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca503-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca503-106">Contém propriedades que descrevem a coordenação de reinicialização após uma instalação de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca503-106">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="ca503-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca503-107">Properties</span></span>
|<span data-ttu-id="ca503-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca503-108">Property</span></span>|<span data-ttu-id="ca503-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca503-109">Type</span></span>|<span data-ttu-id="ca503-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca503-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca503-111">gracePeriodInMinutes</span><span class="sxs-lookup"><span data-stu-id="ca503-111">gracePeriodInMinutes</span></span>|<span data-ttu-id="ca503-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ca503-112">Int32</span></span>|<span data-ttu-id="ca503-113">O número de minutos de espera antes de reiniciar o dispositivo após uma instalação de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca503-113">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="ca503-114">countdownDisplayBeforeRestartInMinutes</span><span class="sxs-lookup"><span data-stu-id="ca503-114">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="ca503-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ca503-115">Int32</span></span>|<span data-ttu-id="ca503-116">O número de minutos antes do tempo de reinicialização para exibir a caixa de diálogo de contagem regressiva de reinicializações pendentes.</span><span class="sxs-lookup"><span data-stu-id="ca503-116">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="ca503-117">restartNotificationSnoozeDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="ca503-117">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="ca503-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ca503-118">Int32</span></span>|<span data-ttu-id="ca503-119">O número de minutos para adiar a caixa de diálogo de notificação de reinicialização quando o botão adiar estiver selecionado.</span><span class="sxs-lookup"><span data-stu-id="ca503-119">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca503-120">Relações</span><span class="sxs-lookup"><span data-stu-id="ca503-120">Relationships</span></span>
<span data-ttu-id="ca503-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca503-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca503-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca503-122">JSON Representation</span></span>
<span data-ttu-id="ca503-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca503-123">Here is a JSON representation of the resource.</span></span>
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



