---
title: tipo de recurso targetResource
description: Representa os tipos de recursos de destino associados à atividade de auditoria.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 641097b6e8b4646d878182ba1763fd62ab75b080
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094054"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="1a987-103">tipo de recurso targetResource</span><span class="sxs-lookup"><span data-stu-id="1a987-103">targetResource resource type</span></span>

<span data-ttu-id="1a987-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a987-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a987-105">Representa os tipos de recursos de destino associados à atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="1a987-105">Represents target resource types associated with audit activity.</span></span> 

## <a name="properties"></a><span data-ttu-id="1a987-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a987-106">Properties</span></span>

| <span data-ttu-id="1a987-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a987-107">Property</span></span>     | <span data-ttu-id="1a987-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a987-108">Type</span></span>   |<span data-ttu-id="1a987-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a987-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a987-110">id</span><span class="sxs-lookup"><span data-stu-id="1a987-110">id</span></span>|<span data-ttu-id="1a987-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a987-111">String</span></span>|<span data-ttu-id="1a987-112">Indica a ID exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a987-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="1a987-113">displayName</span><span class="sxs-lookup"><span data-stu-id="1a987-113">displayName</span></span>|<span data-ttu-id="1a987-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a987-114">String</span></span>|<span data-ttu-id="1a987-115">Indica o nome visível definido para o recurso.</span><span class="sxs-lookup"><span data-stu-id="1a987-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="1a987-116">Normalmente especificado quando o recurso é criado.</span><span class="sxs-lookup"><span data-stu-id="1a987-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="1a987-117">type</span><span class="sxs-lookup"><span data-stu-id="1a987-117">type</span></span>|<span data-ttu-id="1a987-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a987-118">String</span></span>|<span data-ttu-id="1a987-119">Descreve o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="1a987-119">Describes the resource type.</span></span>  <span data-ttu-id="1a987-120">Os valores de exemplo incluem `Application` ,, `Group` `ServicePrincipal` e `User` .</span><span class="sxs-lookup"><span data-stu-id="1a987-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="1a987-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1a987-121">userPrincipalName</span></span>|<span data-ttu-id="1a987-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a987-122">String</span></span>|<span data-ttu-id="1a987-123">Quando **Type** está definido como `User` , isso inclui o nome de usuário que iniciou a ação; `null` para outros tipos.</span><span class="sxs-lookup"><span data-stu-id="1a987-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="1a987-124">groupType</span><span class="sxs-lookup"><span data-stu-id="1a987-124">groupType</span></span>|<span data-ttu-id="1a987-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a987-125">String</span></span>|<span data-ttu-id="1a987-126">Quando **Type** é definido como `Group` , isso indica o tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="1a987-126">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="1a987-127">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="1a987-127">modifiedProperties</span></span>|<span data-ttu-id="1a987-128">coleção [modifiedproperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="1a987-128">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="1a987-129">Indica o nome, o valor antigo e o novo valor de cada atributo que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="1a987-129">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="1a987-130">Os valores de propriedade dependem do **tipo**de operação.</span><span class="sxs-lookup"><span data-stu-id="1a987-130">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a987-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a987-131">JSON representation</span></span>

<span data-ttu-id="1a987-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a987-132">Here is a JSON representation of the resource.</span></span>

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

