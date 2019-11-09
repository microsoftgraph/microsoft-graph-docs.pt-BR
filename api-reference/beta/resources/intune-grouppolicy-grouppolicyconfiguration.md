---
title: tipo de recurso groupPolicyConfiguration
description: A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c9ee783ffa3e037243a78cd49187511797e221de
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088067"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="d9992-103">tipo de recurso groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9992-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="d9992-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9992-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9992-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9992-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9992-106">A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="d9992-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="d9992-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d9992-107">Methods</span></span>
|<span data-ttu-id="d9992-108">Método</span><span class="sxs-lookup"><span data-stu-id="d9992-108">Method</span></span>|<span data-ttu-id="d9992-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d9992-109">Return Type</span></span>|<span data-ttu-id="d9992-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9992-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9992-111">Listar groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="d9992-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="d9992-112">coleção [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9992-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="d9992-113">Listar Propriedades e relações dos objetos [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d9992-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d9992-114">Obter groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9992-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="d9992-115">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9992-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="d9992-116">Leia as propriedades e as relações do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d9992-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d9992-117">Criar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9992-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="d9992-118">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9992-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="d9992-119">Criar um novo objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d9992-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d9992-120">Excluir groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9992-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="d9992-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9992-121">None</span></span>|<span data-ttu-id="d9992-122">Exclui [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9992-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="d9992-123">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9992-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="d9992-124">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9992-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="d9992-125">Atualiza as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d9992-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d9992-126">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="d9992-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="d9992-127">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d9992-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d9992-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9992-128">Not yet documented</span></span>|
|[<span data-ttu-id="d9992-129">ação updateDefinitionValues</span><span class="sxs-lookup"><span data-stu-id="d9992-129">updateDefinitionValues action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|<span data-ttu-id="d9992-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d9992-130">None</span></span>|<span data-ttu-id="d9992-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9992-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d9992-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9992-132">Properties</span></span>
|<span data-ttu-id="d9992-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9992-133">Property</span></span>|<span data-ttu-id="d9992-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9992-134">Type</span></span>|<span data-ttu-id="d9992-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9992-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9992-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9992-136">createdDateTime</span></span>|<span data-ttu-id="d9992-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9992-137">DateTimeOffset</span></span>|<span data-ttu-id="d9992-138">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d9992-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="d9992-139">displayName</span><span class="sxs-lookup"><span data-stu-id="d9992-139">displayName</span></span>|<span data-ttu-id="d9992-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9992-140">String</span></span>|<span data-ttu-id="d9992-141">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="d9992-141">User provided name for the resource object.</span></span>|
|<span data-ttu-id="d9992-142">descrição</span><span class="sxs-lookup"><span data-stu-id="d9992-142">description</span></span>|<span data-ttu-id="d9992-143">String</span><span class="sxs-lookup"><span data-stu-id="d9992-143">String</span></span>|<span data-ttu-id="d9992-144">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="d9992-144">User provided description for the resource object.</span></span>|
|<span data-ttu-id="d9992-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d9992-145">roleScopeTagIds</span></span>|<span data-ttu-id="d9992-146">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d9992-146">String collection</span></span>|<span data-ttu-id="d9992-147">A lista de marcas de escopo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="d9992-147">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="d9992-148">id</span><span class="sxs-lookup"><span data-stu-id="d9992-148">id</span></span>|<span data-ttu-id="d9992-149">String</span><span class="sxs-lookup"><span data-stu-id="d9992-149">String</span></span>|<span data-ttu-id="d9992-150">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d9992-150">Key of the entity.</span></span>|
|<span data-ttu-id="d9992-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9992-151">lastModifiedDateTime</span></span>|<span data-ttu-id="d9992-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9992-152">DateTimeOffset</span></span>|<span data-ttu-id="d9992-153">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d9992-153">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9992-154">Relações</span><span class="sxs-lookup"><span data-stu-id="d9992-154">Relationships</span></span>
|<span data-ttu-id="d9992-155">Relação</span><span class="sxs-lookup"><span data-stu-id="d9992-155">Relationship</span></span>|<span data-ttu-id="d9992-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9992-156">Type</span></span>|<span data-ttu-id="d9992-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9992-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9992-158">definitionValues</span><span class="sxs-lookup"><span data-stu-id="d9992-158">definitionValues</span></span>|<span data-ttu-id="d9992-159">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d9992-159">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="d9992-160">A lista de valores de definição de política de grupo habilitados ou desabilitados para a configuração.</span><span class="sxs-lookup"><span data-stu-id="d9992-160">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="d9992-161">assignments</span><span class="sxs-lookup"><span data-stu-id="d9992-161">assignments</span></span>|<span data-ttu-id="d9992-162">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d9992-162">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d9992-163">A lista de atribuições de grupo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="d9992-163">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9992-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9992-164">JSON Representation</span></span>
<span data-ttu-id="d9992-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9992-165">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



