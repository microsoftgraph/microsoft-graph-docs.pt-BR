---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e65de1501bb0480daf195ce910001624cabff98
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261702"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="c0abd-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="c0abd-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="c0abd-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0abd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0abd-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c0abd-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c0abd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0abd-106">Properties</span></span>
|<span data-ttu-id="c0abd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0abd-107">Property</span></span>|<span data-ttu-id="c0abd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0abd-108">Type</span></span>|<span data-ttu-id="c0abd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0abd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0abd-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="c0abd-110">deviceImportStatus</span></span>|[<span data-ttu-id="c0abd-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="c0abd-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="c0abd-112">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="c0abd-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="c0abd-113">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="c0abd-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="c0abd-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="c0abd-114">deviceRegistrationId</span></span>|<span data-ttu-id="c0abd-115">String</span><span class="sxs-lookup"><span data-stu-id="c0abd-115">String</span></span>|<span data-ttu-id="c0abd-116">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="c0abd-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="c0abd-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="c0abd-117">deviceErrorCode</span></span>|<span data-ttu-id="c0abd-118">Int32</span><span class="sxs-lookup"><span data-stu-id="c0abd-118">Int32</span></span>|<span data-ttu-id="c0abd-119">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="c0abd-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="c0abd-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="c0abd-120">deviceErrorName</span></span>|<span data-ttu-id="c0abd-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0abd-121">String</span></span>|<span data-ttu-id="c0abd-122">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="c0abd-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0abd-123">Relações</span><span class="sxs-lookup"><span data-stu-id="c0abd-123">Relationships</span></span>
<span data-ttu-id="c0abd-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0abd-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0abd-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0abd-125">JSON Representation</span></span>
<span data-ttu-id="c0abd-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0abd-126">Here is a JSON representation of the resource.</span></span>
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



