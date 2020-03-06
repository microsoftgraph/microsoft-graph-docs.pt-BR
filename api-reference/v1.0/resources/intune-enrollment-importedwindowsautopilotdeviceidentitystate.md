---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fe8ae3addc2d4b74323471bc39fd8d5569d4df99
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530240"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="db5f8-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="db5f8-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="db5f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db5f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db5f8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db5f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db5f8-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="db5f8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="db5f8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db5f8-107">Properties</span></span>
|<span data-ttu-id="db5f8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db5f8-108">Property</span></span>|<span data-ttu-id="db5f8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="db5f8-109">Type</span></span>|<span data-ttu-id="db5f8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="db5f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db5f8-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="db5f8-111">deviceImportStatus</span></span>|[<span data-ttu-id="db5f8-112">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="db5f8-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="db5f8-113">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="db5f8-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="db5f8-114">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="db5f8-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="db5f8-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="db5f8-115">deviceRegistrationId</span></span>|<span data-ttu-id="db5f8-116">String</span><span class="sxs-lookup"><span data-stu-id="db5f8-116">String</span></span>|<span data-ttu-id="db5f8-117">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="db5f8-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="db5f8-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="db5f8-118">deviceErrorCode</span></span>|<span data-ttu-id="db5f8-119">Int32</span><span class="sxs-lookup"><span data-stu-id="db5f8-119">Int32</span></span>|<span data-ttu-id="db5f8-120">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="db5f8-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="db5f8-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="db5f8-121">deviceErrorName</span></span>|<span data-ttu-id="db5f8-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db5f8-122">String</span></span>|<span data-ttu-id="db5f8-123">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="db5f8-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="db5f8-124">Relações</span><span class="sxs-lookup"><span data-stu-id="db5f8-124">Relationships</span></span>
<span data-ttu-id="db5f8-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db5f8-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db5f8-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db5f8-126">JSON Representation</span></span>
<span data-ttu-id="db5f8-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db5f8-127">Here is a JSON representation of the resource.</span></span>
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




