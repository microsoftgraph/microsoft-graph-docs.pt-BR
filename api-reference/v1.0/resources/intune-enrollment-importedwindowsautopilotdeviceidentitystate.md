---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 35712bbd8bf0f13ace167cbb7d382a9ba23a319f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977427"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="f2a5b-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="f2a5b-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="f2a5b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a5b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2a5b-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f2a5b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f2a5b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2a5b-106">Properties</span></span>
|<span data-ttu-id="f2a5b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2a5b-107">Property</span></span>|<span data-ttu-id="f2a5b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2a5b-108">Type</span></span>|<span data-ttu-id="f2a5b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2a5b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2a5b-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="f2a5b-110">deviceImportStatus</span></span>|[<span data-ttu-id="f2a5b-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="f2a5b-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="f2a5b-112">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="f2a5b-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="f2a5b-113">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="f2a5b-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="f2a5b-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="f2a5b-114">deviceRegistrationId</span></span>|<span data-ttu-id="f2a5b-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2a5b-115">String</span></span>|<span data-ttu-id="f2a5b-116">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="f2a5b-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f2a5b-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="f2a5b-117">deviceErrorCode</span></span>|<span data-ttu-id="f2a5b-118">Int32</span><span class="sxs-lookup"><span data-stu-id="f2a5b-118">Int32</span></span>|<span data-ttu-id="f2a5b-119">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="f2a5b-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f2a5b-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="f2a5b-120">deviceErrorName</span></span>|<span data-ttu-id="f2a5b-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2a5b-121">String</span></span>|<span data-ttu-id="f2a5b-122">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="f2a5b-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2a5b-123">Relações</span><span class="sxs-lookup"><span data-stu-id="f2a5b-123">Relationships</span></span>
<span data-ttu-id="f2a5b-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2a5b-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f2a5b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2a5b-125">JSON Representation</span></span>
<span data-ttu-id="f2a5b-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2a5b-126">Here is a JSON representation of the resource.</span></span>
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



