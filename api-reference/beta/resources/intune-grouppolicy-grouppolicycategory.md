---
title: tipo de recurso groupPolicyCategory
description: A entidade de categoria armazena a categoria de uma definição de política de grupo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b754020cc4a7c4f7e9fdf7cc35f74d9dcc4c4c1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783120"
---
# <a name="grouppolicycategory-resource-type"></a><span data-ttu-id="6029b-103">tipo de recurso groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="6029b-103">groupPolicyCategory resource type</span></span>

> <span data-ttu-id="6029b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6029b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6029b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6029b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6029b-106">A entidade de categoria armazena a categoria de uma definição de política de grupo</span><span class="sxs-lookup"><span data-stu-id="6029b-106">The category entity stores the category of a group policy definition</span></span>

## <a name="methods"></a><span data-ttu-id="6029b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6029b-107">Methods</span></span>
|<span data-ttu-id="6029b-108">Método</span><span class="sxs-lookup"><span data-stu-id="6029b-108">Method</span></span>|<span data-ttu-id="6029b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6029b-109">Return Type</span></span>|<span data-ttu-id="6029b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6029b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6029b-111">Obter groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="6029b-111">Get groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-get.md)|[<span data-ttu-id="6029b-112">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="6029b-112">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="6029b-113">Leia as propriedades e as relações do objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="6029b-113">Read properties and relationships of the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|
|[<span data-ttu-id="6029b-114">Atualizar groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="6029b-114">Update groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-update.md)|[<span data-ttu-id="6029b-115">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="6029b-115">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="6029b-116">Atualiza as propriedades de um objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="6029b-116">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6029b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6029b-117">Properties</span></span>
|<span data-ttu-id="6029b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6029b-118">Property</span></span>|<span data-ttu-id="6029b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6029b-119">Type</span></span>|<span data-ttu-id="6029b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6029b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6029b-121">displayName</span><span class="sxs-lookup"><span data-stu-id="6029b-121">displayName</span></span>|<span data-ttu-id="6029b-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6029b-122">String</span></span>|<span data-ttu-id="6029b-123">A ID da cadeia de caracteres do nome de exibição da categoria</span><span class="sxs-lookup"><span data-stu-id="6029b-123">The string id of the category's display name</span></span>|
|<span data-ttu-id="6029b-124">IsRoot</span><span class="sxs-lookup"><span data-stu-id="6029b-124">isRoot</span></span>|<span data-ttu-id="6029b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="6029b-125">Boolean</span></span>|<span data-ttu-id="6029b-126">Define se a categoria é uma categoria raiz</span><span class="sxs-lookup"><span data-stu-id="6029b-126">Defines if the category is a root category</span></span>|
|<span data-ttu-id="6029b-127">id</span><span class="sxs-lookup"><span data-stu-id="6029b-127">id</span></span>|<span data-ttu-id="6029b-128">String</span><span class="sxs-lookup"><span data-stu-id="6029b-128">String</span></span>|<span data-ttu-id="6029b-129">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6029b-129">Key of the entity.</span></span>|
|<span data-ttu-id="6029b-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6029b-130">lastModifiedDateTime</span></span>|<span data-ttu-id="6029b-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6029b-131">DateTimeOffset</span></span>|<span data-ttu-id="6029b-132">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6029b-132">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6029b-133">Relações</span><span class="sxs-lookup"><span data-stu-id="6029b-133">Relationships</span></span>
|<span data-ttu-id="6029b-134">Relação</span><span class="sxs-lookup"><span data-stu-id="6029b-134">Relationship</span></span>|<span data-ttu-id="6029b-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="6029b-135">Type</span></span>|<span data-ttu-id="6029b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="6029b-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6029b-137">primário</span><span class="sxs-lookup"><span data-stu-id="6029b-137">parent</span></span>|[<span data-ttu-id="6029b-138">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="6029b-138">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="6029b-139">A categoria pai</span><span class="sxs-lookup"><span data-stu-id="6029b-139">The parent category</span></span>|
|<span data-ttu-id="6029b-140">children</span><span class="sxs-lookup"><span data-stu-id="6029b-140">children</span></span>|<span data-ttu-id="6029b-141">coleção [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="6029b-141">[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) collection</span></span>|<span data-ttu-id="6029b-142">As categorias filhas</span><span class="sxs-lookup"><span data-stu-id="6029b-142">The children categories</span></span>|
|<span data-ttu-id="6029b-143">Definição</span><span class="sxs-lookup"><span data-stu-id="6029b-143">definitions</span></span>|<span data-ttu-id="6029b-144">coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6029b-144">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="6029b-145">Os filhos GroupPolicyDefinition imediatos da categoria</span><span class="sxs-lookup"><span data-stu-id="6029b-145">The immediate GroupPolicyDefinition children of the category</span></span>|
|<span data-ttu-id="6029b-146">DefinitionFile</span><span class="sxs-lookup"><span data-stu-id="6029b-146">definitionFile</span></span>|[<span data-ttu-id="6029b-147">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="6029b-147">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="6029b-148">A ID do arquivo de definição do qual a categoria provém</span><span class="sxs-lookup"><span data-stu-id="6029b-148">The id of the definition file the category came from</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6029b-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6029b-149">JSON Representation</span></span>
<span data-ttu-id="6029b-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6029b-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "String",
  "isRoot": true,
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



