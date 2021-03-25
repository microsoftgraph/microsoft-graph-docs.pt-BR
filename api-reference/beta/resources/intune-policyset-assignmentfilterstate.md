---
title: Tipo de recurso assignmentFilterState
description: Representa o resultado da API GetState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 969d902635962a9ff89bb197f32e7d995dd9b35f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159340"
---
# <a name="assignmentfilterstate-resource-type"></a><span data-ttu-id="2b8f5-103">Tipo de recurso assignmentFilterState</span><span class="sxs-lookup"><span data-stu-id="2b8f5-103">assignmentFilterState resource type</span></span>

<span data-ttu-id="2b8f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b8f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b8f5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b8f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b8f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b8f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b8f5-107">Representa o resultado da API GetState.</span><span class="sxs-lookup"><span data-stu-id="2b8f5-107">Represents result of GetState API.</span></span>

## <a name="properties"></a><span data-ttu-id="2b8f5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b8f5-108">Properties</span></span>
|<span data-ttu-id="2b8f5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b8f5-109">Property</span></span>|<span data-ttu-id="2b8f5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b8f5-110">Type</span></span>|<span data-ttu-id="2b8f5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b8f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b8f5-112">enabled</span><span class="sxs-lookup"><span data-stu-id="2b8f5-112">enabled</span></span>|<span data-ttu-id="2b8f5-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b8f5-113">Boolean</span></span>|<span data-ttu-id="2b8f5-114">Indicador para se AssignmentFilter estiver habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="2b8f5-114">Indicator to if AssignmentFilter is enabled or disabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b8f5-115">Relações</span><span class="sxs-lookup"><span data-stu-id="2b8f5-115">Relationships</span></span>
<span data-ttu-id="2b8f5-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b8f5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b8f5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b8f5-117">JSON Representation</span></span>
<span data-ttu-id="2b8f5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b8f5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterState",
  "enabled": true
}
```




