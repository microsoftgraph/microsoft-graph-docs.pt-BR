---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 051d5f381e27e4901f7e2fb9280cea3dc0bb71c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806101"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="da780-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="da780-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="da780-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da780-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da780-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da780-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da780-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="da780-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da780-107">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="da780-107">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="da780-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da780-108">Properties</span></span>
|<span data-ttu-id="da780-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da780-109">Property</span></span>|<span data-ttu-id="da780-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="da780-110">Type</span></span>|<span data-ttu-id="da780-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da780-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da780-112">actionName</span><span class="sxs-lookup"><span data-stu-id="da780-112">actionName</span></span>|<span data-ttu-id="da780-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da780-113">String</span></span>|<span data-ttu-id="da780-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="da780-114">Action name</span></span>|
|<span data-ttu-id="da780-115">actionState</span><span class="sxs-lookup"><span data-stu-id="da780-115">actionState</span></span>|[<span data-ttu-id="da780-116">actionState</span><span class="sxs-lookup"><span data-stu-id="da780-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="da780-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="da780-117">State of the action.</span></span> <span data-ttu-id="da780-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="da780-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="da780-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="da780-119">startDateTime</span></span>|<span data-ttu-id="da780-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da780-120">DateTimeOffset</span></span>|<span data-ttu-id="da780-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="da780-121">Time the action was initiated</span></span>|
|<span data-ttu-id="da780-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="da780-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="da780-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da780-123">DateTimeOffset</span></span>|<span data-ttu-id="da780-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="da780-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="da780-125">Relações</span><span class="sxs-lookup"><span data-stu-id="da780-125">Relationships</span></span>
<span data-ttu-id="da780-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da780-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="da780-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da780-127">JSON Representation</span></span>
<span data-ttu-id="da780-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da780-128">Here is a JSON representation of the resource.</span></span>
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





