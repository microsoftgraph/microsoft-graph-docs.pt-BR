---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 22fd8e1bc338191bba54ba9f655f03899054ae86
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912299"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="2b994-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="2b994-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="2b994-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2b994-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b994-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2b994-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b994-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2b994-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b994-107">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="2b994-107">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="2b994-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b994-108">Properties</span></span>
|<span data-ttu-id="2b994-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b994-109">Property</span></span>|<span data-ttu-id="2b994-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b994-110">Type</span></span>|<span data-ttu-id="2b994-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b994-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b994-112">actionName</span><span class="sxs-lookup"><span data-stu-id="2b994-112">actionName</span></span>|<span data-ttu-id="2b994-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b994-113">String</span></span>|<span data-ttu-id="2b994-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="2b994-114">Action name</span></span>|
|<span data-ttu-id="2b994-115">actionState</span><span class="sxs-lookup"><span data-stu-id="2b994-115">actionState</span></span>|[<span data-ttu-id="2b994-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2b994-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2b994-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="2b994-117">State of the action.</span></span> <span data-ttu-id="2b994-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="2b994-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2b994-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2b994-119">startDateTime</span></span>|<span data-ttu-id="2b994-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b994-120">DateTimeOffset</span></span>|<span data-ttu-id="2b994-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="2b994-121">Time the action was initiated</span></span>|
|<span data-ttu-id="2b994-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b994-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="2b994-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b994-123">DateTimeOffset</span></span>|<span data-ttu-id="2b994-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="2b994-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b994-125">Relações</span><span class="sxs-lookup"><span data-stu-id="2b994-125">Relationships</span></span>
<span data-ttu-id="2b994-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b994-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2b994-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b994-127">JSON Representation</span></span>
<span data-ttu-id="2b994-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b994-128">Here is a JSON representation of the resource.</span></span>
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





