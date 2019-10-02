---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 841855ca7fb9de734fd685efa0d2382087256beb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356832"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="cb2c4-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="cb2c4-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="cb2c4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb2c4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb2c4-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cb2c4-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="cb2c4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb2c4-106">Properties</span></span>
|<span data-ttu-id="cb2c4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb2c4-107">Property</span></span>|<span data-ttu-id="cb2c4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb2c4-108">Type</span></span>|<span data-ttu-id="cb2c4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb2c4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb2c4-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="cb2c4-110">deviceImportStatus</span></span>|[<span data-ttu-id="cb2c4-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="cb2c4-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="cb2c4-112">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="cb2c4-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="cb2c4-113">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="cb2c4-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="cb2c4-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="cb2c4-114">deviceRegistrationId</span></span>|<span data-ttu-id="cb2c4-115">String</span><span class="sxs-lookup"><span data-stu-id="cb2c4-115">String</span></span>|<span data-ttu-id="cb2c4-116">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="cb2c4-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="cb2c4-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="cb2c4-117">deviceErrorCode</span></span>|<span data-ttu-id="cb2c4-118">Int32</span><span class="sxs-lookup"><span data-stu-id="cb2c4-118">Int32</span></span>|<span data-ttu-id="cb2c4-119">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="cb2c4-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="cb2c4-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="cb2c4-120">deviceErrorName</span></span>|<span data-ttu-id="cb2c4-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb2c4-121">String</span></span>|<span data-ttu-id="cb2c4-122">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="cb2c4-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb2c4-123">Relações</span><span class="sxs-lookup"><span data-stu-id="cb2c4-123">Relationships</span></span>
<span data-ttu-id="cb2c4-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb2c4-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb2c4-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb2c4-125">JSON Representation</span></span>
<span data-ttu-id="cb2c4-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb2c4-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```




