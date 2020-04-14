---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3aae8d82706d25ed95e238c8c4dfa07516c64771
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472094"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="2666b-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="2666b-103">auditResource resource type</span></span>

<span data-ttu-id="2666b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2666b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2666b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2666b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2666b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2666b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2666b-107">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="2666b-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="2666b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2666b-108">Properties</span></span>
|<span data-ttu-id="2666b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2666b-109">Property</span></span>|<span data-ttu-id="2666b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2666b-110">Type</span></span>|<span data-ttu-id="2666b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2666b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2666b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2666b-112">displayName</span></span>|<span data-ttu-id="2666b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2666b-113">String</span></span>|<span data-ttu-id="2666b-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="2666b-114">Display name.</span></span>|
|<span data-ttu-id="2666b-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="2666b-115">modifiedProperties</span></span>|<span data-ttu-id="2666b-116">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="2666b-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="2666b-117">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="2666b-117">List of modified properties.</span></span>|
|<span data-ttu-id="2666b-118">type</span><span class="sxs-lookup"><span data-stu-id="2666b-118">type</span></span>|<span data-ttu-id="2666b-119">String</span><span class="sxs-lookup"><span data-stu-id="2666b-119">String</span></span>|<span data-ttu-id="2666b-120">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="2666b-120">Audit resource's type.</span></span>|
|<span data-ttu-id="2666b-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="2666b-121">resourceId</span></span>|<span data-ttu-id="2666b-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2666b-122">String</span></span>|<span data-ttu-id="2666b-123">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="2666b-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2666b-124">Relações</span><span class="sxs-lookup"><span data-stu-id="2666b-124">Relationships</span></span>
<span data-ttu-id="2666b-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2666b-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2666b-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2666b-126">JSON Representation</span></span>
<span data-ttu-id="2666b-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2666b-127">Here is a JSON representation of the resource.</span></span>
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



