---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0f4e76b23d4d970a9fb873326dc84f278aa2ed2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410963"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="bdaa2-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="bdaa2-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="bdaa2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bdaa2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdaa2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdaa2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bdaa2-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bdaa2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdaa2-108">Properties</span></span>
|<span data-ttu-id="bdaa2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdaa2-109">Property</span></span>|<span data-ttu-id="bdaa2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdaa2-110">Type</span></span>|<span data-ttu-id="bdaa2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdaa2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdaa2-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="bdaa2-112">deviceImportStatus</span></span>|[<span data-ttu-id="bdaa2-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="bdaa2-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="bdaa2-114">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="bdaa2-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="bdaa2-115">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="bdaa2-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="bdaa2-116">deviceRegistrationId</span></span>|<span data-ttu-id="bdaa2-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdaa2-117">String</span></span>|<span data-ttu-id="bdaa2-118">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="bdaa2-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="bdaa2-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="bdaa2-119">deviceErrorCode</span></span>|<span data-ttu-id="bdaa2-120">Int32</span><span class="sxs-lookup"><span data-stu-id="bdaa2-120">Int32</span></span>|<span data-ttu-id="bdaa2-121">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="bdaa2-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="bdaa2-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="bdaa2-122">deviceErrorName</span></span>|<span data-ttu-id="bdaa2-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdaa2-123">String</span></span>|<span data-ttu-id="bdaa2-124">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="bdaa2-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdaa2-125">Relações</span><span class="sxs-lookup"><span data-stu-id="bdaa2-125">Relationships</span></span>
<span data-ttu-id="bdaa2-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bdaa2-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bdaa2-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdaa2-127">JSON Representation</span></span>
<span data-ttu-id="bdaa2-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdaa2-128">Here is a JSON representation of the resource.</span></span>
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




