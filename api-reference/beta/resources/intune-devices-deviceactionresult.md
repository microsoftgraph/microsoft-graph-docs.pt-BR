---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6bdbadcda27116803522a16cd43c7f642b342d7d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983117"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="5a534-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="5a534-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="5a534-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5a534-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a534-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a534-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a534-106">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a534-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="5a534-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a534-107">Properties</span></span>
|<span data-ttu-id="5a534-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a534-108">Property</span></span>|<span data-ttu-id="5a534-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a534-109">Type</span></span>|<span data-ttu-id="5a534-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a534-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a534-111">actionName</span><span class="sxs-lookup"><span data-stu-id="5a534-111">actionName</span></span>|<span data-ttu-id="5a534-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a534-112">String</span></span>|<span data-ttu-id="5a534-113">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="5a534-113">Action name</span></span>|
|<span data-ttu-id="5a534-114">actionState</span><span class="sxs-lookup"><span data-stu-id="5a534-114">actionState</span></span>|[<span data-ttu-id="5a534-115">actionState</span><span class="sxs-lookup"><span data-stu-id="5a534-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="5a534-116">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="5a534-116">State of the action.</span></span> <span data-ttu-id="5a534-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="5a534-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5a534-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5a534-118">startDateTime</span></span>|<span data-ttu-id="5a534-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a534-119">DateTimeOffset</span></span>|<span data-ttu-id="5a534-120">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="5a534-120">Time the action was initiated</span></span>|
|<span data-ttu-id="5a534-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a534-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="5a534-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a534-122">DateTimeOffset</span></span>|<span data-ttu-id="5a534-123">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="5a534-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a534-124">Relações</span><span class="sxs-lookup"><span data-stu-id="5a534-124">Relationships</span></span>
<span data-ttu-id="5a534-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a534-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a534-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a534-126">JSON Representation</span></span>
<span data-ttu-id="5a534-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a534-127">Here is a JSON representation of the resource.</span></span>
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





