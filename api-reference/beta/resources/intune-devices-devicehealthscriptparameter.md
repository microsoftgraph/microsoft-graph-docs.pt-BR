---
title: tipo de recurso deviceHealthScriptParameter
description: Propriedades básicas do parâmetro script.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a11915af80b10944fe6a3573d5293c19e3fc0357
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729345"
---
# <a name="devicehealthscriptparameter-resource-type"></a><span data-ttu-id="129f4-103">tipo de recurso deviceHealthScriptParameter</span><span class="sxs-lookup"><span data-stu-id="129f4-103">deviceHealthScriptParameter resource type</span></span>

<span data-ttu-id="129f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="129f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="129f4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="129f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="129f4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="129f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="129f4-107">Propriedades básicas do parâmetro script.</span><span class="sxs-lookup"><span data-stu-id="129f4-107">Base properties of the script parameter.</span></span>

## <a name="properties"></a><span data-ttu-id="129f4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="129f4-108">Properties</span></span>
|<span data-ttu-id="129f4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="129f4-109">Property</span></span>|<span data-ttu-id="129f4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="129f4-110">Type</span></span>|<span data-ttu-id="129f4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="129f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="129f4-112">nome</span><span class="sxs-lookup"><span data-stu-id="129f4-112">name</span></span>|<span data-ttu-id="129f4-113">String</span><span class="sxs-lookup"><span data-stu-id="129f4-113">String</span></span>|<span data-ttu-id="129f4-114">O nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="129f4-114">The name of the param</span></span>|
|<span data-ttu-id="129f4-115">description</span><span class="sxs-lookup"><span data-stu-id="129f4-115">description</span></span>|<span data-ttu-id="129f4-116">String</span><span class="sxs-lookup"><span data-stu-id="129f4-116">String</span></span>|<span data-ttu-id="129f4-117">A descrição do parâmetro</span><span class="sxs-lookup"><span data-stu-id="129f4-117">The description of the param</span></span>|
|<span data-ttu-id="129f4-118">isRequired</span><span class="sxs-lookup"><span data-stu-id="129f4-118">isRequired</span></span>|<span data-ttu-id="129f4-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="129f4-119">Boolean</span></span>|<span data-ttu-id="129f4-120">Se o parâmetro é obrigatório</span><span class="sxs-lookup"><span data-stu-id="129f4-120">Whether the param is required</span></span>|
|<span data-ttu-id="129f4-121">applyDefaultValueWhenNotAssigned</span><span class="sxs-lookup"><span data-stu-id="129f4-121">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="129f4-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="129f4-122">Boolean</span></span>|<span data-ttu-id="129f4-123">Se aplicar DefaultValue quando não atribuído</span><span class="sxs-lookup"><span data-stu-id="129f4-123">Whether Apply DefaultValue When Not Assigned</span></span>|

## <a name="relationships"></a><span data-ttu-id="129f4-124">Relações</span><span class="sxs-lookup"><span data-stu-id="129f4-124">Relationships</span></span>
<span data-ttu-id="129f4-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="129f4-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="129f4-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="129f4-126">JSON Representation</span></span>
<span data-ttu-id="129f4-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="129f4-127">Here is a JSON representation of the resource.</span></span>
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





