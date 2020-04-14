---
title: tipo de recurso win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3110ea120f88f56e49cfe33bf1b47631dc5c1f86
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422613"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="18763-103">tipo de recurso win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="18763-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="18763-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18763-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18763-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18763-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18763-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18763-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18763-107">Contém propriedades de código de retorno para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="18763-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="18763-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18763-108">Properties</span></span>
|<span data-ttu-id="18763-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18763-109">Property</span></span>|<span data-ttu-id="18763-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="18763-110">Type</span></span>|<span data-ttu-id="18763-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="18763-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18763-112">returnCode</span><span class="sxs-lookup"><span data-stu-id="18763-112">returnCode</span></span>|<span data-ttu-id="18763-113">Int32</span><span class="sxs-lookup"><span data-stu-id="18763-113">Int32</span></span>|<span data-ttu-id="18763-114">Código de retorno.</span><span class="sxs-lookup"><span data-stu-id="18763-114">Return code.</span></span>|
|<span data-ttu-id="18763-115">type</span><span class="sxs-lookup"><span data-stu-id="18763-115">type</span></span>|[<span data-ttu-id="18763-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="18763-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="18763-117">O tipo de código de retorno.</span><span class="sxs-lookup"><span data-stu-id="18763-117">The type of return code.</span></span> <span data-ttu-id="18763-118">Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="18763-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18763-119">Relações</span><span class="sxs-lookup"><span data-stu-id="18763-119">Relationships</span></span>
<span data-ttu-id="18763-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18763-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18763-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18763-121">JSON Representation</span></span>
<span data-ttu-id="18763-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18763-122">Here is a JSON representation of the resource.</span></span>
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



