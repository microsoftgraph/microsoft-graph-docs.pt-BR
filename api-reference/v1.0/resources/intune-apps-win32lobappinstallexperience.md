---
title: Tipo de recurso win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5a1f844683368d898be7a3acdc1dacbcaffa99ff
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760297"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="23f62-103">Tipo de recurso win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="23f62-103">win32LobAppInstallExperience resource type</span></span>

<span data-ttu-id="23f62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23f62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23f62-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23f62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23f62-106">Contém propriedades de experiência de instalação para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="23f62-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="23f62-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23f62-107">Properties</span></span>
|<span data-ttu-id="23f62-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23f62-108">Property</span></span>|<span data-ttu-id="23f62-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="23f62-109">Type</span></span>|<span data-ttu-id="23f62-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="23f62-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23f62-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="23f62-111">runAsAccount</span></span>|[<span data-ttu-id="23f62-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="23f62-112">runAsAccountType</span></span>](../resources/intune-apps-runasaccounttype.md)|<span data-ttu-id="23f62-113">Indica o tipo de contexto de execução em que o aplicativo é executado.</span><span class="sxs-lookup"><span data-stu-id="23f62-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="23f62-114">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="23f62-114">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="23f62-115">deviceRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="23f62-115">deviceRestartBehavior</span></span>|[<span data-ttu-id="23f62-116">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="23f62-116">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="23f62-117">Comportamento de reinicialização do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23f62-117">Device restart behavior.</span></span> <span data-ttu-id="23f62-118">Os valores possíveis são: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="23f62-118">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23f62-119">Relações</span><span class="sxs-lookup"><span data-stu-id="23f62-119">Relationships</span></span>
<span data-ttu-id="23f62-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23f62-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23f62-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23f62-121">JSON Representation</span></span>
<span data-ttu-id="23f62-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23f62-122">Here is a JSON representation of the resource.</span></span>
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




