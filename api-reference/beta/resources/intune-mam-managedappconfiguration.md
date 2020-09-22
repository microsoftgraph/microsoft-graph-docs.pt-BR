---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc34ab5464b1da8140d9d93f95ce1b34ab9ec9b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030434"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="0e986-103">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e986-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="0e986-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e986-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e986-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e986-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e986-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e986-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e986-107">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="0e986-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="0e986-108">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0e986-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0e986-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="0e986-109">Methods</span></span>
|<span data-ttu-id="0e986-110">Método</span><span class="sxs-lookup"><span data-stu-id="0e986-110">Method</span></span>|<span data-ttu-id="0e986-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0e986-111">Return Type</span></span>|<span data-ttu-id="0e986-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e986-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e986-113">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="0e986-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="0e986-114">Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e986-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="0e986-115">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e986-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0e986-116">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e986-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="0e986-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e986-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="0e986-118">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e986-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e986-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e986-119">Properties</span></span>
|<span data-ttu-id="0e986-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e986-120">Property</span></span>|<span data-ttu-id="0e986-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e986-121">Type</span></span>|<span data-ttu-id="0e986-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e986-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e986-123">displayName</span><span class="sxs-lookup"><span data-stu-id="0e986-123">displayName</span></span>|<span data-ttu-id="0e986-124">String</span><span class="sxs-lookup"><span data-stu-id="0e986-124">String</span></span>|<span data-ttu-id="0e986-125">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="0e986-125">Policy display name.</span></span> <span data-ttu-id="0e986-126">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0e986-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0e986-127">description</span><span class="sxs-lookup"><span data-stu-id="0e986-127">description</span></span>|<span data-ttu-id="0e986-128">String</span><span class="sxs-lookup"><span data-stu-id="0e986-128">String</span></span>|<span data-ttu-id="0e986-129">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="0e986-129">The policy's description.</span></span> <span data-ttu-id="0e986-130">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0e986-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0e986-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e986-131">createdDateTime</span></span>|<span data-ttu-id="0e986-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e986-132">DateTimeOffset</span></span>|<span data-ttu-id="0e986-133">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="0e986-133">The date and time the policy was created.</span></span> <span data-ttu-id="0e986-134">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0e986-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0e986-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e986-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0e986-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e986-136">DateTimeOffset</span></span>|<span data-ttu-id="0e986-137">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="0e986-137">Last time the policy was modified.</span></span> <span data-ttu-id="0e986-138">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0e986-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0e986-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e986-139">roleScopeTagIds</span></span>|<span data-ttu-id="0e986-140">Coleção String</span><span class="sxs-lookup"><span data-stu-id="0e986-140">String collection</span></span>|<span data-ttu-id="0e986-141">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0e986-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0e986-142">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0e986-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0e986-143">id</span><span class="sxs-lookup"><span data-stu-id="0e986-143">id</span></span>|<span data-ttu-id="0e986-144">String</span><span class="sxs-lookup"><span data-stu-id="0e986-144">String</span></span>|<span data-ttu-id="0e986-145">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0e986-145">Key of the entity.</span></span> <span data-ttu-id="0e986-146">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0e986-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0e986-147">version</span><span class="sxs-lookup"><span data-stu-id="0e986-147">version</span></span>|<span data-ttu-id="0e986-148">String</span><span class="sxs-lookup"><span data-stu-id="0e986-148">String</span></span>|<span data-ttu-id="0e986-149">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="0e986-149">Version of the entity.</span></span> <span data-ttu-id="0e986-150">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0e986-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0e986-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="0e986-151">customSettings</span></span>|<span data-ttu-id="0e986-152">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0e986-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0e986-153">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="0e986-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e986-154">Relações</span><span class="sxs-lookup"><span data-stu-id="0e986-154">Relationships</span></span>
<span data-ttu-id="0e986-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e986-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e986-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e986-156">JSON Representation</span></span>
<span data-ttu-id="0e986-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e986-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```






