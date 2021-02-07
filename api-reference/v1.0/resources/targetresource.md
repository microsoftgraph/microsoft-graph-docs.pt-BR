---
title: Tipo de recurso targetResource
description: Representa os tipos de recursos de destino associados à atividade de auditoria.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 66470d9e29bad5c662bfa6aa3227091b2ec739bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130147"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="ba8a1-103">Tipo de recurso targetResource</span><span class="sxs-lookup"><span data-stu-id="ba8a1-103">targetResource resource type</span></span>

<span data-ttu-id="ba8a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba8a1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba8a1-105">Representa os tipos de recursos de destino associados à atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="ba8a1-105">Represents target resource types associated with audit activity.</span></span> 

## <a name="properties"></a><span data-ttu-id="ba8a1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba8a1-106">Properties</span></span>

| <span data-ttu-id="ba8a1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba8a1-107">Property</span></span>     | <span data-ttu-id="ba8a1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba8a1-108">Type</span></span>   |<span data-ttu-id="ba8a1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba8a1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba8a1-110">id</span><span class="sxs-lookup"><span data-stu-id="ba8a1-110">id</span></span>|<span data-ttu-id="ba8a1-111">String</span><span class="sxs-lookup"><span data-stu-id="ba8a1-111">String</span></span>|<span data-ttu-id="ba8a1-112">Indica a ID exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba8a1-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="ba8a1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ba8a1-113">displayName</span></span>|<span data-ttu-id="ba8a1-114">String</span><span class="sxs-lookup"><span data-stu-id="ba8a1-114">String</span></span>|<span data-ttu-id="ba8a1-115">Indica o nome visível definido para o recurso.</span><span class="sxs-lookup"><span data-stu-id="ba8a1-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="ba8a1-116">Normalmente especificado quando o recurso é criado.</span><span class="sxs-lookup"><span data-stu-id="ba8a1-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="ba8a1-117">type</span><span class="sxs-lookup"><span data-stu-id="ba8a1-117">type</span></span>|<span data-ttu-id="ba8a1-118">String</span><span class="sxs-lookup"><span data-stu-id="ba8a1-118">String</span></span>|<span data-ttu-id="ba8a1-119">Descreve o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="ba8a1-119">Describes the resource type.</span></span>  <span data-ttu-id="ba8a1-120">Os valores de `Application` exemplo `Group` incluem , `ServicePrincipal` e `User` .</span><span class="sxs-lookup"><span data-stu-id="ba8a1-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="ba8a1-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ba8a1-121">userPrincipalName</span></span>|<span data-ttu-id="ba8a1-122">String</span><span class="sxs-lookup"><span data-stu-id="ba8a1-122">String</span></span>|<span data-ttu-id="ba8a1-123">Quando **o** tipo é definido `User` como , isso inclui o nome de usuário que iniciou a ação; `null` para outros tipos.</span><span class="sxs-lookup"><span data-stu-id="ba8a1-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="ba8a1-124">groupType</span><span class="sxs-lookup"><span data-stu-id="ba8a1-124">groupType</span></span>|<span data-ttu-id="ba8a1-125">String</span><span class="sxs-lookup"><span data-stu-id="ba8a1-125">String</span></span>|<span data-ttu-id="ba8a1-126">Quando **o** tipo é definido `Group` como , isso indica o tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="ba8a1-126">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="ba8a1-127">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="ba8a1-127">modifiedProperties</span></span>|<span data-ttu-id="ba8a1-128">[Coleção modifiedProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ba8a1-128">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="ba8a1-129">Indica o nome, o valor antigo e o novo valor de cada atributo que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="ba8a1-129">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="ba8a1-130">Os valores de propriedade dependem do tipo de **operação.**</span><span class="sxs-lookup"><span data-stu-id="ba8a1-130">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba8a1-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba8a1-131">JSON representation</span></span>

<span data-ttu-id="ba8a1-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba8a1-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

