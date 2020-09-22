---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20a5d4ef3fe2dc79c3843d86c525086940a8d78c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079932"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="c43f1-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="c43f1-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="c43f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c43f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c43f1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c43f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c43f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c43f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c43f1-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c43f1-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c43f1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c43f1-108">Properties</span></span>
|<span data-ttu-id="c43f1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c43f1-109">Property</span></span>|<span data-ttu-id="c43f1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c43f1-110">Type</span></span>|<span data-ttu-id="c43f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c43f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c43f1-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="c43f1-112">deviceImportStatus</span></span>|[<span data-ttu-id="c43f1-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="c43f1-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="c43f1-114">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="c43f1-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="c43f1-115">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="c43f1-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="c43f1-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="c43f1-116">deviceRegistrationId</span></span>|<span data-ttu-id="c43f1-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c43f1-117">String</span></span>|<span data-ttu-id="c43f1-118">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="c43f1-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="c43f1-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="c43f1-119">deviceErrorCode</span></span>|<span data-ttu-id="c43f1-120">Int32</span><span class="sxs-lookup"><span data-stu-id="c43f1-120">Int32</span></span>|<span data-ttu-id="c43f1-121">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="c43f1-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="c43f1-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="c43f1-122">deviceErrorName</span></span>|<span data-ttu-id="c43f1-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c43f1-123">String</span></span>|<span data-ttu-id="c43f1-124">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="c43f1-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c43f1-125">Relações</span><span class="sxs-lookup"><span data-stu-id="c43f1-125">Relationships</span></span>
<span data-ttu-id="c43f1-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c43f1-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c43f1-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c43f1-127">JSON Representation</span></span>
<span data-ttu-id="c43f1-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c43f1-128">Here is a JSON representation of the resource.</span></span>
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






