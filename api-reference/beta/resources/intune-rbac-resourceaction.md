---
title: Tipo de recurso resourceAction
description: Conjunto de ações permitidas e não permitidas para um recurso.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b8d176b64b6eacc7fbf34a4fe5e15a88da709f2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733179"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="b28b7-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="b28b7-103">resourceAction resource type</span></span>

<span data-ttu-id="b28b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b28b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b28b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b28b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b28b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b28b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b28b7-107">Conjunto de ações permitidas e não permitidas para um recurso.</span><span class="sxs-lookup"><span data-stu-id="b28b7-107">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="b28b7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b28b7-108">Properties</span></span>
|<span data-ttu-id="b28b7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b28b7-109">Property</span></span>|<span data-ttu-id="b28b7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b28b7-110">Type</span></span>|<span data-ttu-id="b28b7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b28b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b28b7-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="b28b7-112">allowedResourceActions</span></span>|<span data-ttu-id="b28b7-113">String collection</span><span class="sxs-lookup"><span data-stu-id="b28b7-113">String collection</span></span>|<span data-ttu-id="b28b7-114">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="b28b7-114">Allowed Actions</span></span>|
|<span data-ttu-id="b28b7-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="b28b7-115">notAllowedResourceActions</span></span>|<span data-ttu-id="b28b7-116">String collection</span><span class="sxs-lookup"><span data-stu-id="b28b7-116">String collection</span></span>|<span data-ttu-id="b28b7-117">Ações não permitidas.</span><span class="sxs-lookup"><span data-stu-id="b28b7-117">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b28b7-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b28b7-118">Relationships</span></span>
<span data-ttu-id="b28b7-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b28b7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b28b7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b28b7-120">JSON Representation</span></span>
<span data-ttu-id="b28b7-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b28b7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```





