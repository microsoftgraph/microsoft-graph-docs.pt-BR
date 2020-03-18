---
title: tipo de recurso win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5e1c312fd7a43c6f685d80211849e9a9280917b8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797546"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="3c6a7-103">tipo de recurso win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="3c6a7-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="3c6a7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c6a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c6a7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c6a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c6a7-106">Contém propriedades de código de retorno para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="3c6a7-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="3c6a7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c6a7-107">Properties</span></span>
|<span data-ttu-id="3c6a7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c6a7-108">Property</span></span>|<span data-ttu-id="3c6a7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c6a7-109">Type</span></span>|<span data-ttu-id="3c6a7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c6a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c6a7-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="3c6a7-111">returnCode</span></span>|<span data-ttu-id="3c6a7-112">Int32</span><span class="sxs-lookup"><span data-stu-id="3c6a7-112">Int32</span></span>|<span data-ttu-id="3c6a7-113">Código de retorno.</span><span class="sxs-lookup"><span data-stu-id="3c6a7-113">Return code.</span></span>|
|<span data-ttu-id="3c6a7-114">type</span><span class="sxs-lookup"><span data-stu-id="3c6a7-114">type</span></span>|[<span data-ttu-id="3c6a7-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="3c6a7-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="3c6a7-116">O tipo de código de retorno.</span><span class="sxs-lookup"><span data-stu-id="3c6a7-116">The type of return code.</span></span> <span data-ttu-id="3c6a7-117">Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="3c6a7-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c6a7-118">Relações</span><span class="sxs-lookup"><span data-stu-id="3c6a7-118">Relationships</span></span>
<span data-ttu-id="3c6a7-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c6a7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c6a7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c6a7-120">JSON Representation</span></span>
<span data-ttu-id="3c6a7-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c6a7-121">Here is a JSON representation of the resource.</span></span>
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



