---
title: tipo complexo de recurso targetResource - API do Microsoft Graph
description: Define o tipo complexo de recurso da entidade targetResource da API do Microsoft Graph que dá suporte à atividade de organização de relatórios de log de auditoria (locatário).
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: 12030bdb5c51e41e821218e3db67c4878a90c53d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954955"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="96bf1-103">tipo de recurso targetResource</span><span class="sxs-lookup"><span data-stu-id="96bf1-103">targetResource resource type</span></span>

<span data-ttu-id="96bf1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96bf1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96bf1-105">Representa tipos de recursos de destino associados à atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="96bf1-105">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="96bf1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96bf1-106">Properties</span></span>

| <span data-ttu-id="96bf1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96bf1-107">Property</span></span>     | <span data-ttu-id="96bf1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="96bf1-108">Type</span></span>   |<span data-ttu-id="96bf1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="96bf1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96bf1-110">id</span><span class="sxs-lookup"><span data-stu-id="96bf1-110">id</span></span>|<span data-ttu-id="96bf1-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96bf1-111">String</span></span>|<span data-ttu-id="96bf1-112">Indica a ID exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="96bf1-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="96bf1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="96bf1-113">displayName</span></span>|<span data-ttu-id="96bf1-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96bf1-114">String</span></span>|<span data-ttu-id="96bf1-115">Indica o nome visível definido para o recurso.</span><span class="sxs-lookup"><span data-stu-id="96bf1-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="96bf1-116">Normalmente especificado quando o recurso é criado.</span><span class="sxs-lookup"><span data-stu-id="96bf1-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="96bf1-117">tipo</span><span class="sxs-lookup"><span data-stu-id="96bf1-117">type</span></span>|<span data-ttu-id="96bf1-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96bf1-118">String</span></span>|<span data-ttu-id="96bf1-119">Descreve o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="96bf1-119">Describes the resource type.</span></span>  <span data-ttu-id="96bf1-120">Os valores de `Application` exemplo `Group` incluem , `ServicePrincipal` , e `User` .</span><span class="sxs-lookup"><span data-stu-id="96bf1-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="96bf1-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="96bf1-121">userPrincipalName</span></span>|<span data-ttu-id="96bf1-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96bf1-122">String</span></span>|<span data-ttu-id="96bf1-123">Quando **o** tipo é definido como , isso inclui o nome de usuário que iniciou a `User` ação; para outros `null` tipos.</span><span class="sxs-lookup"><span data-stu-id="96bf1-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="96bf1-124">groupType</span><span class="sxs-lookup"><span data-stu-id="96bf1-124">groupType</span></span>|<span data-ttu-id="96bf1-125">groupType</span><span class="sxs-lookup"><span data-stu-id="96bf1-125">groupType</span></span>|<span data-ttu-id="96bf1-126">Quando **o** tipo é definido como `Group` , isso indica o tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="96bf1-126">When **type** is set to `Group`, this indicates the group type.</span></span>  <span data-ttu-id="96bf1-127">Os valores possíveis são: `unifiedGroups` `azureAD` , e `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="96bf1-127">Possible values are: `unifiedGroups`, `azureAD`, and `unknownFutureValue`</span></span>|
|<span data-ttu-id="96bf1-128">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="96bf1-128">modifiedProperties</span></span>|<span data-ttu-id="96bf1-129">[Coleção modifiedProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="96bf1-129">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="96bf1-130">Indica nome, valor antigo e novo valor de cada atributo que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="96bf1-130">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="96bf1-131">Os valores de propriedade dependem do tipo de **operação**.</span><span class="sxs-lookup"><span data-stu-id="96bf1-131">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96bf1-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96bf1-132">JSON representation</span></span>

<span data-ttu-id="96bf1-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96bf1-133">Here is a JSON representation of the resource.</span></span>

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


