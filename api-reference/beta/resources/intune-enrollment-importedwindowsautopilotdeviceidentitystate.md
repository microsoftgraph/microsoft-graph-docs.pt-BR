---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: b8df80f71e6767e22a35db2d82a18e0a7263342d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304505"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="25922-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="25922-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="25922-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="25922-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25922-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="25922-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25922-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="25922-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25922-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="25922-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="25922-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25922-108">Properties</span></span>
|<span data-ttu-id="25922-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25922-109">Property</span></span>|<span data-ttu-id="25922-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="25922-110">Type</span></span>|<span data-ttu-id="25922-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="25922-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25922-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="25922-112">deviceImportStatus</span></span>|[<span data-ttu-id="25922-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="25922-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="25922-114">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="25922-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="25922-115">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="25922-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="25922-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="25922-116">deviceRegistrationId</span></span>|<span data-ttu-id="25922-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25922-117">String</span></span>|<span data-ttu-id="25922-118">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="25922-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="25922-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="25922-119">deviceErrorCode</span></span>|<span data-ttu-id="25922-120">Int32</span><span class="sxs-lookup"><span data-stu-id="25922-120">Int32</span></span>|<span data-ttu-id="25922-121">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="25922-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="25922-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="25922-122">deviceErrorName</span></span>|<span data-ttu-id="25922-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25922-123">String</span></span>|<span data-ttu-id="25922-124">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="25922-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="25922-125">Relações</span><span class="sxs-lookup"><span data-stu-id="25922-125">Relationships</span></span>
<span data-ttu-id="25922-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25922-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="25922-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25922-127">JSON Representation</span></span>
<span data-ttu-id="25922-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25922-128">Here is a JSON representation of the resource.</span></span>
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





