---
title: tipo de recurso policySetItem
description: Uma classe que contém as propriedades usadas para o item Policyset.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 98000e00ad90938bc3835b9ba3becb047920fd0a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729105"
---
# <a name="policysetitem-resource-type"></a><span data-ttu-id="39fdb-103">tipo de recurso policySetItem</span><span class="sxs-lookup"><span data-stu-id="39fdb-103">policySetItem resource type</span></span>

> <span data-ttu-id="39fdb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39fdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39fdb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39fdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39fdb-106">Uma classe que contém as propriedades usadas para o item Policyset.</span><span class="sxs-lookup"><span data-stu-id="39fdb-106">A class containing the properties used for PolicySet Item.</span></span>

## <a name="methods"></a><span data-ttu-id="39fdb-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="39fdb-107">Methods</span></span>
|<span data-ttu-id="39fdb-108">Método</span><span class="sxs-lookup"><span data-stu-id="39fdb-108">Method</span></span>|<span data-ttu-id="39fdb-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="39fdb-109">Return Type</span></span>|<span data-ttu-id="39fdb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="39fdb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39fdb-111">Listar policySetItems</span><span class="sxs-lookup"><span data-stu-id="39fdb-111">List policySetItems</span></span>](../api/intune-policyset-policysetitem-list.md)|<span data-ttu-id="39fdb-112">coleção [policySetItem](../resources/intune-policyset-policysetitem.md)</span><span class="sxs-lookup"><span data-stu-id="39fdb-112">[policySetItem](../resources/intune-policyset-policysetitem.md) collection</span></span>|<span data-ttu-id="39fdb-113">Listar Propriedades e relações dos objetos [policySetItem](../resources/intune-policyset-policysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="39fdb-113">List properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) objects.</span></span>|
|[<span data-ttu-id="39fdb-114">Obter policySetItem</span><span class="sxs-lookup"><span data-stu-id="39fdb-114">Get policySetItem</span></span>](../api/intune-policyset-policysetitem-get.md)|[<span data-ttu-id="39fdb-115">policySetItem</span><span class="sxs-lookup"><span data-stu-id="39fdb-115">policySetItem</span></span>](../resources/intune-policyset-policysetitem.md)|<span data-ttu-id="39fdb-116">Leia as propriedades e as relações do objeto [policySetItem](../resources/intune-policyset-policysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="39fdb-116">Read properties and relationships of the [policySetItem](../resources/intune-policyset-policysetitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="39fdb-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39fdb-117">Properties</span></span>
|<span data-ttu-id="39fdb-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39fdb-118">Property</span></span>|<span data-ttu-id="39fdb-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="39fdb-119">Type</span></span>|<span data-ttu-id="39fdb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="39fdb-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39fdb-121">id</span><span class="sxs-lookup"><span data-stu-id="39fdb-121">id</span></span>|<span data-ttu-id="39fdb-122">String</span><span class="sxs-lookup"><span data-stu-id="39fdb-122">String</span></span>|<span data-ttu-id="39fdb-123">Chave do MobileAppPolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="39fdb-123">Key of the MobileAppPolicySetItem.</span></span>|
|<span data-ttu-id="39fdb-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39fdb-124">createdDateTime</span></span>|<span data-ttu-id="39fdb-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39fdb-125">DateTimeOffset</span></span>|<span data-ttu-id="39fdb-126">Hora de criação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="39fdb-126">Creation time of the PolicySetItem.</span></span>|
|<span data-ttu-id="39fdb-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39fdb-127">lastModifiedDateTime</span></span>|<span data-ttu-id="39fdb-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39fdb-128">DateTimeOffset</span></span>|<span data-ttu-id="39fdb-129">Hora da última modificação do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="39fdb-129">Last modified time of the PolicySetItem.</span></span>|
|<span data-ttu-id="39fdb-130">payloadId</span><span class="sxs-lookup"><span data-stu-id="39fdb-130">payloadId</span></span>|<span data-ttu-id="39fdb-131">String</span><span class="sxs-lookup"><span data-stu-id="39fdb-131">String</span></span>|<span data-ttu-id="39fdb-132">PayloadId do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="39fdb-132">PayloadId of the PolicySetItem.</span></span>|
|<span data-ttu-id="39fdb-133">itemType</span><span class="sxs-lookup"><span data-stu-id="39fdb-133">itemType</span></span>|<span data-ttu-id="39fdb-134">String</span><span class="sxs-lookup"><span data-stu-id="39fdb-134">String</span></span>|<span data-ttu-id="39fdb-135">policySetType do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="39fdb-135">policySetType of the PolicySetItem.</span></span>|
|<span data-ttu-id="39fdb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="39fdb-136">displayName</span></span>|<span data-ttu-id="39fdb-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39fdb-137">String</span></span>|<span data-ttu-id="39fdb-138">DisplayName do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="39fdb-138">DisplayName of the PolicySetItem.</span></span>|
|<span data-ttu-id="39fdb-139">status</span><span class="sxs-lookup"><span data-stu-id="39fdb-139">status</span></span>|[<span data-ttu-id="39fdb-140">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="39fdb-140">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="39fdb-141">Status do PolicySetItem.</span><span class="sxs-lookup"><span data-stu-id="39fdb-141">Status of the PolicySetItem.</span></span> <span data-ttu-id="39fdb-142">Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="39fdb-142">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="39fdb-143">errorCode</span><span class="sxs-lookup"><span data-stu-id="39fdb-143">errorCode</span></span>|[<span data-ttu-id="39fdb-144">errorCode</span><span class="sxs-lookup"><span data-stu-id="39fdb-144">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="39fdb-145">Código de erro, caso algum tenha ocorrido.</span><span class="sxs-lookup"><span data-stu-id="39fdb-145">Error code if any occured.</span></span> <span data-ttu-id="39fdb-146">Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="39fdb-146">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="39fdb-147">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="39fdb-147">guidedDeploymentTags</span></span>|<span data-ttu-id="39fdb-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="39fdb-148">String collection</span></span>|<span data-ttu-id="39fdb-149">Marcas da implantação dirigida</span><span class="sxs-lookup"><span data-stu-id="39fdb-149">Tags of the guided deployment</span></span>|

## <a name="relationships"></a><span data-ttu-id="39fdb-150">Relações</span><span class="sxs-lookup"><span data-stu-id="39fdb-150">Relationships</span></span>
<span data-ttu-id="39fdb-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="39fdb-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39fdb-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39fdb-152">JSON Representation</span></span>
<span data-ttu-id="39fdb-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39fdb-153">Here is a JSON representation of the resource.</span></span>
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



