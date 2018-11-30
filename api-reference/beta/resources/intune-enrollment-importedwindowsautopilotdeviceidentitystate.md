---
title: Tipo de recurso importedWindowsAutopilotDeviceIdentityState
description: Ainda não documentado
ms.openlocfilehash: cdb13df520d109ddcc49e2637652499186ac9f24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037976"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="47df2-103">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="47df2-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="47df2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="47df2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47df2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="47df2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47df2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="47df2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47df2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="47df2-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="47df2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47df2-108">Properties</span></span>
|<span data-ttu-id="47df2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47df2-109">Property</span></span>|<span data-ttu-id="47df2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="47df2-110">Type</span></span>|<span data-ttu-id="47df2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="47df2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47df2-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="47df2-112">deviceImportStatus</span></span>|[<span data-ttu-id="47df2-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="47df2-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="47df2-114">Status do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="47df2-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="47df2-115">Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="47df2-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="47df2-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="47df2-116">deviceRegistrationId</span></span>|<span data-ttu-id="47df2-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47df2-117">String</span></span>|<span data-ttu-id="47df2-118">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="47df2-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="47df2-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="47df2-119">deviceErrorCode</span></span>|<span data-ttu-id="47df2-120">Int32</span><span class="sxs-lookup"><span data-stu-id="47df2-120">Int32</span></span>|<span data-ttu-id="47df2-121">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="47df2-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="47df2-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="47df2-122">deviceErrorName</span></span>|<span data-ttu-id="47df2-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47df2-123">String</span></span>|<span data-ttu-id="47df2-124">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="47df2-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="47df2-125">Relações</span><span class="sxs-lookup"><span data-stu-id="47df2-125">Relationships</span></span>
<span data-ttu-id="47df2-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47df2-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47df2-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47df2-127">JSON Representation</span></span>
<span data-ttu-id="47df2-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47df2-128">Here is a JSON representation of the resource.</span></span>
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





