---
title: tipo de recurso de groupPolicyConfiguration
description: A entidade de configuração de diretiva de grupo contém os valores configurados para uma ou mais definições de política de grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be3b43ab0e9e3f87f53ed0dae144f2b6f4dce7b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431305"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="f71a9-103">tipo de recurso de groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f71a9-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="f71a9-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f71a9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f71a9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f71a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f71a9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f71a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f71a9-107">A entidade de configuração de diretiva de grupo contém os valores configurados para uma ou mais definições de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="f71a9-107">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="f71a9-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f71a9-108">Methods</span></span>
|<span data-ttu-id="f71a9-109">Método</span><span class="sxs-lookup"><span data-stu-id="f71a9-109">Method</span></span>|<span data-ttu-id="f71a9-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f71a9-110">Return Type</span></span>|<span data-ttu-id="f71a9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f71a9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f71a9-112">Lista groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="f71a9-112">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="f71a9-113">coleção [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f71a9-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="f71a9-114">Lista as propriedades e os relacionamentos dos objetos [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f71a9-114">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f71a9-115">Obter groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f71a9-115">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="f71a9-116">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f71a9-116">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="f71a9-117">Leia as propriedades e os relacionamentos do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f71a9-117">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f71a9-118">Criar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f71a9-118">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="f71a9-119">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f71a9-119">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="f71a9-120">Crie um novo objeto de [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f71a9-120">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f71a9-121">Excluir groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f71a9-121">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="f71a9-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f71a9-122">None</span></span>|<span data-ttu-id="f71a9-123">Exclui um [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f71a9-123">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="f71a9-124">Atualizar groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f71a9-124">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="f71a9-125">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="f71a9-125">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="f71a9-126">Atualize as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f71a9-126">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f71a9-127">Ação assign</span><span class="sxs-lookup"><span data-stu-id="f71a9-127">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="f71a9-128">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f71a9-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f71a9-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f71a9-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f71a9-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f71a9-130">Properties</span></span>
|<span data-ttu-id="f71a9-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f71a9-131">Property</span></span>|<span data-ttu-id="f71a9-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f71a9-132">Type</span></span>|<span data-ttu-id="f71a9-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f71a9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f71a9-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f71a9-134">createdDateTime</span></span>|<span data-ttu-id="f71a9-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f71a9-135">DateTimeOffset</span></span>|<span data-ttu-id="f71a9-136">A data e hora que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f71a9-136">The date and time the object was created.</span></span>|
|<span data-ttu-id="f71a9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f71a9-137">displayName</span></span>|<span data-ttu-id="f71a9-138">String</span><span class="sxs-lookup"><span data-stu-id="f71a9-138">String</span></span>|<span data-ttu-id="f71a9-139">Nome de usuário fornecido para o objeto resource.</span><span class="sxs-lookup"><span data-stu-id="f71a9-139">User provided name for the resource object.</span></span>|
|<span data-ttu-id="f71a9-140">description</span><span class="sxs-lookup"><span data-stu-id="f71a9-140">description</span></span>|<span data-ttu-id="f71a9-141">String</span><span class="sxs-lookup"><span data-stu-id="f71a9-141">String</span></span>|<span data-ttu-id="f71a9-142">Descrição para o objeto resource fornecidos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="f71a9-142">User provided description for the resource object.</span></span>|
|<span data-ttu-id="f71a9-143">id</span><span class="sxs-lookup"><span data-stu-id="f71a9-143">id</span></span>|<span data-ttu-id="f71a9-144">String</span><span class="sxs-lookup"><span data-stu-id="f71a9-144">String</span></span>|<span data-ttu-id="f71a9-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f71a9-145">Key of the entity.</span></span>|
|<span data-ttu-id="f71a9-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f71a9-146">lastModifiedDateTime</span></span>|<span data-ttu-id="f71a9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f71a9-147">DateTimeOffset</span></span>|<span data-ttu-id="f71a9-148">A data e hora que a entidade foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f71a9-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f71a9-149">Relações</span><span class="sxs-lookup"><span data-stu-id="f71a9-149">Relationships</span></span>
|<span data-ttu-id="f71a9-150">Relação</span><span class="sxs-lookup"><span data-stu-id="f71a9-150">Relationship</span></span>|<span data-ttu-id="f71a9-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="f71a9-151">Type</span></span>|<span data-ttu-id="f71a9-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="f71a9-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f71a9-153">definitionValues</span><span class="sxs-lookup"><span data-stu-id="f71a9-153">definitionValues</span></span>|<span data-ttu-id="f71a9-154">coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f71a9-154">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="f71a9-155">A lista de habilitada ou desabilitada valores de definição de diretiva de grupo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="f71a9-155">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="f71a9-156">assignments</span><span class="sxs-lookup"><span data-stu-id="f71a9-156">assignments</span></span>|<span data-ttu-id="f71a9-157">coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f71a9-157">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f71a9-158">A lista de atribuições de grupo para a configuração.</span><span class="sxs-lookup"><span data-stu-id="f71a9-158">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f71a9-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f71a9-159">JSON Representation</span></span>
<span data-ttu-id="f71a9-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f71a9-160">Here is a JSON representation of the resource.</span></span>
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




