---
title: Tipo de recurso cloudPcAuditProperty
description: Representa a propriedade de auditoria.Isso mostra o nome da propriedade editada, o valor antigo e o novo valor.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1f73733f0ace4526d3cbae226c963887d5af37ce
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211235"
---
# <a name="cloudpcauditproperty-resource-type"></a><span data-ttu-id="ba8d9-104">Tipo de recurso cloudPcAuditProperty</span><span class="sxs-lookup"><span data-stu-id="ba8d9-104">cloudPcAuditProperty resource type</span></span>

<span data-ttu-id="ba8d9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba8d9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba8d9-106">Representa a propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="ba8d9-106">Represents the audit property.</span></span><span data-ttu-id="ba8d9-107">Isso mostra o nome da propriedade editada, o valor antigo e o novo valor.</span><span class="sxs-lookup"><span data-stu-id="ba8d9-107"> This shows the edited property name, the old value, and the new value.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="ba8d9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba8d9-108">Properties</span></span>
|<span data-ttu-id="ba8d9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba8d9-109">Property</span></span>|<span data-ttu-id="ba8d9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba8d9-110">Type</span></span>|<span data-ttu-id="ba8d9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba8d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba8d9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ba8d9-112">displayName</span></span>|<span data-ttu-id="ba8d9-113">String</span><span class="sxs-lookup"><span data-stu-id="ba8d9-113">String</span></span>|<span data-ttu-id="ba8d9-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="ba8d9-114">Display name.</span></span>|
|<span data-ttu-id="ba8d9-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="ba8d9-115">oldValue</span></span>|<span data-ttu-id="ba8d9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba8d9-116">String</span></span>|<span data-ttu-id="ba8d9-117">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="ba8d9-117">Old value.</span></span>|
|<span data-ttu-id="ba8d9-118">newValue</span><span class="sxs-lookup"><span data-stu-id="ba8d9-118">newValue</span></span>|<span data-ttu-id="ba8d9-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba8d9-119">String</span></span>|<span data-ttu-id="ba8d9-120">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="ba8d9-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba8d9-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ba8d9-121">Relationships</span></span>

<span data-ttu-id="ba8d9-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba8d9-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba8d9-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba8d9-123">JSON Representation</span></span>

<span data-ttu-id="ba8d9-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba8d9-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditProperty"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```
