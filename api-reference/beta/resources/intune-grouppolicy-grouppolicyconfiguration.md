---
title: tipo de recurso groupPolicyConfiguration
description: A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d910bf8bdef34c60ca6bb66e1ce87ca9cf1d51ab
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941174"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="f4278-103">tipo de recurso groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4278-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="f4278-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4278-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4278-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4278-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4278-106">A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f4278-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="f4278-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f4278-107">Methods</span></span>
|<span data-ttu-id="f4278-108">Método</span><span class="sxs-lookup"><span data-stu-id="f4278-108">Method</span></span>|<span data-ttu-id="f4278-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4278-109">Return Type</span></span>|<span data-ttu-id="f4278-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4278-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4278-111">Listar groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="f4278-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="f4278-112">coleção [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4278-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="f4278-113">Listar Propriedades e relações dos objetos [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f4278-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f4278-114">Obter groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4278-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="f4278-115">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4278-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="f4278-116">Leia as propriedades e as relações do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f4278-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f4278-117">Criar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4278-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="f4278-118">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4278-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="f4278-119">Criar um novo objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f4278-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f4278-120">Excluir groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4278-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="f4278-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4278-121">None</span></span>|<span data-ttu-id="f4278-122">Exclui [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4278-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="f4278-123">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4278-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="f4278-124">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4278-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="f4278-125">Atualiza as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f4278-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f4278-126">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="f4278-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="f4278-127">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f4278-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f4278-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f4278-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f4278-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4278-129">Properties</span></span>
|<span data-ttu-id="f4278-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4278-130">Property</span></span>|<span data-ttu-id="f4278-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4278-131">Type</span></span>|<span data-ttu-id="f4278-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4278-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4278-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4278-133">createdDateTime</span></span>|<span data-ttu-id="f4278-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4278-134">DateTimeOffset</span></span>|<span data-ttu-id="f4278-135">A data e a hora em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f4278-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="f4278-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f4278-136">displayName</span></span>|<span data-ttu-id="f4278-137">String</span><span class="sxs-lookup"><span data-stu-id="f4278-137">String</span></span>|<span data-ttu-id="f4278-138">Nome fornecido pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="f4278-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="f4278-139">description</span><span class="sxs-lookup"><span data-stu-id="f4278-139">description</span></span>|<span data-ttu-id="f4278-140">String</span><span class="sxs-lookup"><span data-stu-id="f4278-140">String</span></span>|<span data-ttu-id="f4278-141">Descrição fornecida pelo usuário para o objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="f4278-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="f4278-142">id</span><span class="sxs-lookup"><span data-stu-id="f4278-142">id</span></span>|<span data-ttu-id="f4278-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4278-143">String</span></span>|<span data-ttu-id="f4278-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4278-144">Key of the entity.</span></span>|
|<span data-ttu-id="f4278-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4278-145">lastModifiedDateTime</span></span>|<span data-ttu-id="f4278-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4278-146">DateTimeOffset</span></span>|<span data-ttu-id="f4278-147">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f4278-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4278-148">Relações</span><span class="sxs-lookup"><span data-stu-id="f4278-148">Relationships</span></span>
|<span data-ttu-id="f4278-149">Relação</span><span class="sxs-lookup"><span data-stu-id="f4278-149">Relationship</span></span>|<span data-ttu-id="f4278-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4278-150">Type</span></span>|<span data-ttu-id="f4278-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4278-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4278-152">definitionValues</span><span class="sxs-lookup"><span data-stu-id="f4278-152">definitionValues</span></span>|<span data-ttu-id="f4278-153">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f4278-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="f4278-154">A lista de valores de definição de política de grupo habilitados ou desabilitados para a configuração.</span><span class="sxs-lookup"><span data-stu-id="f4278-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="f4278-155">assignments</span><span class="sxs-lookup"><span data-stu-id="f4278-155">assignments</span></span>|<span data-ttu-id="f4278-156">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f4278-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f4278-157">A lista de atribuições de grupo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="f4278-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4278-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4278-158">JSON Representation</span></span>
<span data-ttu-id="f4278-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4278-159">Here is a JSON representation of the resource.</span></span>
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




