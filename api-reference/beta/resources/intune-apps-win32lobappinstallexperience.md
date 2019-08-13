---
title: tipo de recurso win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8cb0efbec4044bb63b9c8069e12bf934662ca587
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335666"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="565c6-103">tipo de recurso win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="565c6-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="565c6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="565c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="565c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="565c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="565c6-106">Contém propriedades de experiência de instalação para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="565c6-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="565c6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="565c6-107">Properties</span></span>
|<span data-ttu-id="565c6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="565c6-108">Property</span></span>|<span data-ttu-id="565c6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="565c6-109">Type</span></span>|<span data-ttu-id="565c6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="565c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="565c6-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="565c6-111">runAsAccount</span></span>|[<span data-ttu-id="565c6-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="565c6-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="565c6-113">Indica o tipo de contexto de execução em que o aplicativo é executado.</span><span class="sxs-lookup"><span data-stu-id="565c6-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="565c6-114">Os valores possíveis são: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="565c6-114">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="565c6-115">Relações</span><span class="sxs-lookup"><span data-stu-id="565c6-115">Relationships</span></span>
<span data-ttu-id="565c6-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="565c6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="565c6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="565c6-117">JSON Representation</span></span>
<span data-ttu-id="565c6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="565c6-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```



