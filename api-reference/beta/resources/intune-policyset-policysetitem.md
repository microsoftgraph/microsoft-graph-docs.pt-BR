---
title: tipo de recurso policySetItem
description: Uma classe que contém as propriedades usadas para o item Policyset.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 77438e4b0322dcb6feade0aab57c830869832e14
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287925"
---
# <a name="policysetitem-resource-type"></a><span data-ttu-id="b174a-103">tipo de recurso policySetItem</span><span class="sxs-lookup"><span data-stu-id="b174a-103">policySetItem resource type</span></span>

<span data-ttu-id="b174a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b174a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b174a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b174a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b174a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b174a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b174a-107">Uma classe que contém as propriedades usadas para o item Policyset.</span><span class="sxs-lookup"><span data-stu-id="b174a-107">A class containing the properties used for PolicySet Item.</span></span>

## <a name="methods"></a><span data-ttu-id="b174a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b174a-108">Methods</span></span>
|<span data-ttu-id="b174a-109">Método</span><span class="sxs-lookup"><span data-stu-id="b174a-109">Method</span></span>|<span data-ttu-id="b174a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b174a-110">Return Type</span></span>|<span data-ttu-id="b174a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b174a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b174a-112">Listar policySetItems</span><span class="sxs-lookup"><span data-stu-id="b174a-112">List policySetItems</span></span>](../api/intune-policyset-policysetitem-list.md)|<span data-ttu-id="b174a-113">coleção [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="b174a-113">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="b174a-114">Listar Propriedades e relações dos objetos [policySetItem](../resources/intune-policyset-policysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="b174a-114">List properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) objects.</span></span>|
|[<span data-ttu-id="b174a-115">Obter policySetItem</span><span class="sxs-lookup"><span data-stu-id="b174a-115">Get policySetItem</span></span>](../api/intune-policyset-policysetitem-get.md)|[<span data-ttu-id="b174a-116">policySetItem</span><span class="sxs-lookup"><span data-stu-id="b174a-116">policySetItem</span></span>](../resources/intune-policyset-policysetitem.md)|<span data-ttu-id="b174a-117">Leia as propriedades e as relações do objeto [policySetItem](../resources/intune-policyset-policysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="b174a-117">Read properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b174a-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b174a-118">Properties</span></span>
|<span data-ttu-id="b174a-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b174a-119">Property</span></span>|<span data-ttu-id="b174a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b174a-120">Type</span></span>|<span data-ttu-id="b174a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b174a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b174a-122">id</span><span class="sxs-lookup"><span data-stu-id="b174a-122">id</span></span>|<span data-ttu-id="b174a-123">String</span><span class="sxs-lookup"><span data-stu-id="b174a-123">String</span></span>|<span data-ttu-id="b174a-124">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b174a-124">Key of the MobileAppPolicySetItem.</span></span>|
|<span data-ttu-id="b174a-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b174a-125">createdDateTime</span></span>|<span data-ttu-id="b174a-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b174a-126">DateTimeOffset</span></span>|<span data-ttu-id="b174a-127">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b174a-127">Creation time of the PolicySetItem.</span></span>|
|<span data-ttu-id="b174a-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b174a-128">lastModifiedDateTime</span></span>|<span data-ttu-id="b174a-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b174a-129">DateTimeOffset</span></span>|<span data-ttu-id="b174a-130">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b174a-130">Last modified time of the PolicySetItem.</span></span>|
|<span data-ttu-id="b174a-131">payloadId</span><span class="sxs-lookup"><span data-stu-id="b174a-131">payloadId</span></span>|<span data-ttu-id="b174a-132">String</span><span class="sxs-lookup"><span data-stu-id="b174a-132">String</span></span>|<span data-ttu-id="b174a-133">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b174a-133">PayloadId of the PolicySetItem.</span></span>|
|<span data-ttu-id="b174a-134">itemType</span><span class="sxs-lookup"><span data-stu-id="b174a-134">itemType</span></span>|<span data-ttu-id="b174a-135">String</span><span class="sxs-lookup"><span data-stu-id="b174a-135">String</span></span>|<span data-ttu-id="b174a-136">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b174a-136">policySetType of the PolicySetItem.</span></span>|
|<span data-ttu-id="b174a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b174a-137">displayName</span></span>|<span data-ttu-id="b174a-138">String</span><span class="sxs-lookup"><span data-stu-id="b174a-138">String</span></span>|<span data-ttu-id="b174a-139">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b174a-139">DisplayName of the PolicySetItem.</span></span>|
|<span data-ttu-id="b174a-140">status</span><span class="sxs-lookup"><span data-stu-id="b174a-140">status</span></span>|[<span data-ttu-id="b174a-141">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="b174a-141">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="b174a-142">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="b174a-142">Status of the PolicySetItem.</span></span> <span data-ttu-id="b174a-143">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b174a-143">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="b174a-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="b174a-144">errorCode</span></span>|[<span data-ttu-id="b174a-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="b174a-145">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="b174a-146">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="b174a-146">Error code if any occured.</span></span> <span data-ttu-id="b174a-147">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="b174a-147">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="b174a-148">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="b174a-148">guidedDeploymentTags</span></span>|<span data-ttu-id="b174a-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b174a-149">String collection</span></span>|<span data-ttu-id="b174a-150">Marcas da implantação dirigida</span><span class="sxs-lookup"><span data-stu-id="b174a-150">Tags of the guided deployment</span></span>|

## <a name="relationships"></a><span data-ttu-id="b174a-151">Relações</span><span class="sxs-lookup"><span data-stu-id="b174a-151">Relationships</span></span>
<span data-ttu-id="b174a-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b174a-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b174a-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b174a-153">JSON Representation</span></span>
<span data-ttu-id="b174a-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b174a-154">Here is a JSON representation of the resource.</span></span>
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




