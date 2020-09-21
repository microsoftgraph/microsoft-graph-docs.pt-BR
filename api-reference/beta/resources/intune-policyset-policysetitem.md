---
title: tipo de recurso policySetItem
description: Uma classe que contém as propriedades usadas para o item Policyset.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 530dd10960eacd0ded5c5c8d9340469c66020e8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993410"
---
# <a name="policysetitem-resource-type"></a><span data-ttu-id="33728-103">tipo de recurso policySetItem</span><span class="sxs-lookup"><span data-stu-id="33728-103">policySetItem resource type</span></span>

<span data-ttu-id="33728-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33728-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33728-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33728-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33728-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33728-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33728-107">Uma classe que contém as propriedades usadas para o item Policyset.</span><span class="sxs-lookup"><span data-stu-id="33728-107">A class containing the properties used for PolicySet Item.</span></span>

## <a name="methods"></a><span data-ttu-id="33728-108">Methods</span><span class="sxs-lookup"><span data-stu-id="33728-108">Methods</span></span>
|<span data-ttu-id="33728-109">Método</span><span class="sxs-lookup"><span data-stu-id="33728-109">Method</span></span>|<span data-ttu-id="33728-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="33728-110">Return Type</span></span>|<span data-ttu-id="33728-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="33728-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="33728-112">Listar policySetItems</span><span class="sxs-lookup"><span data-stu-id="33728-112">List policySetItems</span></span>](../api/intune-policyset-policysetitem-list.md)|<span data-ttu-id="33728-113">coleção [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="33728-113">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="33728-114">Listar Propriedades e relações dos objetos [policySetItem](../resources/intune-policyset-policysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="33728-114">List properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) objects.</span></span>|
|[<span data-ttu-id="33728-115">Obter policySetItem</span><span class="sxs-lookup"><span data-stu-id="33728-115">Get policySetItem</span></span>](../api/intune-policyset-policysetitem-get.md)|[<span data-ttu-id="33728-116">policySetItem</span><span class="sxs-lookup"><span data-stu-id="33728-116">policySetItem</span></span>](../resources/intune-policyset-policysetitem.md)|<span data-ttu-id="33728-117">Leia as propriedades e as relações do objeto [policySetItem](../resources/intune-policyset-policysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="33728-117">Read properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="33728-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33728-118">Properties</span></span>
|<span data-ttu-id="33728-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33728-119">Property</span></span>|<span data-ttu-id="33728-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="33728-120">Type</span></span>|<span data-ttu-id="33728-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="33728-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33728-122">id</span><span class="sxs-lookup"><span data-stu-id="33728-122">id</span></span>|<span data-ttu-id="33728-123">String</span><span class="sxs-lookup"><span data-stu-id="33728-123">String</span></span>|<span data-ttu-id="33728-124">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="33728-124">Key of the MobileAppPolicySetItem.</span></span>|
|<span data-ttu-id="33728-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33728-125">createdDateTime</span></span>|<span data-ttu-id="33728-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33728-126">DateTimeOffset</span></span>|<span data-ttu-id="33728-127">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="33728-127">Creation time of the PolicySetItem.</span></span>|
|<span data-ttu-id="33728-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33728-128">lastModifiedDateTime</span></span>|<span data-ttu-id="33728-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33728-129">DateTimeOffset</span></span>|<span data-ttu-id="33728-130">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="33728-130">Last modified time of the PolicySetItem.</span></span>|
|<span data-ttu-id="33728-131">payloadId</span><span class="sxs-lookup"><span data-stu-id="33728-131">payloadId</span></span>|<span data-ttu-id="33728-132">String</span><span class="sxs-lookup"><span data-stu-id="33728-132">String</span></span>|<span data-ttu-id="33728-133">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="33728-133">PayloadId of the PolicySetItem.</span></span>|
|<span data-ttu-id="33728-134">itemType</span><span class="sxs-lookup"><span data-stu-id="33728-134">itemType</span></span>|<span data-ttu-id="33728-135">String</span><span class="sxs-lookup"><span data-stu-id="33728-135">String</span></span>|<span data-ttu-id="33728-136">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="33728-136">policySetType of the PolicySetItem.</span></span>|
|<span data-ttu-id="33728-137">displayName</span><span class="sxs-lookup"><span data-stu-id="33728-137">displayName</span></span>|<span data-ttu-id="33728-138">String</span><span class="sxs-lookup"><span data-stu-id="33728-138">String</span></span>|<span data-ttu-id="33728-139">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="33728-139">DisplayName of the PolicySetItem.</span></span>|
|<span data-ttu-id="33728-140">status</span><span class="sxs-lookup"><span data-stu-id="33728-140">status</span></span>|[<span data-ttu-id="33728-141">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="33728-141">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="33728-142">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="33728-142">Status of the PolicySetItem.</span></span> <span data-ttu-id="33728-143">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="33728-143">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="33728-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="33728-144">errorCode</span></span>|[<span data-ttu-id="33728-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="33728-145">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="33728-146">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="33728-146">Error code if any occured.</span></span> <span data-ttu-id="33728-147">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="33728-147">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="33728-148">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="33728-148">guidedDeploymentTags</span></span>|<span data-ttu-id="33728-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="33728-149">String collection</span></span>|<span data-ttu-id="33728-150">Marcas da implantação dirigida</span><span class="sxs-lookup"><span data-stu-id="33728-150">Tags of the guided deployment</span></span>|

## <a name="relationships"></a><span data-ttu-id="33728-151">Relações</span><span class="sxs-lookup"><span data-stu-id="33728-151">Relationships</span></span>
<span data-ttu-id="33728-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33728-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33728-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33728-153">JSON Representation</span></span>
<span data-ttu-id="33728-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33728-154">Here is a JSON representation of the resource.</span></span>
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






