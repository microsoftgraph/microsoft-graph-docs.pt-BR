---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 557a314893faeb268ae21d13ec78a46bff9d6e0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809636"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="4b427-103">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b427-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="4b427-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4b427-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b427-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4b427-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b427-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4b427-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b427-107">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="4b427-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="4b427-108">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4b427-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="4b427-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="4b427-109">Methods</span></span>
|<span data-ttu-id="4b427-110">Método</span><span class="sxs-lookup"><span data-stu-id="4b427-110">Method</span></span>|<span data-ttu-id="4b427-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4b427-111">Return Type</span></span>|<span data-ttu-id="4b427-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b427-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b427-113">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="4b427-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="4b427-114">Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b427-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="4b427-115">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b427-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="4b427-116">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b427-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="4b427-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b427-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="4b427-118">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b427-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b427-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b427-119">Properties</span></span>
|<span data-ttu-id="4b427-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b427-120">Property</span></span>|<span data-ttu-id="4b427-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b427-121">Type</span></span>|<span data-ttu-id="4b427-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b427-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b427-123">displayName</span><span class="sxs-lookup"><span data-stu-id="4b427-123">displayName</span></span>|<span data-ttu-id="4b427-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b427-124">String</span></span>|<span data-ttu-id="4b427-125">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="4b427-125">Policy display name.</span></span> <span data-ttu-id="4b427-126">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4b427-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4b427-127">description</span><span class="sxs-lookup"><span data-stu-id="4b427-127">description</span></span>|<span data-ttu-id="4b427-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b427-128">String</span></span>|<span data-ttu-id="4b427-129">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="4b427-129">The policy's description.</span></span> <span data-ttu-id="4b427-130">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4b427-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4b427-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b427-131">createdDateTime</span></span>|<span data-ttu-id="4b427-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b427-132">DateTimeOffset</span></span>|<span data-ttu-id="4b427-133">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="4b427-133">The date and time the policy was created.</span></span> <span data-ttu-id="4b427-134">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4b427-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4b427-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b427-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4b427-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b427-136">DateTimeOffset</span></span>|<span data-ttu-id="4b427-137">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="4b427-137">Last time the policy was modified.</span></span> <span data-ttu-id="4b427-138">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4b427-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4b427-139">id</span><span class="sxs-lookup"><span data-stu-id="4b427-139">id</span></span>|<span data-ttu-id="4b427-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b427-140">String</span></span>|<span data-ttu-id="4b427-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4b427-141">Key of the entity.</span></span> <span data-ttu-id="4b427-142">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4b427-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4b427-143">version</span><span class="sxs-lookup"><span data-stu-id="4b427-143">version</span></span>|<span data-ttu-id="4b427-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b427-144">String</span></span>|<span data-ttu-id="4b427-145">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="4b427-145">Version of the entity.</span></span> <span data-ttu-id="4b427-146">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4b427-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4b427-147">customSettings</span><span class="sxs-lookup"><span data-stu-id="4b427-147">customSettings</span></span>|<span data-ttu-id="4b427-148">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4b427-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4b427-149">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="4b427-149">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b427-150">Relações</span><span class="sxs-lookup"><span data-stu-id="4b427-150">Relationships</span></span>
<span data-ttu-id="4b427-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b427-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b427-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b427-152">JSON Representation</span></span>
<span data-ttu-id="4b427-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b427-153">Here is a JSON representation of the resource.</span></span>
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





