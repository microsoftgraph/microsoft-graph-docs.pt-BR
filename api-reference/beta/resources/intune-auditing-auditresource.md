---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df8d9a0d255f01992d1559ae348882644c88dbcb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706055"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="9c8a1-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="9c8a1-103">auditResource resource type</span></span>

<span data-ttu-id="9c8a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c8a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c8a1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c8a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c8a1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c8a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c8a1-107">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="9c8a1-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="9c8a1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c8a1-108">Properties</span></span>
|<span data-ttu-id="9c8a1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c8a1-109">Property</span></span>|<span data-ttu-id="9c8a1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c8a1-110">Type</span></span>|<span data-ttu-id="9c8a1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c8a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c8a1-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9c8a1-112">displayName</span></span>|<span data-ttu-id="9c8a1-113">String</span><span class="sxs-lookup"><span data-stu-id="9c8a1-113">String</span></span>|<span data-ttu-id="9c8a1-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="9c8a1-114">Display name.</span></span>|
|<span data-ttu-id="9c8a1-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="9c8a1-115">modifiedProperties</span></span>|<span data-ttu-id="9c8a1-116">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="9c8a1-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="9c8a1-117">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="9c8a1-117">List of modified properties.</span></span>|
|<span data-ttu-id="9c8a1-118">type</span><span class="sxs-lookup"><span data-stu-id="9c8a1-118">type</span></span>|<span data-ttu-id="9c8a1-119">String</span><span class="sxs-lookup"><span data-stu-id="9c8a1-119">String</span></span>|<span data-ttu-id="9c8a1-120">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="9c8a1-120">Audit resource's type.</span></span>|
|<span data-ttu-id="9c8a1-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="9c8a1-121">resourceId</span></span>|<span data-ttu-id="9c8a1-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c8a1-122">String</span></span>|<span data-ttu-id="9c8a1-123">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="9c8a1-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c8a1-124">Relações</span><span class="sxs-lookup"><span data-stu-id="9c8a1-124">Relationships</span></span>
<span data-ttu-id="9c8a1-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c8a1-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c8a1-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c8a1-126">JSON Representation</span></span>
<span data-ttu-id="9c8a1-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c8a1-127">Here is a JSON representation of the resource.</span></span>
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





