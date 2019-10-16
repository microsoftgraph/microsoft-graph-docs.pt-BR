---
title: tipo de recurso win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aaf3c6dd99b36e33a8af3a8eb4687e1942779937
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538550"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="97c7c-103">tipo de recurso win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="97c7c-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="97c7c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97c7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97c7c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97c7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97c7c-106">Contém propriedades de experiência de instalação para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="97c7c-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="97c7c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97c7c-107">Properties</span></span>
|<span data-ttu-id="97c7c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97c7c-108">Property</span></span>|<span data-ttu-id="97c7c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="97c7c-109">Type</span></span>|<span data-ttu-id="97c7c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="97c7c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97c7c-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="97c7c-111">runAsAccount</span></span>|[<span data-ttu-id="97c7c-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="97c7c-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="97c7c-113">Indica o tipo de contexto de execução em que o aplicativo é executado.</span><span class="sxs-lookup"><span data-stu-id="97c7c-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="97c7c-114">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="97c7c-114">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="97c7c-115">deviceRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="97c7c-115">deviceRestartBehavior</span></span>|[<span data-ttu-id="97c7c-116">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="97c7c-116">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="97c7c-117">Comportamento de reinicialização de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97c7c-117">Device restart behavior.</span></span> <span data-ttu-id="97c7c-118">Os valores possíveis são: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="97c7c-118">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97c7c-119">Relações</span><span class="sxs-lookup"><span data-stu-id="97c7c-119">Relationships</span></span>
<span data-ttu-id="97c7c-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97c7c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97c7c-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97c7c-121">JSON Representation</span></span>
<span data-ttu-id="97c7c-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97c7c-122">Here is a JSON representation of the resource.</span></span>
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



