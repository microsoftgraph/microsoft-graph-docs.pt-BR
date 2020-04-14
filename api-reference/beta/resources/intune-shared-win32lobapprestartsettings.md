---
title: tipo de recurso win32LobAppRestartSettings
description: Contém propriedades que descrevem a coordenação de reinicialização após uma instalação de aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e962c9e03a587f0393ddec1fe273be15c6547b22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471994"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="1dd9c-103">tipo de recurso win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="1dd9c-103">win32LobAppRestartSettings resource type</span></span>

<span data-ttu-id="1dd9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dd9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dd9c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1dd9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dd9c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1dd9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dd9c-107">Contém propriedades que descrevem a coordenação de reinicialização após uma instalação de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1dd9c-107">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="1dd9c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1dd9c-108">Properties</span></span>
|<span data-ttu-id="1dd9c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dd9c-109">Property</span></span>|<span data-ttu-id="1dd9c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dd9c-110">Type</span></span>|<span data-ttu-id="1dd9c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dd9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dd9c-112">gracePeriodInMinutes</span><span class="sxs-lookup"><span data-stu-id="1dd9c-112">gracePeriodInMinutes</span></span>|<span data-ttu-id="1dd9c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1dd9c-113">Int32</span></span>|<span data-ttu-id="1dd9c-114">O número de minutos de espera antes de reiniciar o dispositivo após uma instalação de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1dd9c-114">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="1dd9c-115">countdownDisplayBeforeRestartInMinutes</span><span class="sxs-lookup"><span data-stu-id="1dd9c-115">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="1dd9c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1dd9c-116">Int32</span></span>|<span data-ttu-id="1dd9c-117">O número de minutos antes do tempo de reinicialização para exibir a caixa de diálogo de contagem regressiva de reinicializações pendentes.</span><span class="sxs-lookup"><span data-stu-id="1dd9c-117">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="1dd9c-118">restartNotificationSnoozeDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="1dd9c-118">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="1dd9c-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1dd9c-119">Int32</span></span>|<span data-ttu-id="1dd9c-120">O número de minutos para adiar a caixa de diálogo de notificação de reinicialização quando o botão adiar estiver selecionado.</span><span class="sxs-lookup"><span data-stu-id="1dd9c-120">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dd9c-121">Relações</span><span class="sxs-lookup"><span data-stu-id="1dd9c-121">Relationships</span></span>
<span data-ttu-id="1dd9c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1dd9c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dd9c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1dd9c-123">JSON Representation</span></span>
<span data-ttu-id="1dd9c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1dd9c-124">Here is a JSON representation of the resource.</span></span>
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



