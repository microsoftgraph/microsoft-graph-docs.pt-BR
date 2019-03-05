---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3c8db1f356890dc478833e7b77267a218f08bbc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148080"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="7c1c6-103">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c1c6-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="7c1c6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c1c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c1c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c1c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c1c6-106">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="7c1c6-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="7c1c6-107">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7c1c6-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7c1c6-108">Methods</span></span>
|<span data-ttu-id="7c1c6-109">Método</span><span class="sxs-lookup"><span data-stu-id="7c1c6-109">Method</span></span>|<span data-ttu-id="7c1c6-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7c1c6-110">Return Type</span></span>|<span data-ttu-id="7c1c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c1c6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7c1c6-112">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="7c1c6-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="7c1c6-113">Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="7c1c6-114">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c1c6-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="7c1c6-115">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c1c6-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="7c1c6-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c1c6-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="7c1c6-117">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c1c6-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c1c6-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c1c6-118">Properties</span></span>
|<span data-ttu-id="7c1c6-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c1c6-119">Property</span></span>|<span data-ttu-id="7c1c6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c1c6-120">Type</span></span>|<span data-ttu-id="7c1c6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c1c6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c1c6-122">displayName</span><span class="sxs-lookup"><span data-stu-id="7c1c6-122">displayName</span></span>|<span data-ttu-id="7c1c6-123">String</span><span class="sxs-lookup"><span data-stu-id="7c1c6-123">String</span></span>|<span data-ttu-id="7c1c6-124">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="7c1c6-124">Policy display name.</span></span> <span data-ttu-id="7c1c6-125">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c1c6-126">descrição</span><span class="sxs-lookup"><span data-stu-id="7c1c6-126">description</span></span>|<span data-ttu-id="7c1c6-127">String</span><span class="sxs-lookup"><span data-stu-id="7c1c6-127">String</span></span>|<span data-ttu-id="7c1c6-128">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="7c1c6-128">The policy's description.</span></span> <span data-ttu-id="7c1c6-129">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c1c6-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c1c6-130">createdDateTime</span></span>|<span data-ttu-id="7c1c6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c1c6-131">DateTimeOffset</span></span>|<span data-ttu-id="7c1c6-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="7c1c6-132">The date and time the policy was created.</span></span> <span data-ttu-id="7c1c6-133">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c1c6-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c1c6-134">lastModifiedDateTime</span></span>|<span data-ttu-id="7c1c6-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c1c6-135">DateTimeOffset</span></span>|<span data-ttu-id="7c1c6-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="7c1c6-136">Last time the policy was modified.</span></span> <span data-ttu-id="7c1c6-137">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c1c6-138">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7c1c6-138">roleScopeTagIds</span></span>|<span data-ttu-id="7c1c6-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c1c6-139">String collection</span></span>|<span data-ttu-id="7c1c6-140">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7c1c6-140">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7c1c6-141">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c1c6-142">id</span><span class="sxs-lookup"><span data-stu-id="7c1c6-142">id</span></span>|<span data-ttu-id="7c1c6-143">String</span><span class="sxs-lookup"><span data-stu-id="7c1c6-143">String</span></span>|<span data-ttu-id="7c1c6-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7c1c6-144">Key of the entity.</span></span> <span data-ttu-id="7c1c6-145">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c1c6-146">version</span><span class="sxs-lookup"><span data-stu-id="7c1c6-146">version</span></span>|<span data-ttu-id="7c1c6-147">String</span><span class="sxs-lookup"><span data-stu-id="7c1c6-147">String</span></span>|<span data-ttu-id="7c1c6-148">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="7c1c6-148">Version of the entity.</span></span> <span data-ttu-id="7c1c6-149">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="7c1c6-150">customSettings</span><span class="sxs-lookup"><span data-stu-id="7c1c6-150">customSettings</span></span>|<span data-ttu-id="7c1c6-151">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7c1c6-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7c1c6-152">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="7c1c6-152">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c1c6-153">Relações</span><span class="sxs-lookup"><span data-stu-id="7c1c6-153">Relationships</span></span>
<span data-ttu-id="7c1c6-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c1c6-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c1c6-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c1c6-155">JSON Representation</span></span>
<span data-ttu-id="7c1c6-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c1c6-156">Here is a JSON representation of the resource.</span></span>
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




