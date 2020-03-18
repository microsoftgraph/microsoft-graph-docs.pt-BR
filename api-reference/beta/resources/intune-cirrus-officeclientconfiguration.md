---
title: tipo de recurso Conjuntoofficeclientconfiguration
description: Configuração de cliente do Office.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a6077f327efc24279d04e1a4a377f2ef50eb171
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797329"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="62094-103">tipo de recurso Conjuntoofficeclientconfiguration</span><span class="sxs-lookup"><span data-stu-id="62094-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="62094-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62094-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62094-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62094-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62094-106">Configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="62094-106">Office Client Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="62094-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="62094-107">Methods</span></span>
|<span data-ttu-id="62094-108">Método</span><span class="sxs-lookup"><span data-stu-id="62094-108">Method</span></span>|<span data-ttu-id="62094-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="62094-109">Return Type</span></span>|<span data-ttu-id="62094-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="62094-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="62094-111">Listar officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="62094-111">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="62094-112">coleção [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62094-112">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="62094-113">Listar Propriedades e relações dos objetos [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="62094-113">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="62094-114">Obter Conjuntoofficeclientconfiguration</span><span class="sxs-lookup"><span data-stu-id="62094-114">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="62094-115">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="62094-115">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="62094-116">Leia as propriedades e as relações do objeto [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="62094-116">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="62094-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="62094-117">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="62094-118">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="62094-118">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="62094-119">Substituir todos os grupos de destino de uma política.</span><span class="sxs-lookup"><span data-stu-id="62094-119">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="62094-120">ação updatePriorities</span><span class="sxs-lookup"><span data-stu-id="62094-120">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="62094-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62094-121">None</span></span>|<span data-ttu-id="62094-122">Atualizar prioridades de política.</span><span class="sxs-lookup"><span data-stu-id="62094-122">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="62094-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62094-123">Properties</span></span>
|<span data-ttu-id="62094-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62094-124">Property</span></span>|<span data-ttu-id="62094-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="62094-125">Type</span></span>|<span data-ttu-id="62094-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="62094-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62094-127">id</span><span class="sxs-lookup"><span data-stu-id="62094-127">id</span></span>|<span data-ttu-id="62094-128">String</span><span class="sxs-lookup"><span data-stu-id="62094-128">String</span></span>|<span data-ttu-id="62094-129">ID da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="62094-129">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="62094-130">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="62094-130">userPreferencePayload</span></span>|<span data-ttu-id="62094-131">Stream</span><span class="sxs-lookup"><span data-stu-id="62094-131">Stream</span></span>|<span data-ttu-id="62094-132">Cadeia de caracteres JSON das configurações de preferência no formato binário, esses valores podem ser substituídos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="62094-132">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="62094-133">policyPayload</span><span class="sxs-lookup"><span data-stu-id="62094-133">policyPayload</span></span>|<span data-ttu-id="62094-134">Stream</span><span class="sxs-lookup"><span data-stu-id="62094-134">Stream</span></span>|<span data-ttu-id="62094-135">Cadeia de caracteres JSON de configurações de política no formato binário, esses valores não podem ser alterados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="62094-135">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="62094-136">description</span><span class="sxs-lookup"><span data-stu-id="62094-136">description</span></span>|<span data-ttu-id="62094-137">String</span><span class="sxs-lookup"><span data-stu-id="62094-137">String</span></span>|<span data-ttu-id="62094-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="62094-138">Not yet documented</span></span>|
|<span data-ttu-id="62094-139">displayName</span><span class="sxs-lookup"><span data-stu-id="62094-139">displayName</span></span>|<span data-ttu-id="62094-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62094-140">String</span></span>|<span data-ttu-id="62094-141">Descrição fornecida pelo administrador da política de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="62094-141">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="62094-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62094-142">lastModifiedDateTime</span></span>|<span data-ttu-id="62094-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="62094-143">DateTime</span></span>|<span data-ttu-id="62094-144">Carimbo de data/hora da última modificação da política.</span><span class="sxs-lookup"><span data-stu-id="62094-144">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="62094-145">prioridade</span><span class="sxs-lookup"><span data-stu-id="62094-145">priority</span></span>|<span data-ttu-id="62094-146">Int32</span><span class="sxs-lookup"><span data-stu-id="62094-146">Int32</span></span>|<span data-ttu-id="62094-147">O valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflitos, a prioridade média de valores menores é alta.</span><span class="sxs-lookup"><span data-stu-id="62094-147">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="62094-148">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="62094-148">userCheckinSummary</span></span>|[<span data-ttu-id="62094-149">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="62094-149">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="62094-150">Resumo de check-in do usuário da política.</span><span class="sxs-lookup"><span data-stu-id="62094-150">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="62094-151">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="62094-151">checkinStatuses</span></span>|<span data-ttu-id="62094-152">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="62094-152">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="62094-153">Lista de status de check-in do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="62094-153">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62094-154">Relações</span><span class="sxs-lookup"><span data-stu-id="62094-154">Relationships</span></span>
|<span data-ttu-id="62094-155">Relação</span><span class="sxs-lookup"><span data-stu-id="62094-155">Relationship</span></span>|<span data-ttu-id="62094-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="62094-156">Type</span></span>|<span data-ttu-id="62094-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="62094-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62094-158">assignments</span><span class="sxs-lookup"><span data-stu-id="62094-158">assignments</span></span>|<span data-ttu-id="62094-159">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="62094-159">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="62094-160">A lista de atribuições de grupo para a política.</span><span class="sxs-lookup"><span data-stu-id="62094-160">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62094-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62094-161">JSON Representation</span></span>
<span data-ttu-id="62094-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62094-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```



