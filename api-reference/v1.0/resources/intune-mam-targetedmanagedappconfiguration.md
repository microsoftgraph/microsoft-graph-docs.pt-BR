---
title: Tipo de recurso targetedManagedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para todos os usuários do grupo de segurança visado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 371541835ae900c0988ebe817bcf2c57dccf764d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474093"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="2c17a-103">Tipo de recurso targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c17a-103">targetedManagedAppConfiguration resource type</span></span>

<span data-ttu-id="2c17a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c17a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c17a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c17a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c17a-106">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para todos os usuários do grupo de segurança visado</span><span class="sxs-lookup"><span data-stu-id="2c17a-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="2c17a-107">Herda de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2c17a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="2c17a-108">Methods</span></span>
|<span data-ttu-id="2c17a-109">Método</span><span class="sxs-lookup"><span data-stu-id="2c17a-109">Method</span></span>|<span data-ttu-id="2c17a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2c17a-110">Return Type</span></span>|<span data-ttu-id="2c17a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c17a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2c17a-112">Listar targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="2c17a-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="2c17a-113">Coleção [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="2c17a-114">Listar propriedades e relações dos objetos [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c17a-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="2c17a-115">Obter targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c17a-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="2c17a-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c17a-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="2c17a-117">Ler propriedades e relações do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c17a-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2c17a-118">Criar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c17a-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="2c17a-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c17a-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="2c17a-120">Cria um novo objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c17a-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2c17a-121">Excluir targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c17a-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="2c17a-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c17a-122">None</span></span>|<span data-ttu-id="2c17a-123">Excluir um [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c17a-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="2c17a-124">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c17a-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="2c17a-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c17a-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="2c17a-126">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c17a-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2c17a-127">Ação assign</span><span class="sxs-lookup"><span data-stu-id="2c17a-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="2c17a-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2c17a-128">None</span></span>|<span data-ttu-id="2c17a-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2c17a-129">Not yet documented</span></span>|
|[<span data-ttu-id="2c17a-130">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="2c17a-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="2c17a-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2c17a-131">None</span></span>|<span data-ttu-id="2c17a-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2c17a-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2c17a-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c17a-133">Properties</span></span>
|<span data-ttu-id="2c17a-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c17a-134">Property</span></span>|<span data-ttu-id="2c17a-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c17a-135">Type</span></span>|<span data-ttu-id="2c17a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c17a-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c17a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2c17a-137">displayName</span></span>|<span data-ttu-id="2c17a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c17a-138">String</span></span>|<span data-ttu-id="2c17a-139">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="2c17a-139">Policy display name.</span></span> <span data-ttu-id="2c17a-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c17a-141">description</span><span class="sxs-lookup"><span data-stu-id="2c17a-141">description</span></span>|<span data-ttu-id="2c17a-142">String</span><span class="sxs-lookup"><span data-stu-id="2c17a-142">String</span></span>|<span data-ttu-id="2c17a-143">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="2c17a-143">The policy's description.</span></span> <span data-ttu-id="2c17a-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c17a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c17a-145">createdDateTime</span></span>|<span data-ttu-id="2c17a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c17a-146">DateTimeOffset</span></span>|<span data-ttu-id="2c17a-147">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="2c17a-147">The date and time the policy was created.</span></span> <span data-ttu-id="2c17a-148">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c17a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c17a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2c17a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c17a-150">DateTimeOffset</span></span>|<span data-ttu-id="2c17a-151">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="2c17a-151">Last time the policy was modified.</span></span> <span data-ttu-id="2c17a-152">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c17a-153">id</span><span class="sxs-lookup"><span data-stu-id="2c17a-153">id</span></span>|<span data-ttu-id="2c17a-154">String</span><span class="sxs-lookup"><span data-stu-id="2c17a-154">String</span></span>|<span data-ttu-id="2c17a-155">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2c17a-155">Key of the entity.</span></span> <span data-ttu-id="2c17a-156">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c17a-157">version</span><span class="sxs-lookup"><span data-stu-id="2c17a-157">version</span></span>|<span data-ttu-id="2c17a-158">String</span><span class="sxs-lookup"><span data-stu-id="2c17a-158">String</span></span>|<span data-ttu-id="2c17a-159">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="2c17a-159">Version of the entity.</span></span> <span data-ttu-id="2c17a-160">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2c17a-161">customSettings</span><span class="sxs-lookup"><span data-stu-id="2c17a-161">customSettings</span></span>|<span data-ttu-id="2c17a-162">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-162">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2c17a-163">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-163">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="2c17a-164">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="2c17a-164">deployedAppCount</span></span>|<span data-ttu-id="2c17a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2c17a-165">Int32</span></span>|<span data-ttu-id="2c17a-166">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="2c17a-166">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="2c17a-167">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2c17a-167">isAssigned</span></span>|<span data-ttu-id="2c17a-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c17a-168">Boolean</span></span>|<span data-ttu-id="2c17a-169">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="2c17a-169">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c17a-170">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="2c17a-170">Relationships</span></span>
|<span data-ttu-id="2c17a-171">Relação</span><span class="sxs-lookup"><span data-stu-id="2c17a-171">Relationship</span></span>|<span data-ttu-id="2c17a-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c17a-172">Type</span></span>|<span data-ttu-id="2c17a-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c17a-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c17a-174">apps</span><span class="sxs-lookup"><span data-stu-id="2c17a-174">apps</span></span>|<span data-ttu-id="2c17a-175">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-175">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="2c17a-176">Lista de aplicativos em que a política é implantada.</span><span class="sxs-lookup"><span data-stu-id="2c17a-176">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="2c17a-177">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="2c17a-177">deploymentSummary</span></span>|[<span data-ttu-id="2c17a-178">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="2c17a-178">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="2c17a-179">Propriedade de navegação para o resumo de implantação da configuração.</span><span class="sxs-lookup"><span data-stu-id="2c17a-179">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="2c17a-180">assignments</span><span class="sxs-lookup"><span data-stu-id="2c17a-180">assignments</span></span>|<span data-ttu-id="2c17a-181">Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2c17a-181">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="2c17a-182">Propriedades de navegação para lista de grupos de inclusão e exclusão às quais a política é implantada.</span><span class="sxs-lookup"><span data-stu-id="2c17a-182">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c17a-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c17a-183">JSON Representation</span></span>
<span data-ttu-id="2c17a-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c17a-184">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```







