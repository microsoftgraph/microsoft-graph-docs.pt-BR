---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60ee8156773db386d5ad8496bf037984005dc5bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448428"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="1949f-103">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1949f-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="1949f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1949f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1949f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1949f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1949f-106">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="1949f-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="1949f-107">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1949f-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1949f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="1949f-108">Methods</span></span>
|<span data-ttu-id="1949f-109">Método</span><span class="sxs-lookup"><span data-stu-id="1949f-109">Method</span></span>|<span data-ttu-id="1949f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1949f-110">Return Type</span></span>|<span data-ttu-id="1949f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1949f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1949f-112">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="1949f-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="1949f-113">Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1949f-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="1949f-114">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1949f-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1949f-115">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1949f-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="1949f-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1949f-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="1949f-117">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1949f-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1949f-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1949f-118">Properties</span></span>
|<span data-ttu-id="1949f-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1949f-119">Property</span></span>|<span data-ttu-id="1949f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1949f-120">Type</span></span>|<span data-ttu-id="1949f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1949f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1949f-122">displayName</span><span class="sxs-lookup"><span data-stu-id="1949f-122">displayName</span></span>|<span data-ttu-id="1949f-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1949f-123">String</span></span>|<span data-ttu-id="1949f-124">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="1949f-124">Policy display name.</span></span> <span data-ttu-id="1949f-125">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1949f-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1949f-126">description</span><span class="sxs-lookup"><span data-stu-id="1949f-126">description</span></span>|<span data-ttu-id="1949f-127">String</span><span class="sxs-lookup"><span data-stu-id="1949f-127">String</span></span>|<span data-ttu-id="1949f-128">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="1949f-128">The policy's description.</span></span> <span data-ttu-id="1949f-129">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1949f-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1949f-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1949f-130">createdDateTime</span></span>|<span data-ttu-id="1949f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1949f-131">DateTimeOffset</span></span>|<span data-ttu-id="1949f-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="1949f-132">The date and time the policy was created.</span></span> <span data-ttu-id="1949f-133">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1949f-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1949f-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1949f-134">lastModifiedDateTime</span></span>|<span data-ttu-id="1949f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1949f-135">DateTimeOffset</span></span>|<span data-ttu-id="1949f-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="1949f-136">Last time the policy was modified.</span></span> <span data-ttu-id="1949f-137">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1949f-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1949f-138">id</span><span class="sxs-lookup"><span data-stu-id="1949f-138">id</span></span>|<span data-ttu-id="1949f-139">String</span><span class="sxs-lookup"><span data-stu-id="1949f-139">String</span></span>|<span data-ttu-id="1949f-140">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1949f-140">Key of the entity.</span></span> <span data-ttu-id="1949f-141">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1949f-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1949f-142">version</span><span class="sxs-lookup"><span data-stu-id="1949f-142">version</span></span>|<span data-ttu-id="1949f-143">String</span><span class="sxs-lookup"><span data-stu-id="1949f-143">String</span></span>|<span data-ttu-id="1949f-144">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="1949f-144">Version of the entity.</span></span> <span data-ttu-id="1949f-145">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1949f-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1949f-146">customSettings</span><span class="sxs-lookup"><span data-stu-id="1949f-146">customSettings</span></span>|<span data-ttu-id="1949f-147">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1949f-147">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="1949f-148">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="1949f-148">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="1949f-149">Relações</span><span class="sxs-lookup"><span data-stu-id="1949f-149">Relationships</span></span>
<span data-ttu-id="1949f-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1949f-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1949f-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1949f-151">JSON Representation</span></span>
<span data-ttu-id="1949f-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1949f-152">Here is a JSON representation of the resource.</span></span>
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




