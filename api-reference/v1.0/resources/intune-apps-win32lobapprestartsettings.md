---
title: Tipo de recurso win32LobAppRestartSettings
description: Contém propriedades que descrevem a coordenação de reinicialização após uma instalação do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1db011486f1ec26afcc7e045afd2e1be1b553ec7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757827"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="c85d3-103">Tipo de recurso win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="c85d3-103">win32LobAppRestartSettings resource type</span></span>

<span data-ttu-id="c85d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c85d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c85d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c85d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c85d3-106">Contém propriedades que descrevem a coordenação de reinicialização após uma instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c85d3-106">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="c85d3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c85d3-107">Properties</span></span>
|<span data-ttu-id="c85d3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c85d3-108">Property</span></span>|<span data-ttu-id="c85d3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c85d3-109">Type</span></span>|<span data-ttu-id="c85d3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c85d3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c85d3-111">gracePeriodInMinutes</span><span class="sxs-lookup"><span data-stu-id="c85d3-111">gracePeriodInMinutes</span></span>|<span data-ttu-id="c85d3-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c85d3-112">Int32</span></span>|<span data-ttu-id="c85d3-113">O número de minutos para aguardar antes de reiniciar o dispositivo após a instalação de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c85d3-113">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="c85d3-114">countdownDisplayBeforeRestartInMinutes</span><span class="sxs-lookup"><span data-stu-id="c85d3-114">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="c85d3-115">Int32</span><span class="sxs-lookup"><span data-stu-id="c85d3-115">Int32</span></span>|<span data-ttu-id="c85d3-116">O número de minutos antes da hora de reinicialização para exibir a caixa de diálogo de contagem regressiva para reinicializações pendentes.</span><span class="sxs-lookup"><span data-stu-id="c85d3-116">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="c85d3-117">restartNotificationSnoozeDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="c85d3-117">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="c85d3-118">Int32</span><span class="sxs-lookup"><span data-stu-id="c85d3-118">Int32</span></span>|<span data-ttu-id="c85d3-119">O número de minutos para esnocar a caixa de diálogo de notificação de reinicialização quando o botão de esnooze estiver selecionado.</span><span class="sxs-lookup"><span data-stu-id="c85d3-119">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c85d3-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c85d3-120">Relationships</span></span>
<span data-ttu-id="c85d3-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c85d3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c85d3-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c85d3-122">JSON Representation</span></span>
<span data-ttu-id="c85d3-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c85d3-123">Here is a JSON representation of the resource.</span></span>
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




