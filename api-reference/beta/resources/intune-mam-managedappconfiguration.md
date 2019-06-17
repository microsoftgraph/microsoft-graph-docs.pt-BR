---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8d6fd389ef632aa1606fa8af070a0e83faf1d1b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991958"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="f500f-103">Tipo de recurso managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f500f-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="f500f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f500f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f500f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f500f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f500f-106">Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido</span><span class="sxs-lookup"><span data-stu-id="f500f-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="f500f-107">Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f500f-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f500f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f500f-108">Methods</span></span>
|<span data-ttu-id="f500f-109">Método</span><span class="sxs-lookup"><span data-stu-id="f500f-109">Method</span></span>|<span data-ttu-id="f500f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f500f-110">Return Type</span></span>|<span data-ttu-id="f500f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f500f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f500f-112">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="f500f-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="f500f-113">Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f500f-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="f500f-114">Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f500f-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f500f-115">Obter managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f500f-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="f500f-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f500f-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="f500f-117">Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f500f-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f500f-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f500f-118">Properties</span></span>
|<span data-ttu-id="f500f-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f500f-119">Property</span></span>|<span data-ttu-id="f500f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f500f-120">Type</span></span>|<span data-ttu-id="f500f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f500f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f500f-122">displayName</span><span class="sxs-lookup"><span data-stu-id="f500f-122">displayName</span></span>|<span data-ttu-id="f500f-123">String</span><span class="sxs-lookup"><span data-stu-id="f500f-123">String</span></span>|<span data-ttu-id="f500f-124">Nome para exibição da política.</span><span class="sxs-lookup"><span data-stu-id="f500f-124">Policy display name.</span></span> <span data-ttu-id="f500f-125">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f500f-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f500f-126">descrição</span><span class="sxs-lookup"><span data-stu-id="f500f-126">description</span></span>|<span data-ttu-id="f500f-127">String</span><span class="sxs-lookup"><span data-stu-id="f500f-127">String</span></span>|<span data-ttu-id="f500f-128">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="f500f-128">The policy's description.</span></span> <span data-ttu-id="f500f-129">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f500f-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f500f-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f500f-130">createdDateTime</span></span>|<span data-ttu-id="f500f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f500f-131">DateTimeOffset</span></span>|<span data-ttu-id="f500f-132">A data e a hora da criação da política.</span><span class="sxs-lookup"><span data-stu-id="f500f-132">The date and time the policy was created.</span></span> <span data-ttu-id="f500f-133">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f500f-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f500f-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f500f-134">lastModifiedDateTime</span></span>|<span data-ttu-id="f500f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f500f-135">DateTimeOffset</span></span>|<span data-ttu-id="f500f-136">Última vez em que a política foi modificada.</span><span class="sxs-lookup"><span data-stu-id="f500f-136">Last time the policy was modified.</span></span> <span data-ttu-id="f500f-137">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f500f-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f500f-138">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f500f-138">roleScopeTagIds</span></span>|<span data-ttu-id="f500f-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f500f-139">String collection</span></span>|<span data-ttu-id="f500f-140">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f500f-140">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f500f-141">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f500f-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f500f-142">id</span><span class="sxs-lookup"><span data-stu-id="f500f-142">id</span></span>|<span data-ttu-id="f500f-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f500f-143">String</span></span>|<span data-ttu-id="f500f-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f500f-144">Key of the entity.</span></span> <span data-ttu-id="f500f-145">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f500f-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f500f-146">version</span><span class="sxs-lookup"><span data-stu-id="f500f-146">version</span></span>|<span data-ttu-id="f500f-147">String</span><span class="sxs-lookup"><span data-stu-id="f500f-147">String</span></span>|<span data-ttu-id="f500f-148">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="f500f-148">Version of the entity.</span></span> <span data-ttu-id="f500f-149">Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f500f-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f500f-150">customSettings</span><span class="sxs-lookup"><span data-stu-id="f500f-150">customSettings</span></span>|<span data-ttu-id="f500f-151">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f500f-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f500f-152">Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço</span><span class="sxs-lookup"><span data-stu-id="f500f-152">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="f500f-153">Relações</span><span class="sxs-lookup"><span data-stu-id="f500f-153">Relationships</span></span>
<span data-ttu-id="f500f-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f500f-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f500f-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f500f-155">JSON Representation</span></span>
<span data-ttu-id="f500f-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f500f-156">Here is a JSON representation of the resource.</span></span>
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





