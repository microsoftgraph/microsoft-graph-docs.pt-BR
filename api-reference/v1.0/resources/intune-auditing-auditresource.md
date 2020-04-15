---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 35d4385ca16569e1b7e0177995c32ae22e5a0aa0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439484"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="eb7d1-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="eb7d1-103">auditResource resource type</span></span>

<span data-ttu-id="eb7d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb7d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb7d1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb7d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb7d1-106">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="eb7d1-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="eb7d1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb7d1-107">Properties</span></span>
|<span data-ttu-id="eb7d1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb7d1-108">Property</span></span>|<span data-ttu-id="eb7d1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb7d1-109">Type</span></span>|<span data-ttu-id="eb7d1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb7d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb7d1-111">displayName</span><span class="sxs-lookup"><span data-stu-id="eb7d1-111">displayName</span></span>|<span data-ttu-id="eb7d1-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb7d1-112">String</span></span>|<span data-ttu-id="eb7d1-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="eb7d1-113">Display name.</span></span>|
|<span data-ttu-id="eb7d1-114">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="eb7d1-114">modifiedProperties</span></span>|<span data-ttu-id="eb7d1-115">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="eb7d1-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="eb7d1-116">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="eb7d1-116">List of modified properties.</span></span>|
|<span data-ttu-id="eb7d1-117">type</span><span class="sxs-lookup"><span data-stu-id="eb7d1-117">type</span></span>|<span data-ttu-id="eb7d1-118">String</span><span class="sxs-lookup"><span data-stu-id="eb7d1-118">String</span></span>|<span data-ttu-id="eb7d1-119">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="eb7d1-119">Audit resource's type.</span></span>|
|<span data-ttu-id="eb7d1-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="eb7d1-120">resourceId</span></span>|<span data-ttu-id="eb7d1-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb7d1-121">String</span></span>|<span data-ttu-id="eb7d1-122">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="eb7d1-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb7d1-123">Relações</span><span class="sxs-lookup"><span data-stu-id="eb7d1-123">Relationships</span></span>
<span data-ttu-id="eb7d1-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb7d1-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb7d1-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb7d1-125">JSON Representation</span></span>
<span data-ttu-id="eb7d1-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb7d1-126">Here is a JSON representation of the resource.</span></span>
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







