---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d46aa2d4359430d17e3f3892b8b526a9efed603
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523333"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="c5109-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="c5109-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="c5109-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5109-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5109-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5109-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5109-106">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c5109-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="c5109-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5109-107">Properties</span></span>
|<span data-ttu-id="c5109-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5109-108">Property</span></span>|<span data-ttu-id="c5109-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5109-109">Type</span></span>|<span data-ttu-id="c5109-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5109-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5109-111">actionName</span><span class="sxs-lookup"><span data-stu-id="c5109-111">actionName</span></span>|<span data-ttu-id="c5109-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5109-112">String</span></span>|<span data-ttu-id="c5109-113">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="c5109-113">Action name</span></span>|
|<span data-ttu-id="c5109-114">actionState</span><span class="sxs-lookup"><span data-stu-id="c5109-114">actionState</span></span>|[<span data-ttu-id="c5109-115">actionState</span><span class="sxs-lookup"><span data-stu-id="c5109-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c5109-116">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="c5109-116">State of the action.</span></span> <span data-ttu-id="c5109-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c5109-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c5109-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c5109-118">startDateTime</span></span>|<span data-ttu-id="c5109-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5109-119">DateTimeOffset</span></span>|<span data-ttu-id="c5109-120">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="c5109-120">Time the action was initiated</span></span>|
|<span data-ttu-id="c5109-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5109-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="c5109-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5109-122">DateTimeOffset</span></span>|<span data-ttu-id="c5109-123">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="c5109-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5109-124">Relações</span><span class="sxs-lookup"><span data-stu-id="c5109-124">Relationships</span></span>
<span data-ttu-id="c5109-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c5109-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5109-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5109-126">JSON Representation</span></span>
<span data-ttu-id="c5109-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5109-127">Here is a JSON representation of the resource.</span></span>
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





