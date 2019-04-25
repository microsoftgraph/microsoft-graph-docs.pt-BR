---
title: tipo complexo de recurso de targetResource-API do Microsoft Graph
description: Define o tipo complexo de recurso de entidade de targetResource da API do Microsoft Graph que oferece suporte à atividade de locatário de relatórios de log de auditoria (locatário).
author: lleonard-msft
localization_priority: Normal
ms.prod: azure-ad
ms.openlocfilehash: a03ca03e0b7105c8f07347f6ed52aa322a6fd090
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583106"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="041fa-103">tipo de recurso targetResource</span><span class="sxs-lookup"><span data-stu-id="041fa-103">targetResource resource type</span></span>

<span data-ttu-id="041fa-104">Representa os tipos de recursos de destino associados à atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="041fa-104">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="041fa-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="041fa-105">Properties</span></span>

| <span data-ttu-id="041fa-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="041fa-106">Property</span></span>     | <span data-ttu-id="041fa-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="041fa-107">Type</span></span>   |<span data-ttu-id="041fa-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="041fa-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="041fa-109">id</span><span class="sxs-lookup"><span data-stu-id="041fa-109">id</span></span>|<span data-ttu-id="041fa-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="041fa-110">String</span></span>|<span data-ttu-id="041fa-111">Indica a ID exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="041fa-111">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="041fa-112">displayName</span><span class="sxs-lookup"><span data-stu-id="041fa-112">displayName</span></span>|<span data-ttu-id="041fa-113">String</span><span class="sxs-lookup"><span data-stu-id="041fa-113">String</span></span>|<span data-ttu-id="041fa-114">Indica o nome visível definido para o recurso.</span><span class="sxs-lookup"><span data-stu-id="041fa-114">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="041fa-115">Normalmente especificado quando o recurso é criado.</span><span class="sxs-lookup"><span data-stu-id="041fa-115">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="041fa-116">type</span><span class="sxs-lookup"><span data-stu-id="041fa-116">type</span></span>|<span data-ttu-id="041fa-117">String</span><span class="sxs-lookup"><span data-stu-id="041fa-117">String</span></span>|<span data-ttu-id="041fa-118">Descreve o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="041fa-118">Describes the resource type.</span></span>  <span data-ttu-id="041fa-119">Os valores de `Application`exemplo `Group`incluem `ServicePrincipal`,, `User`e.</span><span class="sxs-lookup"><span data-stu-id="041fa-119">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="041fa-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="041fa-120">userPrincipalName</span></span>|<span data-ttu-id="041fa-121">String</span><span class="sxs-lookup"><span data-stu-id="041fa-121">String</span></span>|<span data-ttu-id="041fa-122">Quando o **tipo** está definido `User`como, isso inclui o nome de usuário que iniciou a ação; `null` para outros tipos.</span><span class="sxs-lookup"><span data-stu-id="041fa-122">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="041fa-123">groupType</span><span class="sxs-lookup"><span data-stu-id="041fa-123">groupType</span></span>|<span data-ttu-id="041fa-124">String</span><span class="sxs-lookup"><span data-stu-id="041fa-124">String</span></span>|<span data-ttu-id="041fa-125">Quando **Type** é definido como `Group`, isso indica o tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="041fa-125">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="041fa-126">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="041fa-126">modifiedProperties</span></span>|<span data-ttu-id="041fa-127">[](modifiedproperty.md) coleção modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="041fa-127">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="041fa-128">Indica o nome, o valor antigo e o novo valor de cada atributo que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="041fa-128">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="041fa-129">Os valores de propriedade dependem do **tipo**de operação.</span><span class="sxs-lookup"><span data-stu-id="041fa-129">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="041fa-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="041fa-130">JSON representation</span></span>

<span data-ttu-id="041fa-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="041fa-131">Here is a JSON representation of the resource.</span></span>

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
