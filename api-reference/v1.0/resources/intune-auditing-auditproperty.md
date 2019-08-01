---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2a3e4ed10a756c4d1cb62bf98c1b6cb13d6f22c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032050"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="16254-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="16254-103">auditProperty resource type</span></span>

> <span data-ttu-id="16254-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16254-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16254-105">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="16254-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="16254-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16254-106">Properties</span></span>
|<span data-ttu-id="16254-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16254-107">Property</span></span>|<span data-ttu-id="16254-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="16254-108">Type</span></span>|<span data-ttu-id="16254-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="16254-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16254-110">displayName</span><span class="sxs-lookup"><span data-stu-id="16254-110">displayName</span></span>|<span data-ttu-id="16254-111">String</span><span class="sxs-lookup"><span data-stu-id="16254-111">String</span></span>|<span data-ttu-id="16254-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="16254-112">Display name.</span></span>|
|<span data-ttu-id="16254-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="16254-113">oldValue</span></span>|<span data-ttu-id="16254-114">String</span><span class="sxs-lookup"><span data-stu-id="16254-114">String</span></span>|<span data-ttu-id="16254-115">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="16254-115">Old value.</span></span>|
|<span data-ttu-id="16254-116">newValue</span><span class="sxs-lookup"><span data-stu-id="16254-116">newValue</span></span>|<span data-ttu-id="16254-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16254-117">String</span></span>|<span data-ttu-id="16254-118">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="16254-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16254-119">Relações</span><span class="sxs-lookup"><span data-stu-id="16254-119">Relationships</span></span>
<span data-ttu-id="16254-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="16254-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16254-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16254-121">JSON Representation</span></span>
<span data-ttu-id="16254-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16254-122">Here is a JSON representation of the resource.</span></span>
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



