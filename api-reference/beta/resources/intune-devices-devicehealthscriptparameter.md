---
title: tipo de recurso deviceHealthScriptParameter
description: Propriedades básicas do parâmetro script.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad82da1915702448a62c0c99f6933ddf1a51c5b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060297"
---
# <a name="devicehealthscriptparameter-resource-type"></a><span data-ttu-id="d762c-103">tipo de recurso deviceHealthScriptParameter</span><span class="sxs-lookup"><span data-stu-id="d762c-103">deviceHealthScriptParameter resource type</span></span>

<span data-ttu-id="d762c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d762c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d762c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d762c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d762c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d762c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d762c-107">Propriedades básicas do parâmetro script.</span><span class="sxs-lookup"><span data-stu-id="d762c-107">Base properties of the script parameter.</span></span>

## <a name="properties"></a><span data-ttu-id="d762c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d762c-108">Properties</span></span>
|<span data-ttu-id="d762c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d762c-109">Property</span></span>|<span data-ttu-id="d762c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d762c-110">Type</span></span>|<span data-ttu-id="d762c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d762c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d762c-112">name</span><span class="sxs-lookup"><span data-stu-id="d762c-112">name</span></span>|<span data-ttu-id="d762c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d762c-113">String</span></span>|<span data-ttu-id="d762c-114">O nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="d762c-114">The name of the param</span></span>|
|<span data-ttu-id="d762c-115">description</span><span class="sxs-lookup"><span data-stu-id="d762c-115">description</span></span>|<span data-ttu-id="d762c-116">String</span><span class="sxs-lookup"><span data-stu-id="d762c-116">String</span></span>|<span data-ttu-id="d762c-117">A descrição do parâmetro</span><span class="sxs-lookup"><span data-stu-id="d762c-117">The description of the param</span></span>|
|<span data-ttu-id="d762c-118">isRequired</span><span class="sxs-lookup"><span data-stu-id="d762c-118">isRequired</span></span>|<span data-ttu-id="d762c-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="d762c-119">Boolean</span></span>|<span data-ttu-id="d762c-120">Se o parâmetro é obrigatório</span><span class="sxs-lookup"><span data-stu-id="d762c-120">Whether the param is required</span></span>|
|<span data-ttu-id="d762c-121">applyDefaultValueWhenNotAssigned</span><span class="sxs-lookup"><span data-stu-id="d762c-121">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="d762c-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="d762c-122">Boolean</span></span>|<span data-ttu-id="d762c-123">Se aplicar DefaultValue quando não atribuído</span><span class="sxs-lookup"><span data-stu-id="d762c-123">Whether Apply DefaultValue When Not Assigned</span></span>|

## <a name="relationships"></a><span data-ttu-id="d762c-124">Relações</span><span class="sxs-lookup"><span data-stu-id="d762c-124">Relationships</span></span>
<span data-ttu-id="d762c-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d762c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d762c-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d762c-126">JSON Representation</span></span>
<span data-ttu-id="d762c-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d762c-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true
}
```






