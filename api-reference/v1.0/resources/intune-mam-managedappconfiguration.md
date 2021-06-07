---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffb8e5bbf86dceeedfe480676a18e70239a0d367
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754955"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="ced4b-103">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ced4b-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="ced4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ced4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ced4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ced4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ced4b-106">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="ced4b-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="ced4b-107">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ced4b-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ced4b-108">Methods</span><span class="sxs-lookup"><span data-stu-id="ced4b-108">Methods</span></span>
|<span data-ttu-id="ced4b-109">Método</span><span class="sxs-lookup"><span data-stu-id="ced4b-109">Method</span></span>|<span data-ttu-id="ced4b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ced4b-110">Return Type</span></span>|<span data-ttu-id="ced4b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ced4b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ced4b-112">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="ced4b-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="ced4b-113">Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ced4b-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="ced4b-114">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced4b-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ced4b-115">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ced4b-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="ced4b-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ced4b-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="ced4b-117">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ced4b-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ced4b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ced4b-118">Properties</span></span>
|<span data-ttu-id="ced4b-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ced4b-119">Property</span></span>|<span data-ttu-id="ced4b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ced4b-120">Type</span></span>|<span data-ttu-id="ced4b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ced4b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ced4b-122">displayName</span><span class="sxs-lookup"><span data-stu-id="ced4b-122">displayName</span></span>|<span data-ttu-id="ced4b-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ced4b-123">String</span></span>|<span data-ttu-id="ced4b-124">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="ced4b-124">Policy display name.</span></span> <span data-ttu-id="ced4b-125">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ced4b-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ced4b-126">descrição</span><span class="sxs-lookup"><span data-stu-id="ced4b-126">description</span></span>|<span data-ttu-id="ced4b-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ced4b-127">String</span></span>|<span data-ttu-id="ced4b-128">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="ced4b-128">The policy's description.</span></span> <span data-ttu-id="ced4b-129">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ced4b-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ced4b-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ced4b-130">createdDateTime</span></span>|<span data-ttu-id="ced4b-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ced4b-131">DateTimeOffset</span></span>|<span data-ttu-id="ced4b-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="ced4b-132">The date and time the policy was created.</span></span> <span data-ttu-id="ced4b-133">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ced4b-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ced4b-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ced4b-134">lastModifiedDateTime</span></span>|<span data-ttu-id="ced4b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ced4b-135">DateTimeOffset</span></span>|<span data-ttu-id="ced4b-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="ced4b-136">Last time the policy was modified.</span></span> <span data-ttu-id="ced4b-137">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ced4b-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ced4b-138">id</span><span class="sxs-lookup"><span data-stu-id="ced4b-138">id</span></span>|<span data-ttu-id="ced4b-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ced4b-139">String</span></span>|<span data-ttu-id="ced4b-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ced4b-140">Key of the entity.</span></span> <span data-ttu-id="ced4b-141">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ced4b-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ced4b-142">version</span><span class="sxs-lookup"><span data-stu-id="ced4b-142">version</span></span>|<span data-ttu-id="ced4b-143">String</span><span class="sxs-lookup"><span data-stu-id="ced4b-143">String</span></span>|<span data-ttu-id="ced4b-144">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="ced4b-144">Version of the entity.</span></span> <span data-ttu-id="ced4b-145">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ced4b-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ced4b-146">customSettings</span><span class="sxs-lookup"><span data-stu-id="ced4b-146">customSettings</span></span>|<span data-ttu-id="ced4b-147">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ced4b-147">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ced4b-148">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="ced4b-148">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="ced4b-149">Relações</span><span class="sxs-lookup"><span data-stu-id="ced4b-149">Relationships</span></span>
<span data-ttu-id="ced4b-150">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ced4b-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ced4b-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ced4b-151">JSON Representation</span></span>
<span data-ttu-id="ced4b-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ced4b-152">Here is a JSON representation of the resource.</span></span>
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




