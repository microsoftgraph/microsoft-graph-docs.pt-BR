---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0dbf080592462a104ba6380c6db8116498b9143e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999082"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="7b3d2-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="7b3d2-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="7b3d2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b3d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b3d2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b3d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b3d2-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7b3d2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7b3d2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b3d2-107">Properties</span></span>
|<span data-ttu-id="7b3d2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b3d2-108">Property</span></span>|<span data-ttu-id="7b3d2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b3d2-109">Type</span></span>|<span data-ttu-id="7b3d2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b3d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b3d2-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="7b3d2-111">deviceImportStatus</span></span>|[<span data-ttu-id="7b3d2-112">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="7b3d2-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="7b3d2-113">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="7b3d2-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="7b3d2-114">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="7b3d2-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="7b3d2-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="7b3d2-115">deviceRegistrationId</span></span>|<span data-ttu-id="7b3d2-116">String</span><span class="sxs-lookup"><span data-stu-id="7b3d2-116">String</span></span>|<span data-ttu-id="7b3d2-117">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="7b3d2-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="7b3d2-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="7b3d2-118">deviceErrorCode</span></span>|<span data-ttu-id="7b3d2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="7b3d2-119">Int32</span></span>|<span data-ttu-id="7b3d2-120">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="7b3d2-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="7b3d2-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="7b3d2-121">deviceErrorName</span></span>|<span data-ttu-id="7b3d2-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b3d2-122">String</span></span>|<span data-ttu-id="7b3d2-123">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="7b3d2-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b3d2-124">Relações</span><span class="sxs-lookup"><span data-stu-id="7b3d2-124">Relationships</span></span>
<span data-ttu-id="7b3d2-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b3d2-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b3d2-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b3d2-126">JSON Representation</span></span>
<span data-ttu-id="7b3d2-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b3d2-127">Here is a JSON representation of the resource.</span></span>
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





