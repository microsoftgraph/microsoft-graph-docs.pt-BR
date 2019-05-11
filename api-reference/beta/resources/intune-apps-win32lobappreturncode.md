---
title: tipo de recurso win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a37236064abb2e792e9227b8f76f32e1fd3ff9d9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949476"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="7e349-103">tipo de recurso win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="7e349-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="7e349-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7e349-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e349-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e349-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e349-106">Contém propriedades de código de retorno para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="7e349-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="7e349-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e349-107">Properties</span></span>
|<span data-ttu-id="7e349-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e349-108">Property</span></span>|<span data-ttu-id="7e349-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e349-109">Type</span></span>|<span data-ttu-id="7e349-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e349-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e349-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="7e349-111">returnCode</span></span>|<span data-ttu-id="7e349-112">Int32</span><span class="sxs-lookup"><span data-stu-id="7e349-112">Int32</span></span>|<span data-ttu-id="7e349-113">Código de retorno.</span><span class="sxs-lookup"><span data-stu-id="7e349-113">Return code.</span></span>|
|<span data-ttu-id="7e349-114">type</span><span class="sxs-lookup"><span data-stu-id="7e349-114">type</span></span>|[<span data-ttu-id="7e349-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="7e349-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="7e349-116">O tipo de código de retorno.</span><span class="sxs-lookup"><span data-stu-id="7e349-116">The type of return code.</span></span> <span data-ttu-id="7e349-117">Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="7e349-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e349-118">Relações</span><span class="sxs-lookup"><span data-stu-id="7e349-118">Relationships</span></span>
<span data-ttu-id="7e349-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e349-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e349-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e349-120">JSON Representation</span></span>
<span data-ttu-id="7e349-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e349-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```




