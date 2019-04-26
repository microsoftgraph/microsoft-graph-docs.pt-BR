---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42726817395296945fc593552ee50154fa34d332
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567099"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="64e94-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="64e94-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="64e94-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64e94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64e94-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64e94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64e94-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64e94-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="64e94-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64e94-107">Properties</span></span>
|<span data-ttu-id="64e94-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64e94-108">Property</span></span>|<span data-ttu-id="64e94-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="64e94-109">Type</span></span>|<span data-ttu-id="64e94-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="64e94-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64e94-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="64e94-111">deviceImportStatus</span></span>|[<span data-ttu-id="64e94-112">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="64e94-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="64e94-113">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="64e94-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="64e94-114">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="64e94-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="64e94-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="64e94-115">deviceRegistrationId</span></span>|<span data-ttu-id="64e94-116">String</span><span class="sxs-lookup"><span data-stu-id="64e94-116">String</span></span>|<span data-ttu-id="64e94-117">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="64e94-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="64e94-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="64e94-118">deviceErrorCode</span></span>|<span data-ttu-id="64e94-119">Int32</span><span class="sxs-lookup"><span data-stu-id="64e94-119">Int32</span></span>|<span data-ttu-id="64e94-120">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="64e94-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="64e94-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="64e94-121">deviceErrorName</span></span>|<span data-ttu-id="64e94-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64e94-122">String</span></span>|<span data-ttu-id="64e94-123">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="64e94-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="64e94-124">Relações</span><span class="sxs-lookup"><span data-stu-id="64e94-124">Relationships</span></span>
<span data-ttu-id="64e94-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64e94-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64e94-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64e94-126">JSON Representation</span></span>
<span data-ttu-id="64e94-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64e94-127">Here is a JSON representation of the resource.</span></span>
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





