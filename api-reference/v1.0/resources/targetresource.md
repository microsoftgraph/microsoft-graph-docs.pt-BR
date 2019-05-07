---
title: tipo de recurso targetResource
description: Representa os tipos de recursos de destino associados à atividade de auditoria.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
ms.openlocfilehash: 33a381d6088245be235f37549184183443fe3237
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629212"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="dbef0-103">tipo de recurso targetResource</span><span class="sxs-lookup"><span data-stu-id="dbef0-103">targetResource resource type</span></span>

<span data-ttu-id="dbef0-104">Representa os tipos de recursos de destino associados à atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="dbef0-104">Represents target resource types associated with audit activity.</span></span> 

## <a name="properties"></a><span data-ttu-id="dbef0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbef0-105">Properties</span></span>

| <span data-ttu-id="dbef0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbef0-106">Property</span></span>     | <span data-ttu-id="dbef0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbef0-107">Type</span></span>   |<span data-ttu-id="dbef0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbef0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbef0-109">id</span><span class="sxs-lookup"><span data-stu-id="dbef0-109">id</span></span>|<span data-ttu-id="dbef0-110">String</span><span class="sxs-lookup"><span data-stu-id="dbef0-110">String</span></span>|<span data-ttu-id="dbef0-111">Indica a ID exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbef0-111">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="dbef0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="dbef0-112">displayName</span></span>|<span data-ttu-id="dbef0-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbef0-113">String</span></span>|<span data-ttu-id="dbef0-114">Indica o nome visível definido para o recurso.</span><span class="sxs-lookup"><span data-stu-id="dbef0-114">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="dbef0-115">Normalmente especificado quando o recurso é criado.</span><span class="sxs-lookup"><span data-stu-id="dbef0-115">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="dbef0-116">type</span><span class="sxs-lookup"><span data-stu-id="dbef0-116">type</span></span>|<span data-ttu-id="dbef0-117">String</span><span class="sxs-lookup"><span data-stu-id="dbef0-117">String</span></span>|<span data-ttu-id="dbef0-118">Descreve o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="dbef0-118">Describes the resource type.</span></span>  <span data-ttu-id="dbef0-119">Os valores de `Application`exemplo `Group`incluem `ServicePrincipal`,, `User`e.</span><span class="sxs-lookup"><span data-stu-id="dbef0-119">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="dbef0-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dbef0-120">userPrincipalName</span></span>|<span data-ttu-id="dbef0-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbef0-121">String</span></span>|<span data-ttu-id="dbef0-122">Quando o **tipo** está definido `User`como, isso inclui o nome de usuário que iniciou a ação; `null` para outros tipos.</span><span class="sxs-lookup"><span data-stu-id="dbef0-122">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="dbef0-123">groupType</span><span class="sxs-lookup"><span data-stu-id="dbef0-123">groupType</span></span>|<span data-ttu-id="dbef0-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbef0-124">String</span></span>|<span data-ttu-id="dbef0-125">Quando **Type** é definido como `Group`, isso indica o tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="dbef0-125">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="dbef0-126">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="dbef0-126">modifiedProperties</span></span>|<span data-ttu-id="dbef0-127">[](modifiedproperty.md) coleção modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="dbef0-127">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="dbef0-128">Indica o nome, o valor antigo e o novo valor de cada atributo que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="dbef0-128">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="dbef0-129">Os valores de propriedade dependem do **tipo**de operação.</span><span class="sxs-lookup"><span data-stu-id="dbef0-129">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbef0-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbef0-130">JSON representation</span></span>

<span data-ttu-id="dbef0-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbef0-131">Here is a JSON representation of the resource.</span></span>

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
