---
title: Tipo de recurso cloudPcAuditResource
description: Representa o recurso de auditoria.Isso mostra a entidade de recurso editada de destino, com várias propriedades editadas.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ebd61a14680c5e5f2917e273456bcce60672149e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211212"
---
# <a name="cloudpcauditresource-resource-type"></a><span data-ttu-id="78822-104">Tipo de recurso cloudPcAuditResource</span><span class="sxs-lookup"><span data-stu-id="78822-104">cloudPcAuditResource resource type</span></span>

<span data-ttu-id="78822-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78822-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78822-106">Representa o recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="78822-106">Represents the audit resource.</span></span><span data-ttu-id="78822-107">Isso mostra a entidade de recurso editada de destino, com várias propriedades editadas.</span><span class="sxs-lookup"><span data-stu-id="78822-107"> This shows the target edited resource entity, with multiple edited properties.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="78822-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78822-108">Properties</span></span>
|<span data-ttu-id="78822-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78822-109">Property</span></span>|<span data-ttu-id="78822-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="78822-110">Type</span></span>|<span data-ttu-id="78822-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="78822-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78822-112">displayName</span><span class="sxs-lookup"><span data-stu-id="78822-112">displayName</span></span>|<span data-ttu-id="78822-113">String</span><span class="sxs-lookup"><span data-stu-id="78822-113">String</span></span>|<span data-ttu-id="78822-114">O nome de exibição da entidade de recurso.</span><span class="sxs-lookup"><span data-stu-id="78822-114">The resource entity display name.</span></span>|
|<span data-ttu-id="78822-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="78822-115">modifiedProperties</span></span>|<span data-ttu-id="78822-116">[Coleção cloudPcAuditProperty](../resources/cloudpcauditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="78822-116">[cloudPcAuditProperty](../resources/cloudpcauditproperty.md) collection</span></span>|<span data-ttu-id="78822-117">Uma lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="78822-117">A list of modified properties.</span></span>|
|<span data-ttu-id="78822-118">tipo</span><span class="sxs-lookup"><span data-stu-id="78822-118">type</span></span>|<span data-ttu-id="78822-119">String</span><span class="sxs-lookup"><span data-stu-id="78822-119">String</span></span>|<span data-ttu-id="78822-120">O tipo do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="78822-120">The type of the audit resource.</span></span>|
|<span data-ttu-id="78822-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="78822-121">resourceId</span></span>|<span data-ttu-id="78822-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78822-122">String</span></span>|<span data-ttu-id="78822-123">A ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="78822-123">The ID of the audit resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78822-124">Relações</span><span class="sxs-lookup"><span data-stu-id="78822-124">Relationships</span></span>

<span data-ttu-id="78822-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78822-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78822-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78822-126">JSON Representation</span></span>

<span data-ttu-id="78822-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78822-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditResource"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```
