---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a390f43daca9d86320eea29eb139406ad52476fe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335218"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="e8c14-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="e8c14-103">auditResource resource type</span></span>

> <span data-ttu-id="e8c14-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8c14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8c14-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8c14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8c14-106">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="e8c14-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="e8c14-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8c14-107">Properties</span></span>
|<span data-ttu-id="e8c14-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8c14-108">Property</span></span>|<span data-ttu-id="e8c14-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8c14-109">Type</span></span>|<span data-ttu-id="e8c14-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8c14-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8c14-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e8c14-111">displayName</span></span>|<span data-ttu-id="e8c14-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8c14-112">String</span></span>|<span data-ttu-id="e8c14-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="e8c14-113">Display name.</span></span>|
|<span data-ttu-id="e8c14-114">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="e8c14-114">modifiedProperties</span></span>|<span data-ttu-id="e8c14-115">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="e8c14-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="e8c14-116">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="e8c14-116">List of modified properties.</span></span>|
|<span data-ttu-id="e8c14-117">type</span><span class="sxs-lookup"><span data-stu-id="e8c14-117">type</span></span>|<span data-ttu-id="e8c14-118">String</span><span class="sxs-lookup"><span data-stu-id="e8c14-118">String</span></span>|<span data-ttu-id="e8c14-119">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="e8c14-119">Audit resource's type.</span></span>|
|<span data-ttu-id="e8c14-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="e8c14-120">resourceId</span></span>|<span data-ttu-id="e8c14-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8c14-121">String</span></span>|<span data-ttu-id="e8c14-122">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="e8c14-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8c14-123">Relações</span><span class="sxs-lookup"><span data-stu-id="e8c14-123">Relationships</span></span>
<span data-ttu-id="e8c14-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8c14-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8c14-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8c14-125">JSON Representation</span></span>
<span data-ttu-id="e8c14-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8c14-126">Here is a JSON representation of the resource.</span></span>
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



