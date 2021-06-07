---
title: Tipo de recurso win32LobAppReturnCode
description: Contém propriedades de código de retorno para um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 117ab8bd12cf8113efcbe42aa4f2ab7174e50ac3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759097"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="05c41-103">Tipo de recurso win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="05c41-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="05c41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05c41-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05c41-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05c41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05c41-106">Contém propriedades de código de retorno para um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="05c41-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="05c41-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05c41-107">Properties</span></span>
|<span data-ttu-id="05c41-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05c41-108">Property</span></span>|<span data-ttu-id="05c41-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="05c41-109">Type</span></span>|<span data-ttu-id="05c41-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c41-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05c41-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="05c41-111">returnCode</span></span>|<span data-ttu-id="05c41-112">Int32</span><span class="sxs-lookup"><span data-stu-id="05c41-112">Int32</span></span>|<span data-ttu-id="05c41-113">Código de retorno.</span><span class="sxs-lookup"><span data-stu-id="05c41-113">Return code.</span></span>|
|<span data-ttu-id="05c41-114">tipo</span><span class="sxs-lookup"><span data-stu-id="05c41-114">type</span></span>|[<span data-ttu-id="05c41-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="05c41-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="05c41-116">O tipo de código de retorno.</span><span class="sxs-lookup"><span data-stu-id="05c41-116">The type of return code.</span></span> <span data-ttu-id="05c41-117">Os valores possíveis são: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="05c41-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05c41-118">Relações</span><span class="sxs-lookup"><span data-stu-id="05c41-118">Relationships</span></span>
<span data-ttu-id="05c41-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05c41-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05c41-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05c41-120">JSON Representation</span></span>
<span data-ttu-id="05c41-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05c41-121">Here is a JSON representation of the resource.</span></span>
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




