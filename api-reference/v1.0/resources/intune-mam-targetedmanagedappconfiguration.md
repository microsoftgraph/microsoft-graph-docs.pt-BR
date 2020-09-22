---
title: Tipo de recurso targetedManagedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para todos os usuários do grupo de segurança visado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d650cbfc96c3382671fec8d92e88c92200adaa8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048341"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a><span data-ttu-id="23924-103">Tipo de recurso targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="23924-103">targetedManagedAppConfiguration resource type</span></span>

<span data-ttu-id="23924-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23924-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23924-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23924-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23924-106">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para todos os usuários do grupo de segurança visado</span><span class="sxs-lookup"><span data-stu-id="23924-106">Configuration used to deliver a set of custom settings as-is to all users in the targeted security group</span></span>


<span data-ttu-id="23924-107">Herda de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23924-107">Inherits from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="23924-108">Methods</span><span class="sxs-lookup"><span data-stu-id="23924-108">Methods</span></span>
|<span data-ttu-id="23924-109">Método</span><span class="sxs-lookup"><span data-stu-id="23924-109">Method</span></span>|<span data-ttu-id="23924-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23924-110">Return Type</span></span>|<span data-ttu-id="23924-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="23924-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23924-112">Listar targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="23924-112">List targetedManagedAppConfigurations</span></span>](../api/intune-mam-targetedmanagedappconfiguration-list.md)|<span data-ttu-id="23924-113">Coleção [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23924-113">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) collection</span></span>|<span data-ttu-id="23924-114">Listar propriedades e relações dos objetos [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23924-114">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="23924-115">Obter targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="23924-115">Get targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[<span data-ttu-id="23924-116">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="23924-116">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="23924-117">Ler propriedades e relações do objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23924-117">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="23924-118">Criar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="23924-118">Create targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[<span data-ttu-id="23924-119">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="23924-119">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="23924-120">Cria um novo objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23924-120">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="23924-121">Excluir targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="23924-121">Delete targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|<span data-ttu-id="23924-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23924-122">None</span></span>|<span data-ttu-id="23924-123">Excluir um [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23924-123">Deletes a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>|
|[<span data-ttu-id="23924-124">Atualizar targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="23924-124">Update targetedManagedAppConfiguration</span></span>](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[<span data-ttu-id="23924-125">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="23924-125">targetedManagedAppConfiguration</span></span>](../resources/intune-mam-targetedmanagedappconfiguration.md)|<span data-ttu-id="23924-126">Atualizar as propriedades de um objeto [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23924-126">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="23924-127">Ação assign</span><span class="sxs-lookup"><span data-stu-id="23924-127">assign action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|<span data-ttu-id="23924-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="23924-128">None</span></span>|<span data-ttu-id="23924-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23924-129">Not yet documented</span></span>|
|[<span data-ttu-id="23924-130">Ação targetApps</span><span class="sxs-lookup"><span data-stu-id="23924-130">targetApps action</span></span>](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|<span data-ttu-id="23924-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23924-131">None</span></span>|<span data-ttu-id="23924-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23924-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="23924-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23924-133">Properties</span></span>
|<span data-ttu-id="23924-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23924-134">Property</span></span>|<span data-ttu-id="23924-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="23924-135">Type</span></span>|<span data-ttu-id="23924-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="23924-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23924-137">displayName</span><span class="sxs-lookup"><span data-stu-id="23924-137">displayName</span></span>|<span data-ttu-id="23924-138">String</span><span class="sxs-lookup"><span data-stu-id="23924-138">String</span></span>|<span data-ttu-id="23924-139">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="23924-139">Policy display name.</span></span> <span data-ttu-id="23924-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23924-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="23924-141">description</span><span class="sxs-lookup"><span data-stu-id="23924-141">description</span></span>|<span data-ttu-id="23924-142">String</span><span class="sxs-lookup"><span data-stu-id="23924-142">String</span></span>|<span data-ttu-id="23924-143">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="23924-143">The policy's description.</span></span> <span data-ttu-id="23924-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23924-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="23924-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23924-145">createdDateTime</span></span>|<span data-ttu-id="23924-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23924-146">DateTimeOffset</span></span>|<span data-ttu-id="23924-147">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="23924-147">The date and time the policy was created.</span></span> <span data-ttu-id="23924-148">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23924-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="23924-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23924-149">lastModifiedDateTime</span></span>|<span data-ttu-id="23924-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23924-150">DateTimeOffset</span></span>|<span data-ttu-id="23924-151">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="23924-151">Last time the policy was modified.</span></span> <span data-ttu-id="23924-152">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23924-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="23924-153">id</span><span class="sxs-lookup"><span data-stu-id="23924-153">id</span></span>|<span data-ttu-id="23924-154">String</span><span class="sxs-lookup"><span data-stu-id="23924-154">String</span></span>|<span data-ttu-id="23924-155">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="23924-155">Key of the entity.</span></span> <span data-ttu-id="23924-156">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23924-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="23924-157">version</span><span class="sxs-lookup"><span data-stu-id="23924-157">version</span></span>|<span data-ttu-id="23924-158">String</span><span class="sxs-lookup"><span data-stu-id="23924-158">String</span></span>|<span data-ttu-id="23924-159">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="23924-159">Version of the entity.</span></span> <span data-ttu-id="23924-160">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="23924-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="23924-161">customSettings</span><span class="sxs-lookup"><span data-stu-id="23924-161">customSettings</span></span>|<span data-ttu-id="23924-162">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="23924-162">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="23924-163">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço Herdado de [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23924-163">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="23924-164">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="23924-164">deployedAppCount</span></span>|<span data-ttu-id="23924-165">Int32</span><span class="sxs-lookup"><span data-stu-id="23924-165">Int32</span></span>|<span data-ttu-id="23924-166">Contagem de aplicativos em que a política atual é implantada.</span><span class="sxs-lookup"><span data-stu-id="23924-166">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="23924-167">isAssigned</span><span class="sxs-lookup"><span data-stu-id="23924-167">isAssigned</span></span>|<span data-ttu-id="23924-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="23924-168">Boolean</span></span>|<span data-ttu-id="23924-169">Indica se a política foi implantada a grupos de inclusão ou não.</span><span class="sxs-lookup"><span data-stu-id="23924-169">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23924-170">Relações</span><span class="sxs-lookup"><span data-stu-id="23924-170">Relationships</span></span>
|<span data-ttu-id="23924-171">Relação</span><span class="sxs-lookup"><span data-stu-id="23924-171">Relationship</span></span>|<span data-ttu-id="23924-172">Tipo</span><span class="sxs-lookup"><span data-stu-id="23924-172">Type</span></span>|<span data-ttu-id="23924-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="23924-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23924-174">apps</span><span class="sxs-lookup"><span data-stu-id="23924-174">apps</span></span>|<span data-ttu-id="23924-175">Coleção [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="23924-175">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="23924-176">Lista de aplicativos em que a política é implantada.</span><span class="sxs-lookup"><span data-stu-id="23924-176">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="23924-177">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="23924-177">deploymentSummary</span></span>|[<span data-ttu-id="23924-178">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="23924-178">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="23924-179">Propriedade de navegação para o resumo de implantação da configuração.</span><span class="sxs-lookup"><span data-stu-id="23924-179">Navigation property to deployment summary of the configuration.</span></span>|
|<span data-ttu-id="23924-180">assignments</span><span class="sxs-lookup"><span data-stu-id="23924-180">assignments</span></span>|<span data-ttu-id="23924-181">Conjunto [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="23924-181">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="23924-182">Propriedades de navegação para lista de grupos de inclusão e exclusão às quais a política é implantada.</span><span class="sxs-lookup"><span data-stu-id="23924-182">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23924-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23924-183">JSON Representation</span></span>
<span data-ttu-id="23924-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23924-184">Here is a JSON representation of the resource.</span></span>
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









