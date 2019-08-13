---
title: tipo de recurso groupPolicyConfiguration
description: A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 43f0f9970a3d94285d1abe06c86eff83f2bed818
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331529"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="48b25-103">tipo de recurso groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="48b25-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="48b25-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48b25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48b25-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48b25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48b25-106">A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="48b25-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="48b25-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="48b25-107">Methods</span></span>
|<span data-ttu-id="48b25-108">Método</span><span class="sxs-lookup"><span data-stu-id="48b25-108">Method</span></span>|<span data-ttu-id="48b25-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48b25-109">Return Type</span></span>|<span data-ttu-id="48b25-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="48b25-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="48b25-111">Listar groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="48b25-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="48b25-112">coleção [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48b25-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="48b25-113">Listar Propriedades e relações dos objetos [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48b25-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="48b25-114">Obter groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="48b25-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="48b25-115">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="48b25-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="48b25-116">Leia as propriedades e as relações do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48b25-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="48b25-117">Criar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="48b25-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="48b25-118">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="48b25-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="48b25-119">Criar um novo objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48b25-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="48b25-120">Excluir groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="48b25-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="48b25-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48b25-121">None</span></span>|<span data-ttu-id="48b25-122">Exclui [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48b25-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="48b25-123">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="48b25-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="48b25-124">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="48b25-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="48b25-125">Atualiza as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48b25-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="48b25-126">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="48b25-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="48b25-127">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="48b25-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="48b25-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48b25-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="48b25-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48b25-129">Properties</span></span>
|<span data-ttu-id="48b25-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48b25-130">Property</span></span>|<span data-ttu-id="48b25-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="48b25-131">Type</span></span>|<span data-ttu-id="48b25-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="48b25-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48b25-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48b25-133">createdDateTime</span></span>|<span data-ttu-id="48b25-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48b25-134">DateTimeOffset</span></span>|<span data-ttu-id="48b25-135">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="48b25-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="48b25-136">displayName</span><span class="sxs-lookup"><span data-stu-id="48b25-136">displayName</span></span>|<span data-ttu-id="48b25-137">String</span><span class="sxs-lookup"><span data-stu-id="48b25-137">String</span></span>|<span data-ttu-id="48b25-138">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="48b25-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="48b25-139">descrição</span><span class="sxs-lookup"><span data-stu-id="48b25-139">description</span></span>|<span data-ttu-id="48b25-140">String</span><span class="sxs-lookup"><span data-stu-id="48b25-140">String</span></span>|<span data-ttu-id="48b25-141">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="48b25-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="48b25-142">id</span><span class="sxs-lookup"><span data-stu-id="48b25-142">id</span></span>|<span data-ttu-id="48b25-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48b25-143">String</span></span>|<span data-ttu-id="48b25-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="48b25-144">Key of the entity.</span></span>|
|<span data-ttu-id="48b25-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48b25-145">lastModifiedDateTime</span></span>|<span data-ttu-id="48b25-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48b25-146">DateTimeOffset</span></span>|<span data-ttu-id="48b25-147">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="48b25-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48b25-148">Relações</span><span class="sxs-lookup"><span data-stu-id="48b25-148">Relationships</span></span>
|<span data-ttu-id="48b25-149">Relação</span><span class="sxs-lookup"><span data-stu-id="48b25-149">Relationship</span></span>|<span data-ttu-id="48b25-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="48b25-150">Type</span></span>|<span data-ttu-id="48b25-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="48b25-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48b25-152">definitionValues</span><span class="sxs-lookup"><span data-stu-id="48b25-152">definitionValues</span></span>|<span data-ttu-id="48b25-153">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="48b25-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="48b25-154">A lista de valores de definição de política de grupo habilitados ou desabilitados para a configuração.</span><span class="sxs-lookup"><span data-stu-id="48b25-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="48b25-155">assignments</span><span class="sxs-lookup"><span data-stu-id="48b25-155">assignments</span></span>|<span data-ttu-id="48b25-156">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="48b25-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="48b25-157">A lista de atribuições de grupo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="48b25-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48b25-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48b25-158">JSON Representation</span></span>
<span data-ttu-id="48b25-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48b25-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



