---
title: tipo de recurso groupPolicyDefinitionValue
description: A entidade de valor de definição armazena o valor de uma única definição de política de grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2aa0eef1b4921d1b364486b9af254fba2a8322c0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800991"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a><span data-ttu-id="07ffe-103">tipo de recurso groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="07ffe-103">groupPolicyDefinitionValue resource type</span></span>

> <span data-ttu-id="07ffe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07ffe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07ffe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07ffe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07ffe-106">A entidade de valor de definição armazena o valor de uma única definição de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="07ffe-106">The definition value entity stores the value for a single group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="07ffe-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="07ffe-107">Methods</span></span>
|<span data-ttu-id="07ffe-108">Método</span><span class="sxs-lookup"><span data-stu-id="07ffe-108">Method</span></span>|<span data-ttu-id="07ffe-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="07ffe-109">Return Type</span></span>|<span data-ttu-id="07ffe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07ffe-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="07ffe-111">Listar groupPolicyDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="07ffe-111">List groupPolicyDefinitionValues</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|<span data-ttu-id="07ffe-112">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="07ffe-112">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="07ffe-113">Listar Propriedades e relações dos objetos [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="07ffe-113">List properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) objects.</span></span>|
|[<span data-ttu-id="07ffe-114">Obter groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="07ffe-114">Get groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[<span data-ttu-id="07ffe-115">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="07ffe-115">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="07ffe-116">Leia as propriedades e as relações do objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="07ffe-116">Read properties and relationships of the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="07ffe-117">Criar groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="07ffe-117">Create groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[<span data-ttu-id="07ffe-118">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="07ffe-118">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="07ffe-119">Criar um novo objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="07ffe-119">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|
|[<span data-ttu-id="07ffe-120">Excluir groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="07ffe-120">Delete groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|<span data-ttu-id="07ffe-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07ffe-121">None</span></span>|<span data-ttu-id="07ffe-122">Exclui [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span><span class="sxs-lookup"><span data-stu-id="07ffe-122">Deletes a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>|
|[<span data-ttu-id="07ffe-123">Atualizar groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="07ffe-123">Update groupPolicyDefinitionValue</span></span>](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[<span data-ttu-id="07ffe-124">groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="07ffe-124">groupPolicyDefinitionValue</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|<span data-ttu-id="07ffe-125">Atualiza as propriedades de um objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="07ffe-125">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07ffe-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07ffe-126">Properties</span></span>
|<span data-ttu-id="07ffe-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07ffe-127">Property</span></span>|<span data-ttu-id="07ffe-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="07ffe-128">Type</span></span>|<span data-ttu-id="07ffe-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="07ffe-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07ffe-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07ffe-130">createdDateTime</span></span>|<span data-ttu-id="07ffe-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07ffe-131">DateTimeOffset</span></span>|<span data-ttu-id="07ffe-132">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="07ffe-132">The date and time the object was created.</span></span>|
|<span data-ttu-id="07ffe-133">enabled</span><span class="sxs-lookup"><span data-stu-id="07ffe-133">enabled</span></span>|<span data-ttu-id="07ffe-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="07ffe-134">Boolean</span></span>|<span data-ttu-id="07ffe-135">Habilita ou desabilita a definição de política de grupo associada.</span><span class="sxs-lookup"><span data-stu-id="07ffe-135">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="07ffe-136">ConfigurationType</span><span class="sxs-lookup"><span data-stu-id="07ffe-136">configurationType</span></span>|[<span data-ttu-id="07ffe-137">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="07ffe-137">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="07ffe-138">Especifica como o valor deve ser configurado.</span><span class="sxs-lookup"><span data-stu-id="07ffe-138">Specifies how the value should be configured.</span></span> <span data-ttu-id="07ffe-139">Isso pode ser uma política ou uma preferência.</span><span class="sxs-lookup"><span data-stu-id="07ffe-139">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="07ffe-140">Os valores possíveis são: `policy` e `preference`.</span><span class="sxs-lookup"><span data-stu-id="07ffe-140">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="07ffe-141">id</span><span class="sxs-lookup"><span data-stu-id="07ffe-141">id</span></span>|<span data-ttu-id="07ffe-142">String</span><span class="sxs-lookup"><span data-stu-id="07ffe-142">String</span></span>|<span data-ttu-id="07ffe-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="07ffe-143">Key of the entity.</span></span>|
|<span data-ttu-id="07ffe-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07ffe-144">lastModifiedDateTime</span></span>|<span data-ttu-id="07ffe-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07ffe-145">DateTimeOffset</span></span>|<span data-ttu-id="07ffe-146">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="07ffe-146">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07ffe-147">Relações</span><span class="sxs-lookup"><span data-stu-id="07ffe-147">Relationships</span></span>
|<span data-ttu-id="07ffe-148">Relação</span><span class="sxs-lookup"><span data-stu-id="07ffe-148">Relationship</span></span>|<span data-ttu-id="07ffe-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="07ffe-149">Type</span></span>|<span data-ttu-id="07ffe-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="07ffe-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07ffe-151">presentationValues</span><span class="sxs-lookup"><span data-stu-id="07ffe-151">presentationValues</span></span>|<span data-ttu-id="07ffe-152">coleção [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="07ffe-152">[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) collection</span></span>|<span data-ttu-id="07ffe-153">Os valores da apresentação da política de grupo associada com o valor de definição.</span><span class="sxs-lookup"><span data-stu-id="07ffe-153">The associated group policy presentation values with the definition value.</span></span>|
|<span data-ttu-id="07ffe-154">definir</span><span class="sxs-lookup"><span data-stu-id="07ffe-154">definition</span></span>|[<span data-ttu-id="07ffe-155">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="07ffe-155">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="07ffe-156">A definição da política de grupo associada com o valor.</span><span class="sxs-lookup"><span data-stu-id="07ffe-156">The associated group policy definition with the value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07ffe-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07ffe-157">JSON Representation</span></span>
<span data-ttu-id="07ffe-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07ffe-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "String (timestamp)",
  "enabled": true,
  "configurationType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





