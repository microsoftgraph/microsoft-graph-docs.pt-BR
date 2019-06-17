---
title: tipo de recurso win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af7042dd9a95ffde1a447b9d047db003415ad4b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987296"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="ec8e5-103">tipo de recurso win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="ec8e5-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="ec8e5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ec8e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec8e5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec8e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec8e5-106">Contém propriedades de experiência de instalação para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="ec8e5-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="ec8e5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec8e5-107">Properties</span></span>
|<span data-ttu-id="ec8e5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec8e5-108">Property</span></span>|<span data-ttu-id="ec8e5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec8e5-109">Type</span></span>|<span data-ttu-id="ec8e5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec8e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec8e5-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="ec8e5-111">runAsAccount</span></span>|[<span data-ttu-id="ec8e5-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="ec8e5-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="ec8e5-113">Indica o tipo de contexto de execução em que o aplicativo é executado.</span><span class="sxs-lookup"><span data-stu-id="ec8e5-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="ec8e5-114">Os valores possíveis são: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="ec8e5-114">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec8e5-115">Relações</span><span class="sxs-lookup"><span data-stu-id="ec8e5-115">Relationships</span></span>
<span data-ttu-id="ec8e5-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec8e5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec8e5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec8e5-117">JSON Representation</span></span>
<span data-ttu-id="ec8e5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec8e5-118">Here is a JSON representation of the resource.</span></span>
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





