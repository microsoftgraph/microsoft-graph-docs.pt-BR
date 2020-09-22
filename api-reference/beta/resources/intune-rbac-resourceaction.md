---
title: Tipo de recurso resourceAction
description: Conjunto de ações permitidas e não permitidas para um recurso.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c7b38b3b534465145e30076c175d9da96f25b062
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095223"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="a1791-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="a1791-103">resourceAction resource type</span></span>

<span data-ttu-id="a1791-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1791-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1791-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1791-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1791-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1791-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1791-107">Conjunto de ações permitidas e não permitidas para um recurso.</span><span class="sxs-lookup"><span data-stu-id="a1791-107">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a1791-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1791-108">Properties</span></span>
|<span data-ttu-id="a1791-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1791-109">Property</span></span>|<span data-ttu-id="a1791-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1791-110">Type</span></span>|<span data-ttu-id="a1791-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1791-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1791-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a1791-112">allowedResourceActions</span></span>|<span data-ttu-id="a1791-113">String collection</span><span class="sxs-lookup"><span data-stu-id="a1791-113">String collection</span></span>|<span data-ttu-id="a1791-114">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="a1791-114">Allowed Actions</span></span>|
|<span data-ttu-id="a1791-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a1791-115">notAllowedResourceActions</span></span>|<span data-ttu-id="a1791-116">String collection</span><span class="sxs-lookup"><span data-stu-id="a1791-116">String collection</span></span>|<span data-ttu-id="a1791-117">Ações não permitidas.</span><span class="sxs-lookup"><span data-stu-id="a1791-117">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1791-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a1791-118">Relationships</span></span>
<span data-ttu-id="a1791-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1791-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1791-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1791-120">JSON Representation</span></span>
<span data-ttu-id="a1791-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a1791-121">Here is a JSON representation of the resource.</span></span>
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






