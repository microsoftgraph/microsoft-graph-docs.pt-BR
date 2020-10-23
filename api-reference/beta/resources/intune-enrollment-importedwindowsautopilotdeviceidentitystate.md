---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b14b632e03160e9b56de1ad2ba0c2e32a1b74179
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728974"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="3309a-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="3309a-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="3309a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3309a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3309a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3309a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3309a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3309a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3309a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3309a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3309a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3309a-108">Properties</span></span>
|<span data-ttu-id="3309a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3309a-109">Property</span></span>|<span data-ttu-id="3309a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3309a-110">Type</span></span>|<span data-ttu-id="3309a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3309a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3309a-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="3309a-112">deviceImportStatus</span></span>|[<span data-ttu-id="3309a-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="3309a-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="3309a-114">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="3309a-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="3309a-115">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="3309a-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="3309a-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="3309a-116">deviceRegistrationId</span></span>|<span data-ttu-id="3309a-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3309a-117">String</span></span>|<span data-ttu-id="3309a-118">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="3309a-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="3309a-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="3309a-119">deviceErrorCode</span></span>|<span data-ttu-id="3309a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="3309a-120">Int32</span></span>|<span data-ttu-id="3309a-121">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="3309a-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="3309a-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="3309a-122">deviceErrorName</span></span>|<span data-ttu-id="3309a-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3309a-123">String</span></span>|<span data-ttu-id="3309a-124">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="3309a-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3309a-125">Relações</span><span class="sxs-lookup"><span data-stu-id="3309a-125">Relationships</span></span>
<span data-ttu-id="3309a-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3309a-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3309a-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3309a-127">JSON Representation</span></span>
<span data-ttu-id="3309a-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3309a-128">Here is a JSON representation of the resource.</span></span>
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





