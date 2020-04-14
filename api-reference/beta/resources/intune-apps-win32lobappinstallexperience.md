---
title: tipo de recurso win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2470aeac3b92052e801db12d4da7f76113a9c8d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422970"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="a4832-103">tipo de recurso win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="a4832-103">win32LobAppInstallExperience resource type</span></span>

<span data-ttu-id="a4832-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4832-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4832-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4832-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4832-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4832-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4832-107">Contém propriedades de experiência de instalação para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="a4832-107">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="a4832-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4832-108">Properties</span></span>
|<span data-ttu-id="a4832-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4832-109">Property</span></span>|<span data-ttu-id="a4832-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4832-110">Type</span></span>|<span data-ttu-id="a4832-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4832-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4832-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="a4832-112">runAsAccount</span></span>|[<span data-ttu-id="a4832-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="a4832-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="a4832-114">Indica o tipo de contexto de execução em que o aplicativo é executado.</span><span class="sxs-lookup"><span data-stu-id="a4832-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="a4832-115">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="a4832-115">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="a4832-116">deviceRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="a4832-116">deviceRestartBehavior</span></span>|[<span data-ttu-id="a4832-117">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="a4832-117">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="a4832-118">Comportamento de reinicialização de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a4832-118">Device restart behavior.</span></span> <span data-ttu-id="a4832-119">Os valores possíveis são: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="a4832-119">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4832-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a4832-120">Relationships</span></span>
<span data-ttu-id="a4832-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4832-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4832-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4832-122">JSON Representation</span></span>
<span data-ttu-id="a4832-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4832-123">Here is a JSON representation of the resource.</span></span>
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



