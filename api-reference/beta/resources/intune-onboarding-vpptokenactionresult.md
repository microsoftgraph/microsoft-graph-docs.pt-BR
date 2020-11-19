---
title: tipo de recurso vppTokenActionResult
description: O status da ação executada com um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 465b4f6de73aac8af00937672d90509565804602
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256110"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="2fd45-103">tipo de recurso vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="2fd45-103">vppTokenActionResult resource type</span></span>

<span data-ttu-id="2fd45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fd45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fd45-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2fd45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fd45-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2fd45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fd45-107">O status da ação executada com um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2fd45-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="2fd45-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fd45-108">Properties</span></span>
|<span data-ttu-id="2fd45-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fd45-109">Property</span></span>|<span data-ttu-id="2fd45-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fd45-110">Type</span></span>|<span data-ttu-id="2fd45-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd45-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fd45-112">actionName</span><span class="sxs-lookup"><span data-stu-id="2fd45-112">actionName</span></span>|<span data-ttu-id="2fd45-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fd45-113">String</span></span>|<span data-ttu-id="2fd45-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="2fd45-114">Action name</span></span>|
|<span data-ttu-id="2fd45-115">actionState</span><span class="sxs-lookup"><span data-stu-id="2fd45-115">actionState</span></span>|[<span data-ttu-id="2fd45-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2fd45-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2fd45-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="2fd45-117">State of the action.</span></span> <span data-ttu-id="2fd45-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="2fd45-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2fd45-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2fd45-119">startDateTime</span></span>|<span data-ttu-id="2fd45-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fd45-120">DateTimeOffset</span></span>|<span data-ttu-id="2fd45-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="2fd45-121">Time the action was initiated</span></span>|
|<span data-ttu-id="2fd45-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fd45-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="2fd45-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fd45-123">DateTimeOffset</span></span>|<span data-ttu-id="2fd45-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="2fd45-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fd45-125">Relações</span><span class="sxs-lookup"><span data-stu-id="2fd45-125">Relationships</span></span>
<span data-ttu-id="2fd45-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fd45-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fd45-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fd45-127">JSON Representation</span></span>
<span data-ttu-id="2fd45-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2fd45-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




