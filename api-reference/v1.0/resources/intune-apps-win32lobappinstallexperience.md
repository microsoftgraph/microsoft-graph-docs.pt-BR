---
title: tipo de recurso win32LobAppInstallExperience
description: Contém propriedades de experiência de instalação para um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 468afea165645c2fc6a728e5a171b1ef37e9e338
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080048"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="c4838-103">tipo de recurso win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="c4838-103">win32LobAppInstallExperience resource type</span></span>

<span data-ttu-id="c4838-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4838-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4838-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4838-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4838-106">Contém propriedades de experiência de instalação para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="c4838-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="c4838-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4838-107">Properties</span></span>
|<span data-ttu-id="c4838-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4838-108">Property</span></span>|<span data-ttu-id="c4838-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4838-109">Type</span></span>|<span data-ttu-id="c4838-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4838-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4838-111">deviceRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="c4838-111">deviceRestartBehavior</span></span>|[<span data-ttu-id="c4838-112">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="c4838-112">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="c4838-113">Comportamento de reinicialização de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4838-113">Device restart behavior.</span></span> <span data-ttu-id="c4838-114">Os valores possíveis são: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="c4838-114">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4838-115">Relações</span><span class="sxs-lookup"><span data-stu-id="c4838-115">Relationships</span></span>
<span data-ttu-id="c4838-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c4838-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4838-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4838-117">JSON Representation</span></span>
<span data-ttu-id="c4838-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c4838-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "deviceRestartBehavior": "String"
}
```





