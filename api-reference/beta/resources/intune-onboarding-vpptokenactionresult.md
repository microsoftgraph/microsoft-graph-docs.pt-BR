---
title: tipo de recurso vppTokenActionResult
description: O status da ação executada com um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0cc4856901af4f97fde87acc57916742a27186ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029348"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="75216-103">tipo de recurso vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="75216-103">vppTokenActionResult resource type</span></span>

<span data-ttu-id="75216-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75216-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75216-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75216-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75216-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75216-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75216-107">O status da ação executada com um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="75216-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="75216-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75216-108">Properties</span></span>
|<span data-ttu-id="75216-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75216-109">Property</span></span>|<span data-ttu-id="75216-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="75216-110">Type</span></span>|<span data-ttu-id="75216-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75216-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75216-112">actionName</span><span class="sxs-lookup"><span data-stu-id="75216-112">actionName</span></span>|<span data-ttu-id="75216-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75216-113">String</span></span>|<span data-ttu-id="75216-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="75216-114">Action name</span></span>|
|<span data-ttu-id="75216-115">actionState</span><span class="sxs-lookup"><span data-stu-id="75216-115">actionState</span></span>|[<span data-ttu-id="75216-116">actionState</span><span class="sxs-lookup"><span data-stu-id="75216-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="75216-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="75216-117">State of the action.</span></span> <span data-ttu-id="75216-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="75216-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="75216-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="75216-119">startDateTime</span></span>|<span data-ttu-id="75216-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75216-120">DateTimeOffset</span></span>|<span data-ttu-id="75216-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="75216-121">Time the action was initiated</span></span>|
|<span data-ttu-id="75216-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="75216-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="75216-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75216-123">DateTimeOffset</span></span>|<span data-ttu-id="75216-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="75216-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="75216-125">Relações</span><span class="sxs-lookup"><span data-stu-id="75216-125">Relationships</span></span>
<span data-ttu-id="75216-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75216-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75216-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75216-127">JSON Representation</span></span>
<span data-ttu-id="75216-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75216-128">Here is a JSON representation of the resource.</span></span>
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






