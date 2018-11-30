---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
ms.openlocfilehash: 42544aeacda4494a7757a15bef75a493d96fe0cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007324"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="ec1a7-103">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec1a7-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="ec1a7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ec1a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec1a7-105">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="ec1a7-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="ec1a7-106">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ec1a7-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ec1a7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ec1a7-107">Methods</span></span>
|<span data-ttu-id="ec1a7-108">Método</span><span class="sxs-lookup"><span data-stu-id="ec1a7-108">Method</span></span>|<span data-ttu-id="ec1a7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ec1a7-109">Return Type</span></span>|<span data-ttu-id="ec1a7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec1a7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ec1a7-111">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="ec1a7-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="ec1a7-112">Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec1a7-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="ec1a7-113">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec1a7-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ec1a7-114">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec1a7-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="ec1a7-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec1a7-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="ec1a7-116">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec1a7-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ec1a7-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec1a7-117">Properties</span></span>
|<span data-ttu-id="ec1a7-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec1a7-118">Property</span></span>|<span data-ttu-id="ec1a7-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec1a7-119">Type</span></span>|<span data-ttu-id="ec1a7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec1a7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec1a7-121">displayName</span><span class="sxs-lookup"><span data-stu-id="ec1a7-121">displayName</span></span>|<span data-ttu-id="ec1a7-122">String</span><span class="sxs-lookup"><span data-stu-id="ec1a7-122">String</span></span>|<span data-ttu-id="ec1a7-123">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="ec1a7-123">Policy display name.</span></span> <span data-ttu-id="ec1a7-124">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ec1a7-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ec1a7-125">description</span><span class="sxs-lookup"><span data-stu-id="ec1a7-125">description</span></span>|<span data-ttu-id="ec1a7-126">String</span><span class="sxs-lookup"><span data-stu-id="ec1a7-126">String</span></span>|<span data-ttu-id="ec1a7-127">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="ec1a7-127">The policy's description.</span></span> <span data-ttu-id="ec1a7-128">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ec1a7-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ec1a7-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec1a7-129">createdDateTime</span></span>|<span data-ttu-id="ec1a7-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec1a7-130">DateTimeOffset</span></span>|<span data-ttu-id="ec1a7-131">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="ec1a7-131">The date and time the policy was created.</span></span> <span data-ttu-id="ec1a7-132">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ec1a7-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ec1a7-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec1a7-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ec1a7-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec1a7-134">DateTimeOffset</span></span>|<span data-ttu-id="ec1a7-135">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="ec1a7-135">Last time the policy was modified.</span></span> <span data-ttu-id="ec1a7-136">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ec1a7-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ec1a7-137">id</span><span class="sxs-lookup"><span data-stu-id="ec1a7-137">id</span></span>|<span data-ttu-id="ec1a7-138">String</span><span class="sxs-lookup"><span data-stu-id="ec1a7-138">String</span></span>|<span data-ttu-id="ec1a7-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ec1a7-139">Key of the entity.</span></span> <span data-ttu-id="ec1a7-140">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ec1a7-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ec1a7-141">version</span><span class="sxs-lookup"><span data-stu-id="ec1a7-141">version</span></span>|<span data-ttu-id="ec1a7-142">String</span><span class="sxs-lookup"><span data-stu-id="ec1a7-142">String</span></span>|<span data-ttu-id="ec1a7-143">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="ec1a7-143">Version of the entity.</span></span> <span data-ttu-id="ec1a7-144">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ec1a7-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ec1a7-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="ec1a7-145">customSettings</span></span>|<span data-ttu-id="ec1a7-146">Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ec1a7-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ec1a7-147">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="ec1a7-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec1a7-148">Relações</span><span class="sxs-lookup"><span data-stu-id="ec1a7-148">Relationships</span></span>
<span data-ttu-id="ec1a7-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec1a7-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ec1a7-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec1a7-150">JSON Representation</span></span>
<span data-ttu-id="ec1a7-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec1a7-151">Here is a JSON representation of the resource.</span></span>
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



