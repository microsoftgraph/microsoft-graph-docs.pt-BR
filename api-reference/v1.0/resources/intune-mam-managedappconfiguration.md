---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86c6ecdcad64ae38887370101f96106a9b3aa816
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250765"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="80901-103">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="80901-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="80901-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80901-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80901-105">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="80901-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="80901-106">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="80901-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="80901-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="80901-107">Methods</span></span>
|<span data-ttu-id="80901-108">Método</span><span class="sxs-lookup"><span data-stu-id="80901-108">Method</span></span>|<span data-ttu-id="80901-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="80901-109">Return Type</span></span>|<span data-ttu-id="80901-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="80901-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="80901-111">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="80901-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="80901-112">Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80901-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="80901-113">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80901-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="80901-114">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="80901-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="80901-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="80901-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="80901-116">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80901-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="80901-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80901-117">Properties</span></span>
|<span data-ttu-id="80901-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80901-118">Property</span></span>|<span data-ttu-id="80901-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="80901-119">Type</span></span>|<span data-ttu-id="80901-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="80901-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80901-121">displayName</span><span class="sxs-lookup"><span data-stu-id="80901-121">displayName</span></span>|<span data-ttu-id="80901-122">String</span><span class="sxs-lookup"><span data-stu-id="80901-122">String</span></span>|<span data-ttu-id="80901-123">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="80901-123">Policy display name.</span></span> <span data-ttu-id="80901-124">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="80901-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="80901-125">descrição</span><span class="sxs-lookup"><span data-stu-id="80901-125">description</span></span>|<span data-ttu-id="80901-126">String</span><span class="sxs-lookup"><span data-stu-id="80901-126">String</span></span>|<span data-ttu-id="80901-127">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="80901-127">The policy's description.</span></span> <span data-ttu-id="80901-128">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="80901-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="80901-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80901-129">createdDateTime</span></span>|<span data-ttu-id="80901-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80901-130">DateTimeOffset</span></span>|<span data-ttu-id="80901-131">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="80901-131">The date and time the policy was created.</span></span> <span data-ttu-id="80901-132">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="80901-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="80901-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80901-133">lastModifiedDateTime</span></span>|<span data-ttu-id="80901-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80901-134">DateTimeOffset</span></span>|<span data-ttu-id="80901-135">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="80901-135">Last time the policy was modified.</span></span> <span data-ttu-id="80901-136">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="80901-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="80901-137">id</span><span class="sxs-lookup"><span data-stu-id="80901-137">id</span></span>|<span data-ttu-id="80901-138">String</span><span class="sxs-lookup"><span data-stu-id="80901-138">String</span></span>|<span data-ttu-id="80901-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="80901-139">Key of the entity.</span></span> <span data-ttu-id="80901-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="80901-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="80901-141">version</span><span class="sxs-lookup"><span data-stu-id="80901-141">version</span></span>|<span data-ttu-id="80901-142">String</span><span class="sxs-lookup"><span data-stu-id="80901-142">String</span></span>|<span data-ttu-id="80901-143">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="80901-143">Version of the entity.</span></span> <span data-ttu-id="80901-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="80901-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="80901-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="80901-145">customSettings</span></span>|<span data-ttu-id="80901-146">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="80901-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="80901-147">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="80901-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="80901-148">Relações</span><span class="sxs-lookup"><span data-stu-id="80901-148">Relationships</span></span>
<span data-ttu-id="80901-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80901-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80901-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80901-150">JSON Representation</span></span>
<span data-ttu-id="80901-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80901-151">Here is a JSON representation of the resource.</span></span>
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



