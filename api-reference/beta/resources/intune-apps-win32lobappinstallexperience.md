---
title: tipo de recurso win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1a8f6fcecd995857b337f6d91b09e2ce7361defb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797623"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="bfaf7-103">tipo de recurso win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="bfaf7-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="bfaf7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bfaf7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfaf7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bfaf7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfaf7-106">Contém propriedades de experiência de instalação para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="bfaf7-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="bfaf7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfaf7-107">Properties</span></span>
|<span data-ttu-id="bfaf7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfaf7-108">Property</span></span>|<span data-ttu-id="bfaf7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfaf7-109">Type</span></span>|<span data-ttu-id="bfaf7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfaf7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfaf7-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="bfaf7-111">runAsAccount</span></span>|[<span data-ttu-id="bfaf7-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="bfaf7-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="bfaf7-113">Indica o tipo de contexto de execução em que o aplicativo é executado.</span><span class="sxs-lookup"><span data-stu-id="bfaf7-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="bfaf7-114">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="bfaf7-114">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="bfaf7-115">deviceRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="bfaf7-115">deviceRestartBehavior</span></span>|[<span data-ttu-id="bfaf7-116">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="bfaf7-116">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="bfaf7-117">Comportamento de reinicialização de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bfaf7-117">Device restart behavior.</span></span> <span data-ttu-id="bfaf7-118">Os valores possíveis são: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="bfaf7-118">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfaf7-119">Relações</span><span class="sxs-lookup"><span data-stu-id="bfaf7-119">Relationships</span></span>
<span data-ttu-id="bfaf7-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bfaf7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfaf7-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfaf7-121">JSON Representation</span></span>
<span data-ttu-id="bfaf7-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bfaf7-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String",
  "deviceRestartBehavior": "String"
}
```



