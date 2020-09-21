---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 895f88bf20219447e9f9609271b731b941263798
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965677"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="07851-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="07851-103">auditResource resource type</span></span>

<span data-ttu-id="07851-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07851-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07851-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07851-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07851-106">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="07851-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="07851-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07851-107">Properties</span></span>
|<span data-ttu-id="07851-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07851-108">Property</span></span>|<span data-ttu-id="07851-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="07851-109">Type</span></span>|<span data-ttu-id="07851-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07851-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07851-111">displayName</span><span class="sxs-lookup"><span data-stu-id="07851-111">displayName</span></span>|<span data-ttu-id="07851-112">String</span><span class="sxs-lookup"><span data-stu-id="07851-112">String</span></span>|<span data-ttu-id="07851-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="07851-113">Display name.</span></span>|
|<span data-ttu-id="07851-114">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="07851-114">modifiedProperties</span></span>|<span data-ttu-id="07851-115">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="07851-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="07851-116">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="07851-116">List of modified properties.</span></span>|
|<span data-ttu-id="07851-117">tipo</span><span class="sxs-lookup"><span data-stu-id="07851-117">type</span></span>|<span data-ttu-id="07851-118">String</span><span class="sxs-lookup"><span data-stu-id="07851-118">String</span></span>|<span data-ttu-id="07851-119">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="07851-119">Audit resource's type.</span></span>|
|<span data-ttu-id="07851-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="07851-120">resourceId</span></span>|<span data-ttu-id="07851-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07851-121">String</span></span>|<span data-ttu-id="07851-122">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="07851-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07851-123">Relações</span><span class="sxs-lookup"><span data-stu-id="07851-123">Relationships</span></span>
<span data-ttu-id="07851-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07851-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07851-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07851-125">JSON Representation</span></span>
<span data-ttu-id="07851-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07851-126">Here is a JSON representation of the resource.</span></span>
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









