---
title: tipo de recurso groupPolicyCategory
description: A entidade de categoria armazena a categoria de uma definição de política de grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 905489909e57d45b26df5bb0a23044ad1778a5dd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697438"
---
# <a name="grouppolicycategory-resource-type"></a><span data-ttu-id="3cc6d-103">tipo de recurso groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="3cc6d-103">groupPolicyCategory resource type</span></span>

<span data-ttu-id="3cc6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cc6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cc6d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3cc6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cc6d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3cc6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cc6d-107">A entidade de categoria armazena a categoria de uma definição de política de grupo</span><span class="sxs-lookup"><span data-stu-id="3cc6d-107">The category entity stores the category of a group policy definition</span></span>

## <a name="methods"></a><span data-ttu-id="3cc6d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3cc6d-108">Methods</span></span>
|<span data-ttu-id="3cc6d-109">Método</span><span class="sxs-lookup"><span data-stu-id="3cc6d-109">Method</span></span>|<span data-ttu-id="3cc6d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3cc6d-110">Return Type</span></span>|<span data-ttu-id="3cc6d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cc6d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3cc6d-112">Obter groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="3cc6d-112">Get groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-get.md)|[<span data-ttu-id="3cc6d-113">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="3cc6d-113">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="3cc6d-114">Leia as propriedades e as relações do objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="3cc6d-114">Read properties and relationships of the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|
|[<span data-ttu-id="3cc6d-115">Atualizar groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="3cc6d-115">Update groupPolicyCategory</span></span>](../api/intune-grouppolicy-grouppolicycategory-update.md)|[<span data-ttu-id="3cc6d-116">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="3cc6d-116">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="3cc6d-117">Atualiza as propriedades de um objeto [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="3cc6d-117">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3cc6d-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3cc6d-118">Properties</span></span>
|<span data-ttu-id="3cc6d-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cc6d-119">Property</span></span>|<span data-ttu-id="3cc6d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cc6d-120">Type</span></span>|<span data-ttu-id="3cc6d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cc6d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cc6d-122">displayName</span><span class="sxs-lookup"><span data-stu-id="3cc6d-122">displayName</span></span>|<span data-ttu-id="3cc6d-123">String</span><span class="sxs-lookup"><span data-stu-id="3cc6d-123">String</span></span>|<span data-ttu-id="3cc6d-124">A ID da cadeia de caracteres do nome de exibição da categoria</span><span class="sxs-lookup"><span data-stu-id="3cc6d-124">The string id of the category's display name</span></span>|
|<span data-ttu-id="3cc6d-125">IsRoot</span><span class="sxs-lookup"><span data-stu-id="3cc6d-125">isRoot</span></span>|<span data-ttu-id="3cc6d-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cc6d-126">Boolean</span></span>|<span data-ttu-id="3cc6d-127">Define se a categoria é uma categoria raiz</span><span class="sxs-lookup"><span data-stu-id="3cc6d-127">Defines if the category is a root category</span></span>|
|<span data-ttu-id="3cc6d-128">id</span><span class="sxs-lookup"><span data-stu-id="3cc6d-128">id</span></span>|<span data-ttu-id="3cc6d-129">String</span><span class="sxs-lookup"><span data-stu-id="3cc6d-129">String</span></span>|<span data-ttu-id="3cc6d-130">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3cc6d-130">Key of the entity.</span></span>|
|<span data-ttu-id="3cc6d-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cc6d-131">lastModifiedDateTime</span></span>|<span data-ttu-id="3cc6d-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cc6d-132">DateTimeOffset</span></span>|<span data-ttu-id="3cc6d-133">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3cc6d-133">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cc6d-134">Relações</span><span class="sxs-lookup"><span data-stu-id="3cc6d-134">Relationships</span></span>
|<span data-ttu-id="3cc6d-135">Relação</span><span class="sxs-lookup"><span data-stu-id="3cc6d-135">Relationship</span></span>|<span data-ttu-id="3cc6d-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cc6d-136">Type</span></span>|<span data-ttu-id="3cc6d-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cc6d-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cc6d-138">primário</span><span class="sxs-lookup"><span data-stu-id="3cc6d-138">parent</span></span>|[<span data-ttu-id="3cc6d-139">groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="3cc6d-139">groupPolicyCategory</span></span>](../resources/intune-grouppolicy-grouppolicycategory.md)|<span data-ttu-id="3cc6d-140">A categoria pai</span><span class="sxs-lookup"><span data-stu-id="3cc6d-140">The parent category</span></span>|
|<span data-ttu-id="3cc6d-141">children</span><span class="sxs-lookup"><span data-stu-id="3cc6d-141">children</span></span>|<span data-ttu-id="3cc6d-142">coleção [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="3cc6d-142">[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) collection</span></span>|<span data-ttu-id="3cc6d-143">As categorias filhas</span><span class="sxs-lookup"><span data-stu-id="3cc6d-143">The children categories</span></span>|
|<span data-ttu-id="3cc6d-144">Definição</span><span class="sxs-lookup"><span data-stu-id="3cc6d-144">definitions</span></span>|<span data-ttu-id="3cc6d-145">coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3cc6d-145">[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) collection</span></span>|<span data-ttu-id="3cc6d-146">Os filhos GroupPolicyDefinition imediatos da categoria</span><span class="sxs-lookup"><span data-stu-id="3cc6d-146">The immediate GroupPolicyDefinition children of the category</span></span>|
|<span data-ttu-id="3cc6d-147">DefinitionFile</span><span class="sxs-lookup"><span data-stu-id="3cc6d-147">definitionFile</span></span>|[<span data-ttu-id="3cc6d-148">groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="3cc6d-148">groupPolicyDefinitionFile</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|<span data-ttu-id="3cc6d-149">A ID do arquivo de definição do qual a categoria provém</span><span class="sxs-lookup"><span data-stu-id="3cc6d-149">The id of the definition file the category came from</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cc6d-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3cc6d-150">JSON Representation</span></span>
<span data-ttu-id="3cc6d-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3cc6d-151">Here is a JSON representation of the resource.</span></span>
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





