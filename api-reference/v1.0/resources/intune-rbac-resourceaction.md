---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88ea0c947a87135f874755f49d0847a3c2a08fae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037153"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="8eeaf-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="8eeaf-103">resourceAction resource type</span></span>

> <span data-ttu-id="8eeaf-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8eeaf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eeaf-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8eeaf-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8eeaf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8eeaf-106">Properties</span></span>
|<span data-ttu-id="8eeaf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8eeaf-107">Property</span></span>|<span data-ttu-id="8eeaf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8eeaf-108">Type</span></span>|<span data-ttu-id="8eeaf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8eeaf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eeaf-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="8eeaf-110">allowedResourceActions</span></span>|<span data-ttu-id="8eeaf-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eeaf-111">String collection</span></span>|<span data-ttu-id="8eeaf-112">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="8eeaf-112">Allowed Actions</span></span>|
|<span data-ttu-id="8eeaf-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="8eeaf-113">notAllowedResourceActions</span></span>|<span data-ttu-id="8eeaf-114">String collection</span><span class="sxs-lookup"><span data-stu-id="8eeaf-114">String collection</span></span>|<span data-ttu-id="8eeaf-115">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="8eeaf-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="8eeaf-116">Relações</span><span class="sxs-lookup"><span data-stu-id="8eeaf-116">Relationships</span></span>
<span data-ttu-id="8eeaf-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8eeaf-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8eeaf-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8eeaf-118">JSON Representation</span></span>
<span data-ttu-id="8eeaf-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8eeaf-119">Here is a JSON representation of the resource.</span></span>
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



