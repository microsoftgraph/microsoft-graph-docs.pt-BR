---
title: Tipo de recurso resourceAction
description: Conjunto de ações permitidas e não permitidas para um recurso.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3517a4608691b65ce33ac40b4a9d9929bd277f31
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752431"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="1fc22-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="1fc22-103">resourceAction resource type</span></span>

<span data-ttu-id="1fc22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fc22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fc22-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fc22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fc22-106">Conjunto de ações permitidas e não permitidas para um recurso.</span><span class="sxs-lookup"><span data-stu-id="1fc22-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="1fc22-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fc22-107">Properties</span></span>
|<span data-ttu-id="1fc22-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fc22-108">Property</span></span>|<span data-ttu-id="1fc22-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fc22-109">Type</span></span>|<span data-ttu-id="1fc22-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fc22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fc22-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="1fc22-111">allowedResourceActions</span></span>|<span data-ttu-id="1fc22-112">String collection</span><span class="sxs-lookup"><span data-stu-id="1fc22-112">String collection</span></span>|<span data-ttu-id="1fc22-113">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="1fc22-113">Allowed Actions</span></span>|
|<span data-ttu-id="1fc22-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="1fc22-114">notAllowedResourceActions</span></span>|<span data-ttu-id="1fc22-115">String collection</span><span class="sxs-lookup"><span data-stu-id="1fc22-115">String collection</span></span>|<span data-ttu-id="1fc22-116">Ações não permitidas.</span><span class="sxs-lookup"><span data-stu-id="1fc22-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fc22-117">Relações</span><span class="sxs-lookup"><span data-stu-id="1fc22-117">Relationships</span></span>
<span data-ttu-id="1fc22-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1fc22-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fc22-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fc22-119">JSON Representation</span></span>
<span data-ttu-id="1fc22-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fc22-120">Here is a JSON representation of the resource.</span></span>
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




