---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 14ecd6e4772e6d694707bd047899bd6b75720252
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028858"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="90656-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="90656-103">auditResource resource type</span></span>

> <span data-ttu-id="90656-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90656-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90656-105">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="90656-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="90656-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90656-106">Properties</span></span>
|<span data-ttu-id="90656-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90656-107">Property</span></span>|<span data-ttu-id="90656-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="90656-108">Type</span></span>|<span data-ttu-id="90656-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="90656-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90656-110">displayName</span><span class="sxs-lookup"><span data-stu-id="90656-110">displayName</span></span>|<span data-ttu-id="90656-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90656-111">String</span></span>|<span data-ttu-id="90656-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="90656-112">Display name.</span></span>|
|<span data-ttu-id="90656-113">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="90656-113">modifiedProperties</span></span>|<span data-ttu-id="90656-114">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="90656-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="90656-115">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="90656-115">List of modified properties.</span></span>|
|<span data-ttu-id="90656-116">type</span><span class="sxs-lookup"><span data-stu-id="90656-116">type</span></span>|<span data-ttu-id="90656-117">String</span><span class="sxs-lookup"><span data-stu-id="90656-117">String</span></span>|<span data-ttu-id="90656-118">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="90656-118">Audit resource's type.</span></span>|
|<span data-ttu-id="90656-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="90656-119">resourceId</span></span>|<span data-ttu-id="90656-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90656-120">String</span></span>|<span data-ttu-id="90656-121">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="90656-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90656-122">Relações</span><span class="sxs-lookup"><span data-stu-id="90656-122">Relationships</span></span>
<span data-ttu-id="90656-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90656-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90656-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90656-124">JSON Representation</span></span>
<span data-ttu-id="90656-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90656-125">Here is a JSON representation of the resource.</span></span>
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



