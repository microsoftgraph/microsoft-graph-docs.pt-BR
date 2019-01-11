---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8017ac803ffa07a2e122553dee3268b0193157f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869570"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="515d7-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="515d7-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="515d7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="515d7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="515d7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="515d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="515d7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="515d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="515d7-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="515d7-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="515d7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="515d7-108">Properties</span></span>
|<span data-ttu-id="515d7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="515d7-109">Property</span></span>|<span data-ttu-id="515d7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="515d7-110">Type</span></span>|<span data-ttu-id="515d7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="515d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="515d7-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="515d7-112">deviceImportStatus</span></span>|[<span data-ttu-id="515d7-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="515d7-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="515d7-114">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="515d7-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="515d7-115">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="515d7-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="515d7-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="515d7-116">deviceRegistrationId</span></span>|<span data-ttu-id="515d7-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="515d7-117">String</span></span>|<span data-ttu-id="515d7-118">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="515d7-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="515d7-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="515d7-119">deviceErrorCode</span></span>|<span data-ttu-id="515d7-120">Int32</span><span class="sxs-lookup"><span data-stu-id="515d7-120">Int32</span></span>|<span data-ttu-id="515d7-121">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="515d7-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="515d7-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="515d7-122">deviceErrorName</span></span>|<span data-ttu-id="515d7-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="515d7-123">String</span></span>|<span data-ttu-id="515d7-124">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="515d7-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="515d7-125">Relações</span><span class="sxs-lookup"><span data-stu-id="515d7-125">Relationships</span></span>
<span data-ttu-id="515d7-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="515d7-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="515d7-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="515d7-127">JSON Representation</span></span>
<span data-ttu-id="515d7-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="515d7-128">Here is a JSON representation of the resource.</span></span>
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





