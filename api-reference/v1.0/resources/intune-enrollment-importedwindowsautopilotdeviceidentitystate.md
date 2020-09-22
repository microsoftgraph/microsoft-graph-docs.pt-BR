---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a68b65d2cf640a8a44fff7481f7c782d9ab0375
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988244"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="880f7-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="880f7-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="880f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="880f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="880f7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="880f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="880f7-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="880f7-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="880f7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="880f7-107">Properties</span></span>
|<span data-ttu-id="880f7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="880f7-108">Property</span></span>|<span data-ttu-id="880f7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="880f7-109">Type</span></span>|<span data-ttu-id="880f7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="880f7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="880f7-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="880f7-111">deviceImportStatus</span></span>|[<span data-ttu-id="880f7-112">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="880f7-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="880f7-113">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="880f7-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="880f7-114">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="880f7-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="880f7-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="880f7-115">deviceRegistrationId</span></span>|<span data-ttu-id="880f7-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="880f7-116">String</span></span>|<span data-ttu-id="880f7-117">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="880f7-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="880f7-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="880f7-118">deviceErrorCode</span></span>|<span data-ttu-id="880f7-119">Int32</span><span class="sxs-lookup"><span data-stu-id="880f7-119">Int32</span></span>|<span data-ttu-id="880f7-120">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="880f7-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="880f7-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="880f7-121">deviceErrorName</span></span>|<span data-ttu-id="880f7-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="880f7-122">String</span></span>|<span data-ttu-id="880f7-123">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="880f7-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="880f7-124">Relações</span><span class="sxs-lookup"><span data-stu-id="880f7-124">Relationships</span></span>
<span data-ttu-id="880f7-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="880f7-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="880f7-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="880f7-126">JSON Representation</span></span>
<span data-ttu-id="880f7-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="880f7-127">Here is a JSON representation of the resource.</span></span>
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









