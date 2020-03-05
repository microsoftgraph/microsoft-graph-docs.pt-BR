---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1af3f40e4e128272558b6fec75d5194ef48a9f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528266"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="2f047-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="2f047-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="2f047-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2f047-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f047-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f047-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f047-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f047-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f047-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2f047-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2f047-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f047-108">Properties</span></span>
|<span data-ttu-id="2f047-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f047-109">Property</span></span>|<span data-ttu-id="2f047-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f047-110">Type</span></span>|<span data-ttu-id="2f047-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f047-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f047-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="2f047-112">deviceImportStatus</span></span>|[<span data-ttu-id="2f047-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="2f047-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="2f047-114">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="2f047-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="2f047-115">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="2f047-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="2f047-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="2f047-116">deviceRegistrationId</span></span>|<span data-ttu-id="2f047-117">String</span><span class="sxs-lookup"><span data-stu-id="2f047-117">String</span></span>|<span data-ttu-id="2f047-118">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="2f047-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="2f047-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="2f047-119">deviceErrorCode</span></span>|<span data-ttu-id="2f047-120">Int32</span><span class="sxs-lookup"><span data-stu-id="2f047-120">Int32</span></span>|<span data-ttu-id="2f047-121">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="2f047-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="2f047-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="2f047-122">deviceErrorName</span></span>|<span data-ttu-id="2f047-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f047-123">String</span></span>|<span data-ttu-id="2f047-124">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="2f047-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f047-125">Relações</span><span class="sxs-lookup"><span data-stu-id="2f047-125">Relationships</span></span>
<span data-ttu-id="2f047-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2f047-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f047-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f047-127">JSON Representation</span></span>
<span data-ttu-id="2f047-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f047-128">Here is a JSON representation of the resource.</span></span>
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



