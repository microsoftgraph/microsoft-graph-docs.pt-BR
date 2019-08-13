---
title: tipo de recurso win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84b2798956ec2b88b4c4dea212fb614f26ff1eff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335484"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="cdcbe-103">tipo de recurso win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="cdcbe-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="cdcbe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cdcbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdcbe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cdcbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdcbe-106">Contém propriedades de código de retorno para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="cdcbe-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="cdcbe-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cdcbe-107">Properties</span></span>
|<span data-ttu-id="cdcbe-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdcbe-108">Property</span></span>|<span data-ttu-id="cdcbe-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdcbe-109">Type</span></span>|<span data-ttu-id="cdcbe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdcbe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdcbe-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="cdcbe-111">returnCode</span></span>|<span data-ttu-id="cdcbe-112">Int32</span><span class="sxs-lookup"><span data-stu-id="cdcbe-112">Int32</span></span>|<span data-ttu-id="cdcbe-113">Código de retorno.</span><span class="sxs-lookup"><span data-stu-id="cdcbe-113">Return code.</span></span>|
|<span data-ttu-id="cdcbe-114">type</span><span class="sxs-lookup"><span data-stu-id="cdcbe-114">type</span></span>|[<span data-ttu-id="cdcbe-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="cdcbe-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="cdcbe-116">O tipo de código de retorno.</span><span class="sxs-lookup"><span data-stu-id="cdcbe-116">The type of return code.</span></span> <span data-ttu-id="cdcbe-117">Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="cdcbe-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdcbe-118">Relações</span><span class="sxs-lookup"><span data-stu-id="cdcbe-118">Relationships</span></span>
<span data-ttu-id="cdcbe-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cdcbe-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdcbe-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cdcbe-120">JSON Representation</span></span>
<span data-ttu-id="cdcbe-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cdcbe-121">Here is a JSON representation of the resource.</span></span>
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



