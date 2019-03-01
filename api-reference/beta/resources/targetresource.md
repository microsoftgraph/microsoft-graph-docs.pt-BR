---
title: tipo complexo de recurso de targetResource-API do Microsoft Graph
description: Define o tipo complexo de recurso de entidade de targetResource da API do Microsoft Graph que oferece suporte à atividade de locatário de relatórios de log de auditoria (locatário).
author: lleonard-msft
localization_priority: Normal
ms.prod: azure-ad
ms.openlocfilehash: a03ca03e0b7105c8f07347f6ed52aa322a6fd090
ms.sourcegitcommit: e8b488f8068845522b869bf97475da7b078bee3d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/01/2019
ms.locfileid: "30342286"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="37160-103">tipo de recurso targetResource</span><span class="sxs-lookup"><span data-stu-id="37160-103">targetResource resource type</span></span>

<span data-ttu-id="37160-104">Representa os tipos de recursos de destino associados à atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="37160-104">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="37160-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37160-105">Properties</span></span>

| <span data-ttu-id="37160-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37160-106">Property</span></span>     | <span data-ttu-id="37160-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="37160-107">Type</span></span>   |<span data-ttu-id="37160-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="37160-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37160-109">id</span><span class="sxs-lookup"><span data-stu-id="37160-109">id</span></span>|<span data-ttu-id="37160-110">String</span><span class="sxs-lookup"><span data-stu-id="37160-110">String</span></span>|<span data-ttu-id="37160-111">Indica a ID exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="37160-111">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="37160-112">displayName</span><span class="sxs-lookup"><span data-stu-id="37160-112">displayName</span></span>|<span data-ttu-id="37160-113">String</span><span class="sxs-lookup"><span data-stu-id="37160-113">String</span></span>|<span data-ttu-id="37160-114">Indica o nome visível definido para o recurso.</span><span class="sxs-lookup"><span data-stu-id="37160-114">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="37160-115">Normalmente especificado quando o recurso é criado.</span><span class="sxs-lookup"><span data-stu-id="37160-115">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="37160-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="37160-116">type</span></span>|<span data-ttu-id="37160-117">String</span><span class="sxs-lookup"><span data-stu-id="37160-117">String</span></span>|<span data-ttu-id="37160-118">Descreve o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="37160-118">Describes the resource type.</span></span>  <span data-ttu-id="37160-119">Os valores de `Application`exemplo `Group`incluem `ServicePrincipal`,, `User`e.</span><span class="sxs-lookup"><span data-stu-id="37160-119">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="37160-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="37160-120">userPrincipalName</span></span>|<span data-ttu-id="37160-121">String</span><span class="sxs-lookup"><span data-stu-id="37160-121">String</span></span>|<span data-ttu-id="37160-122">Quando o **tipo** está definido `User`como, isso inclui o nome de usuário que iniciou a ação; `null` para outros tipos.</span><span class="sxs-lookup"><span data-stu-id="37160-122">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="37160-123">groupType</span><span class="sxs-lookup"><span data-stu-id="37160-123">groupType</span></span>|<span data-ttu-id="37160-124">String</span><span class="sxs-lookup"><span data-stu-id="37160-124">String</span></span>|<span data-ttu-id="37160-125">Quando **Type** é definido como `Group`, isso indica o tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="37160-125">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="37160-126">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="37160-126">modifiedProperties</span></span>|<span data-ttu-id="37160-127">[](modifiedproperty.md) coleção modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="37160-127">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="37160-128">Indica o nome, o valor antigo e o novo valor de cada atributo que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="37160-128">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="37160-129">Os valores de propriedade dependem do **tipo**de operação.</span><span class="sxs-lookup"><span data-stu-id="37160-129">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37160-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37160-130">JSON representation</span></span>

<span data-ttu-id="37160-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37160-131">Here is a JSON representation of the resource.</span></span>

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
