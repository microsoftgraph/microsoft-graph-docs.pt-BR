---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c52ade795ff98d809d4013babdb6aae37c8106d9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787292"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="914fe-103">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="914fe-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="914fe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="914fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="914fe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="914fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="914fe-106">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="914fe-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="914fe-107">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="914fe-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="914fe-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="914fe-108">Methods</span></span>
|<span data-ttu-id="914fe-109">Método</span><span class="sxs-lookup"><span data-stu-id="914fe-109">Method</span></span>|<span data-ttu-id="914fe-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="914fe-110">Return Type</span></span>|<span data-ttu-id="914fe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="914fe-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="914fe-112">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="914fe-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="914fe-113">Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="914fe-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="914fe-114">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914fe-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="914fe-115">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="914fe-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="914fe-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="914fe-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="914fe-117">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="914fe-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="914fe-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="914fe-118">Properties</span></span>
|<span data-ttu-id="914fe-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="914fe-119">Property</span></span>|<span data-ttu-id="914fe-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="914fe-120">Type</span></span>|<span data-ttu-id="914fe-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="914fe-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="914fe-122">displayName</span><span class="sxs-lookup"><span data-stu-id="914fe-122">displayName</span></span>|<span data-ttu-id="914fe-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="914fe-123">String</span></span>|<span data-ttu-id="914fe-124">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="914fe-124">Policy display name.</span></span> <span data-ttu-id="914fe-125">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="914fe-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="914fe-126">description</span><span class="sxs-lookup"><span data-stu-id="914fe-126">description</span></span>|<span data-ttu-id="914fe-127">String</span><span class="sxs-lookup"><span data-stu-id="914fe-127">String</span></span>|<span data-ttu-id="914fe-128">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="914fe-128">The policy's description.</span></span> <span data-ttu-id="914fe-129">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="914fe-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="914fe-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="914fe-130">createdDateTime</span></span>|<span data-ttu-id="914fe-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914fe-131">DateTimeOffset</span></span>|<span data-ttu-id="914fe-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="914fe-132">The date and time the policy was created.</span></span> <span data-ttu-id="914fe-133">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="914fe-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="914fe-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="914fe-134">lastModifiedDateTime</span></span>|<span data-ttu-id="914fe-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914fe-135">DateTimeOffset</span></span>|<span data-ttu-id="914fe-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="914fe-136">Last time the policy was modified.</span></span> <span data-ttu-id="914fe-137">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="914fe-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="914fe-138">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="914fe-138">roleScopeTagIds</span></span>|<span data-ttu-id="914fe-139">Coleção String</span><span class="sxs-lookup"><span data-stu-id="914fe-139">String collection</span></span>|<span data-ttu-id="914fe-140">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="914fe-140">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="914fe-141">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="914fe-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="914fe-142">id</span><span class="sxs-lookup"><span data-stu-id="914fe-142">id</span></span>|<span data-ttu-id="914fe-143">String</span><span class="sxs-lookup"><span data-stu-id="914fe-143">String</span></span>|<span data-ttu-id="914fe-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="914fe-144">Key of the entity.</span></span> <span data-ttu-id="914fe-145">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="914fe-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="914fe-146">version</span><span class="sxs-lookup"><span data-stu-id="914fe-146">version</span></span>|<span data-ttu-id="914fe-147">String</span><span class="sxs-lookup"><span data-stu-id="914fe-147">String</span></span>|<span data-ttu-id="914fe-148">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="914fe-148">Version of the entity.</span></span> <span data-ttu-id="914fe-149">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="914fe-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="914fe-150">customSettings</span><span class="sxs-lookup"><span data-stu-id="914fe-150">customSettings</span></span>|<span data-ttu-id="914fe-151">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="914fe-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="914fe-152">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="914fe-152">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="914fe-153">Relações</span><span class="sxs-lookup"><span data-stu-id="914fe-153">Relationships</span></span>
<span data-ttu-id="914fe-154">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="914fe-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="914fe-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="914fe-155">JSON Representation</span></span>
<span data-ttu-id="914fe-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="914fe-156">Here is a JSON representation of the resource.</span></span>
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





