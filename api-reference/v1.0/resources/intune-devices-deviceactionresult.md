---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: tfitzmac
ms.openlocfilehash: 48429e059616d9af0e3cbdac8544e68354b94fb5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320542"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="79d63-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="79d63-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="79d63-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="79d63-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79d63-105">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="79d63-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="79d63-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79d63-106">Properties</span></span>
|<span data-ttu-id="79d63-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79d63-107">Property</span></span>|<span data-ttu-id="79d63-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="79d63-108">Type</span></span>|<span data-ttu-id="79d63-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="79d63-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79d63-110">actionName</span><span class="sxs-lookup"><span data-stu-id="79d63-110">actionName</span></span>|<span data-ttu-id="79d63-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79d63-111">String</span></span>|<span data-ttu-id="79d63-112">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="79d63-112">Action name</span></span>|
|<span data-ttu-id="79d63-113">actionState</span><span class="sxs-lookup"><span data-stu-id="79d63-113">actionState</span></span>|[<span data-ttu-id="79d63-114">actionState</span><span class="sxs-lookup"><span data-stu-id="79d63-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="79d63-115">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="79d63-115">State of the action.</span></span> <span data-ttu-id="79d63-116">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="79d63-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="79d63-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="79d63-117">startDateTime</span></span>|<span data-ttu-id="79d63-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d63-118">DateTimeOffset</span></span>|<span data-ttu-id="79d63-119">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="79d63-119">Time the action was initiated</span></span>|
|<span data-ttu-id="79d63-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="79d63-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="79d63-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d63-121">DateTimeOffset</span></span>|<span data-ttu-id="79d63-122">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="79d63-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="79d63-123">Relações</span><span class="sxs-lookup"><span data-stu-id="79d63-123">Relationships</span></span>
<span data-ttu-id="79d63-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79d63-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="79d63-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79d63-125">JSON Representation</span></span>
<span data-ttu-id="79d63-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79d63-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



