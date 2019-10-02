---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bff6bfde2816292b57e31bca81cf085297ee537f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355971"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="13173-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="13173-103">auditResource resource type</span></span>

> <span data-ttu-id="13173-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13173-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13173-105">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="13173-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="13173-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13173-106">Properties</span></span>
|<span data-ttu-id="13173-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13173-107">Property</span></span>|<span data-ttu-id="13173-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="13173-108">Type</span></span>|<span data-ttu-id="13173-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="13173-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13173-110">displayName</span><span class="sxs-lookup"><span data-stu-id="13173-110">displayName</span></span>|<span data-ttu-id="13173-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13173-111">String</span></span>|<span data-ttu-id="13173-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="13173-112">Display name.</span></span>|
|<span data-ttu-id="13173-113">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="13173-113">modifiedProperties</span></span>|<span data-ttu-id="13173-114">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="13173-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="13173-115">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="13173-115">List of modified properties.</span></span>|
|<span data-ttu-id="13173-116">type</span><span class="sxs-lookup"><span data-stu-id="13173-116">type</span></span>|<span data-ttu-id="13173-117">String</span><span class="sxs-lookup"><span data-stu-id="13173-117">String</span></span>|<span data-ttu-id="13173-118">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="13173-118">Audit resource's type.</span></span>|
|<span data-ttu-id="13173-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="13173-119">resourceId</span></span>|<span data-ttu-id="13173-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13173-120">String</span></span>|<span data-ttu-id="13173-121">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="13173-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13173-122">Relações</span><span class="sxs-lookup"><span data-stu-id="13173-122">Relationships</span></span>
<span data-ttu-id="13173-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13173-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13173-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13173-124">JSON Representation</span></span>
<span data-ttu-id="13173-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13173-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```




