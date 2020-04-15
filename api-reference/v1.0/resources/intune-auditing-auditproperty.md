---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f306fbbf1d93386e4ffd963199c4e6d54296ce26
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439515"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="b9f00-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="b9f00-103">auditProperty resource type</span></span>

<span data-ttu-id="b9f00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9f00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9f00-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9f00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9f00-106">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="b9f00-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="b9f00-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9f00-107">Properties</span></span>
|<span data-ttu-id="b9f00-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9f00-108">Property</span></span>|<span data-ttu-id="b9f00-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9f00-109">Type</span></span>|<span data-ttu-id="b9f00-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9f00-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9f00-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b9f00-111">displayName</span></span>|<span data-ttu-id="b9f00-112">String</span><span class="sxs-lookup"><span data-stu-id="b9f00-112">String</span></span>|<span data-ttu-id="b9f00-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b9f00-113">Display name.</span></span>|
|<span data-ttu-id="b9f00-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="b9f00-114">oldValue</span></span>|<span data-ttu-id="b9f00-115">String</span><span class="sxs-lookup"><span data-stu-id="b9f00-115">String</span></span>|<span data-ttu-id="b9f00-116">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="b9f00-116">Old value.</span></span>|
|<span data-ttu-id="b9f00-117">newValue</span><span class="sxs-lookup"><span data-stu-id="b9f00-117">newValue</span></span>|<span data-ttu-id="b9f00-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9f00-118">String</span></span>|<span data-ttu-id="b9f00-119">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="b9f00-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9f00-120">Relações</span><span class="sxs-lookup"><span data-stu-id="b9f00-120">Relationships</span></span>
<span data-ttu-id="b9f00-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9f00-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9f00-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9f00-122">JSON Representation</span></span>
<span data-ttu-id="b9f00-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9f00-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```







