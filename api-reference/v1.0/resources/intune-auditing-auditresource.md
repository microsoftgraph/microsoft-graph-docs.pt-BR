---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa30fcb276661e3a673c1942c4d35cc71ca41e6b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759443"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="a962f-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="a962f-103">auditResource resource type</span></span>

<span data-ttu-id="a962f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a962f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a962f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a962f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a962f-106">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a962f-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a962f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a962f-107">Properties</span></span>
|<span data-ttu-id="a962f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a962f-108">Property</span></span>|<span data-ttu-id="a962f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a962f-109">Type</span></span>|<span data-ttu-id="a962f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a962f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a962f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a962f-111">displayName</span></span>|<span data-ttu-id="a962f-112">String</span><span class="sxs-lookup"><span data-stu-id="a962f-112">String</span></span>|<span data-ttu-id="a962f-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="a962f-113">Display name.</span></span>|
|<span data-ttu-id="a962f-114">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="a962f-114">modifiedProperties</span></span>|<span data-ttu-id="a962f-115">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="a962f-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="a962f-116">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="a962f-116">List of modified properties.</span></span>|
|<span data-ttu-id="a962f-117">tipo</span><span class="sxs-lookup"><span data-stu-id="a962f-117">type</span></span>|<span data-ttu-id="a962f-118">String</span><span class="sxs-lookup"><span data-stu-id="a962f-118">String</span></span>|<span data-ttu-id="a962f-119">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a962f-119">Audit resource's type.</span></span>|
|<span data-ttu-id="a962f-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="a962f-120">resourceId</span></span>|<span data-ttu-id="a962f-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a962f-121">String</span></span>|<span data-ttu-id="a962f-122">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a962f-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a962f-123">Relações</span><span class="sxs-lookup"><span data-stu-id="a962f-123">Relationships</span></span>
<span data-ttu-id="a962f-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a962f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a962f-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a962f-125">JSON Representation</span></span>
<span data-ttu-id="a962f-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a962f-126">Here is a JSON representation of the resource.</span></span>
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




