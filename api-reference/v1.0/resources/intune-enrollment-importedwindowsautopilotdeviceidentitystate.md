---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e65de1501bb0480daf195ce910001624cabff98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523361"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="ed4a7-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="ed4a7-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="ed4a7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed4a7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed4a7-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed4a7-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ed4a7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed4a7-106">Properties</span></span>
|<span data-ttu-id="ed4a7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed4a7-107">Property</span></span>|<span data-ttu-id="ed4a7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed4a7-108">Type</span></span>|<span data-ttu-id="ed4a7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed4a7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed4a7-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="ed4a7-110">deviceImportStatus</span></span>|[<span data-ttu-id="ed4a7-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="ed4a7-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="ed4a7-112">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="ed4a7-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="ed4a7-113">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="ed4a7-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="ed4a7-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="ed4a7-114">deviceRegistrationId</span></span>|<span data-ttu-id="ed4a7-115">String</span><span class="sxs-lookup"><span data-stu-id="ed4a7-115">String</span></span>|<span data-ttu-id="ed4a7-116">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="ed4a7-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="ed4a7-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="ed4a7-117">deviceErrorCode</span></span>|<span data-ttu-id="ed4a7-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ed4a7-118">Int32</span></span>|<span data-ttu-id="ed4a7-119">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="ed4a7-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="ed4a7-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="ed4a7-120">deviceErrorName</span></span>|<span data-ttu-id="ed4a7-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed4a7-121">String</span></span>|<span data-ttu-id="ed4a7-122">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="ed4a7-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed4a7-123">Relações</span><span class="sxs-lookup"><span data-stu-id="ed4a7-123">Relationships</span></span>
<span data-ttu-id="ed4a7-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed4a7-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed4a7-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed4a7-125">JSON Representation</span></span>
<span data-ttu-id="ed4a7-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed4a7-126">Here is a JSON representation of the resource.</span></span>
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



