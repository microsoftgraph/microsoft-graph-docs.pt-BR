---
title: tipo de recurso win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e7429433f4e1a382d0a5f4ba0dab6028bf27d283
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070972"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="69051-103">tipo de recurso win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="69051-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="69051-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69051-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69051-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69051-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69051-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69051-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69051-107">Contém propriedades de código de retorno para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="69051-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="69051-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69051-108">Properties</span></span>
|<span data-ttu-id="69051-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69051-109">Property</span></span>|<span data-ttu-id="69051-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="69051-110">Type</span></span>|<span data-ttu-id="69051-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69051-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69051-112">returnCode</span><span class="sxs-lookup"><span data-stu-id="69051-112">returnCode</span></span>|<span data-ttu-id="69051-113">Int32</span><span class="sxs-lookup"><span data-stu-id="69051-113">Int32</span></span>|<span data-ttu-id="69051-114">Código de retorno.</span><span class="sxs-lookup"><span data-stu-id="69051-114">Return code.</span></span>|
|<span data-ttu-id="69051-115">tipo</span><span class="sxs-lookup"><span data-stu-id="69051-115">type</span></span>|[<span data-ttu-id="69051-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="69051-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="69051-117">O tipo de código de retorno.</span><span class="sxs-lookup"><span data-stu-id="69051-117">The type of return code.</span></span> <span data-ttu-id="69051-118">Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="69051-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69051-119">Relações</span><span class="sxs-lookup"><span data-stu-id="69051-119">Relationships</span></span>
<span data-ttu-id="69051-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69051-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69051-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69051-121">JSON Representation</span></span>
<span data-ttu-id="69051-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69051-122">Here is a JSON representation of the resource.</span></span>
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






