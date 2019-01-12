---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2bf4e8ce0d32bea7714ae489167dbb582043fa5a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936631"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="fde63-103">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fde63-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="fde63-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fde63-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fde63-105">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="fde63-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="fde63-106">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fde63-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="fde63-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fde63-107">Methods</span></span>
|<span data-ttu-id="fde63-108">Método</span><span class="sxs-lookup"><span data-stu-id="fde63-108">Method</span></span>|<span data-ttu-id="fde63-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fde63-109">Return Type</span></span>|<span data-ttu-id="fde63-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fde63-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fde63-111">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="fde63-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="fde63-112">Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fde63-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="fde63-113">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fde63-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="fde63-114">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fde63-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="fde63-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fde63-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="fde63-116">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fde63-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fde63-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fde63-117">Properties</span></span>
|<span data-ttu-id="fde63-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fde63-118">Property</span></span>|<span data-ttu-id="fde63-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fde63-119">Type</span></span>|<span data-ttu-id="fde63-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fde63-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fde63-121">displayName</span><span class="sxs-lookup"><span data-stu-id="fde63-121">displayName</span></span>|<span data-ttu-id="fde63-122">String</span><span class="sxs-lookup"><span data-stu-id="fde63-122">String</span></span>|<span data-ttu-id="fde63-123">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="fde63-123">Policy display name.</span></span> <span data-ttu-id="fde63-124">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fde63-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fde63-125">description</span><span class="sxs-lookup"><span data-stu-id="fde63-125">description</span></span>|<span data-ttu-id="fde63-126">String</span><span class="sxs-lookup"><span data-stu-id="fde63-126">String</span></span>|<span data-ttu-id="fde63-127">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="fde63-127">The policy's description.</span></span> <span data-ttu-id="fde63-128">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fde63-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fde63-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fde63-129">createdDateTime</span></span>|<span data-ttu-id="fde63-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fde63-130">DateTimeOffset</span></span>|<span data-ttu-id="fde63-131">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="fde63-131">The date and time the policy was created.</span></span> <span data-ttu-id="fde63-132">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fde63-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fde63-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fde63-133">lastModifiedDateTime</span></span>|<span data-ttu-id="fde63-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fde63-134">DateTimeOffset</span></span>|<span data-ttu-id="fde63-135">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="fde63-135">Last time the policy was modified.</span></span> <span data-ttu-id="fde63-136">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fde63-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fde63-137">id</span><span class="sxs-lookup"><span data-stu-id="fde63-137">id</span></span>|<span data-ttu-id="fde63-138">String</span><span class="sxs-lookup"><span data-stu-id="fde63-138">String</span></span>|<span data-ttu-id="fde63-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fde63-139">Key of the entity.</span></span> <span data-ttu-id="fde63-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fde63-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fde63-141">version</span><span class="sxs-lookup"><span data-stu-id="fde63-141">version</span></span>|<span data-ttu-id="fde63-142">String</span><span class="sxs-lookup"><span data-stu-id="fde63-142">String</span></span>|<span data-ttu-id="fde63-143">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="fde63-143">Version of the entity.</span></span> <span data-ttu-id="fde63-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fde63-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="fde63-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="fde63-145">customSettings</span></span>|<span data-ttu-id="fde63-146">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="fde63-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="fde63-147">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="fde63-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="fde63-148">Relações</span><span class="sxs-lookup"><span data-stu-id="fde63-148">Relationships</span></span>
<span data-ttu-id="fde63-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fde63-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fde63-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fde63-150">JSON Representation</span></span>
<span data-ttu-id="fde63-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fde63-151">Here is a JSON representation of the resource.</span></span>
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



