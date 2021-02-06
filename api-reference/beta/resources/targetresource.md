---
title: Tipo complexo de recurso targetResource - API do Microsoft Graph
description: Define o tipo complexo de recurso da entidade targetResource da API do Microsoft Graph que oferece suporte à atividade da organização de relatório de log de auditoria (locatário).
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: 2dc8adea2edf11674d844cee4e5548da96882f7d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137582"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="f1672-103">Tipo de recurso targetResource</span><span class="sxs-lookup"><span data-stu-id="f1672-103">targetResource resource type</span></span>

<span data-ttu-id="f1672-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1672-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1672-105">Representa os tipos de recursos de destino associados à atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f1672-105">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="f1672-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1672-106">Properties</span></span>

| <span data-ttu-id="f1672-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1672-107">Property</span></span>     | <span data-ttu-id="f1672-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1672-108">Type</span></span>   |<span data-ttu-id="f1672-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1672-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1672-110">id</span><span class="sxs-lookup"><span data-stu-id="f1672-110">id</span></span>|<span data-ttu-id="f1672-111">String</span><span class="sxs-lookup"><span data-stu-id="f1672-111">String</span></span>|<span data-ttu-id="f1672-112">Indica a ID exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1672-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="f1672-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f1672-113">displayName</span></span>|<span data-ttu-id="f1672-114">String</span><span class="sxs-lookup"><span data-stu-id="f1672-114">String</span></span>|<span data-ttu-id="f1672-115">Indica o nome visível definido para o recurso.</span><span class="sxs-lookup"><span data-stu-id="f1672-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="f1672-116">Normalmente especificado quando o recurso é criado.</span><span class="sxs-lookup"><span data-stu-id="f1672-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="f1672-117">type</span><span class="sxs-lookup"><span data-stu-id="f1672-117">type</span></span>|<span data-ttu-id="f1672-118">String</span><span class="sxs-lookup"><span data-stu-id="f1672-118">String</span></span>|<span data-ttu-id="f1672-119">Descreve o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="f1672-119">Describes the resource type.</span></span>  <span data-ttu-id="f1672-120">Os valores de `Application` exemplo `Group` incluem , `ServicePrincipal` e `User` .</span><span class="sxs-lookup"><span data-stu-id="f1672-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="f1672-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1672-121">userPrincipalName</span></span>|<span data-ttu-id="f1672-122">String</span><span class="sxs-lookup"><span data-stu-id="f1672-122">String</span></span>|<span data-ttu-id="f1672-123">Quando **o** tipo é definido `User` como , isso inclui o nome de usuário que iniciou a ação; `null` para outros tipos.</span><span class="sxs-lookup"><span data-stu-id="f1672-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="f1672-124">groupType</span><span class="sxs-lookup"><span data-stu-id="f1672-124">groupType</span></span>|<span data-ttu-id="f1672-125">String</span><span class="sxs-lookup"><span data-stu-id="f1672-125">String</span></span>|<span data-ttu-id="f1672-126">Quando **o** tipo é definido `Group` como , isso indica o tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="f1672-126">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="f1672-127">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="f1672-127">modifiedProperties</span></span>|<span data-ttu-id="f1672-128">[Coleção modifiedProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f1672-128">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="f1672-129">Indica o nome, o valor antigo e o novo valor de cada atributo que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="f1672-129">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="f1672-130">Os valores de propriedade dependem do tipo de **operação.**</span><span class="sxs-lookup"><span data-stu-id="f1672-130">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1672-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1672-131">JSON representation</span></span>

<span data-ttu-id="f1672-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1672-132">Here is a JSON representation of the resource.</span></span>

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


