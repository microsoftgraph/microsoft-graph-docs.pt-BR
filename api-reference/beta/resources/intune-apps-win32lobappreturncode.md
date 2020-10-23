---
title: tipo de recurso win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8049ef7a7678d7d5283d45d2236dc364f2df4669
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706167"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="a7408-103">tipo de recurso win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="a7408-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="a7408-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7408-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7408-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a7408-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7408-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7408-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7408-107">Contém propriedades de código de retorno para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="a7408-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="a7408-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7408-108">Properties</span></span>
|<span data-ttu-id="a7408-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7408-109">Property</span></span>|<span data-ttu-id="a7408-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7408-110">Type</span></span>|<span data-ttu-id="a7408-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7408-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7408-112">returnCode</span><span class="sxs-lookup"><span data-stu-id="a7408-112">returnCode</span></span>|<span data-ttu-id="a7408-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a7408-113">Int32</span></span>|<span data-ttu-id="a7408-114">Código de retorno.</span><span class="sxs-lookup"><span data-stu-id="a7408-114">Return code.</span></span>|
|<span data-ttu-id="a7408-115">type</span><span class="sxs-lookup"><span data-stu-id="a7408-115">type</span></span>|[<span data-ttu-id="a7408-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="a7408-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="a7408-117">O tipo de código de retorno.</span><span class="sxs-lookup"><span data-stu-id="a7408-117">The type of return code.</span></span> <span data-ttu-id="a7408-118">Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="a7408-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7408-119">Relações</span><span class="sxs-lookup"><span data-stu-id="a7408-119">Relationships</span></span>
<span data-ttu-id="a7408-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7408-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7408-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7408-121">JSON Representation</span></span>
<span data-ttu-id="a7408-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7408-122">Here is a JSON representation of the resource.</span></span>
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





