---
title: tipo de recurso policySetItem
description: Uma classe que contém as propriedades usadas para o item Policyset.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df5cdc970696db9785c19c0a6c5afb5ab2266f7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523975"
---
# <a name="policysetitem-resource-type"></a><span data-ttu-id="57b0e-103">tipo de recurso policySetItem</span><span class="sxs-lookup"><span data-stu-id="57b0e-103">policySetItem resource type</span></span>

<span data-ttu-id="57b0e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="57b0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57b0e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57b0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57b0e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57b0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57b0e-107">Uma classe que contém as propriedades usadas para o item Policyset.</span><span class="sxs-lookup"><span data-stu-id="57b0e-107">A class containing the properties used for PolicySet Item.</span></span>

## <a name="methods"></a><span data-ttu-id="57b0e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="57b0e-108">Methods</span></span>
|<span data-ttu-id="57b0e-109">Método</span><span class="sxs-lookup"><span data-stu-id="57b0e-109">Method</span></span>|<span data-ttu-id="57b0e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="57b0e-110">Return Type</span></span>|<span data-ttu-id="57b0e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="57b0e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="57b0e-112">Listar policySetItems</span><span class="sxs-lookup"><span data-stu-id="57b0e-112">List policySetItems</span></span>](../api/intune-policyset-policysetitem-list.md)|<span data-ttu-id="57b0e-113">coleção [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="57b0e-113">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="57b0e-114">Listar Propriedades e relações dos objetos [policySetItem](../resources/intune-policyset-policysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="57b0e-114">List properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) objects.</span></span>|
|[<span data-ttu-id="57b0e-115">Obter policySetItem</span><span class="sxs-lookup"><span data-stu-id="57b0e-115">Get policySetItem</span></span>](../api/intune-policyset-policysetitem-get.md)|[<span data-ttu-id="57b0e-116">policySetItem</span><span class="sxs-lookup"><span data-stu-id="57b0e-116">policySetItem</span></span>](../resources/intune-policyset-policysetitem.md)|<span data-ttu-id="57b0e-117">Leia as propriedades e as relações do objeto [policySetItem](../resources/intune-policyset-policysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="57b0e-117">Read properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="57b0e-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57b0e-118">Properties</span></span>
|<span data-ttu-id="57b0e-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57b0e-119">Property</span></span>|<span data-ttu-id="57b0e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="57b0e-120">Type</span></span>|<span data-ttu-id="57b0e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="57b0e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57b0e-122">id</span><span class="sxs-lookup"><span data-stu-id="57b0e-122">id</span></span>|<span data-ttu-id="57b0e-123">String</span><span class="sxs-lookup"><span data-stu-id="57b0e-123">String</span></span>|<span data-ttu-id="57b0e-124">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="57b0e-124">Key of the MobileAppPolicySetItem.</span></span>|
|<span data-ttu-id="57b0e-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57b0e-125">createdDateTime</span></span>|<span data-ttu-id="57b0e-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57b0e-126">DateTimeOffset</span></span>|<span data-ttu-id="57b0e-127">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="57b0e-127">Creation time of the PolicySetItem.</span></span>|
|<span data-ttu-id="57b0e-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57b0e-128">lastModifiedDateTime</span></span>|<span data-ttu-id="57b0e-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57b0e-129">DateTimeOffset</span></span>|<span data-ttu-id="57b0e-130">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="57b0e-130">Last modified time of the PolicySetItem.</span></span>|
|<span data-ttu-id="57b0e-131">payloadId</span><span class="sxs-lookup"><span data-stu-id="57b0e-131">payloadId</span></span>|<span data-ttu-id="57b0e-132">String</span><span class="sxs-lookup"><span data-stu-id="57b0e-132">String</span></span>|<span data-ttu-id="57b0e-133">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="57b0e-133">PayloadId of the PolicySetItem.</span></span>|
|<span data-ttu-id="57b0e-134">itemType</span><span class="sxs-lookup"><span data-stu-id="57b0e-134">itemType</span></span>|<span data-ttu-id="57b0e-135">String</span><span class="sxs-lookup"><span data-stu-id="57b0e-135">String</span></span>|<span data-ttu-id="57b0e-136">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="57b0e-136">policySetType of the PolicySetItem.</span></span>|
|<span data-ttu-id="57b0e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="57b0e-137">displayName</span></span>|<span data-ttu-id="57b0e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57b0e-138">String</span></span>|<span data-ttu-id="57b0e-139">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="57b0e-139">DisplayName of the PolicySetItem.</span></span>|
|<span data-ttu-id="57b0e-140">status</span><span class="sxs-lookup"><span data-stu-id="57b0e-140">status</span></span>|[<span data-ttu-id="57b0e-141">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="57b0e-141">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="57b0e-142">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="57b0e-142">Status of the PolicySetItem.</span></span> <span data-ttu-id="57b0e-143">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="57b0e-143">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="57b0e-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="57b0e-144">errorCode</span></span>|[<span data-ttu-id="57b0e-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="57b0e-145">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="57b0e-146">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="57b0e-146">Error code if any occured.</span></span> <span data-ttu-id="57b0e-147">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="57b0e-147">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="57b0e-148">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="57b0e-148">guidedDeploymentTags</span></span>|<span data-ttu-id="57b0e-149">String collection</span><span class="sxs-lookup"><span data-stu-id="57b0e-149">String collection</span></span>|<span data-ttu-id="57b0e-150">Marcas da implantação dirigida</span><span class="sxs-lookup"><span data-stu-id="57b0e-150">Tags of the guided deployment</span></span>|

## <a name="relationships"></a><span data-ttu-id="57b0e-151">Relações</span><span class="sxs-lookup"><span data-stu-id="57b0e-151">Relationships</span></span>
<span data-ttu-id="57b0e-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57b0e-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57b0e-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57b0e-153">JSON Representation</span></span>
<span data-ttu-id="57b0e-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57b0e-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```



