---
title: tipo de recurso de officeClientConfiguration
description: Configuração do cliente do Office.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 297383f8b7450e6d0df268afc4c009b3110205ee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879629"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="63dc3-103">tipo de recurso de officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="63dc3-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="63dc3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="63dc3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63dc3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="63dc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63dc3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="63dc3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63dc3-107">Configuração do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="63dc3-107">Office Client Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="63dc3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="63dc3-108">Methods</span></span>
|<span data-ttu-id="63dc3-109">Método</span><span class="sxs-lookup"><span data-stu-id="63dc3-109">Method</span></span>|<span data-ttu-id="63dc3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="63dc3-110">Return Type</span></span>|<span data-ttu-id="63dc3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="63dc3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="63dc3-112">Lista officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="63dc3-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="63dc3-113">coleção [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63dc3-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="63dc3-114">Lista as propriedades e os relacionamentos dos objetos [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="63dc3-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="63dc3-115">Obter officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="63dc3-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="63dc3-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="63dc3-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="63dc3-117">Leia as propriedades e os relacionamentos do objeto [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="63dc3-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="63dc3-118">Ação assign</span><span class="sxs-lookup"><span data-stu-id="63dc3-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="63dc3-119">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="63dc3-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="63dc3-120">Substitua direcionados todos os grupos de uma política.</span><span class="sxs-lookup"><span data-stu-id="63dc3-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="63dc3-121">ação de updatePriorities</span><span class="sxs-lookup"><span data-stu-id="63dc3-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="63dc3-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63dc3-122">None</span></span>|<span data-ttu-id="63dc3-123">Atualize as prioridades de política.</span><span class="sxs-lookup"><span data-stu-id="63dc3-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="63dc3-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63dc3-124">Properties</span></span>
|<span data-ttu-id="63dc3-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63dc3-125">Property</span></span>|<span data-ttu-id="63dc3-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="63dc3-126">Type</span></span>|<span data-ttu-id="63dc3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="63dc3-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63dc3-128">id</span><span class="sxs-lookup"><span data-stu-id="63dc3-128">id</span></span>|<span data-ttu-id="63dc3-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63dc3-129">String</span></span>|<span data-ttu-id="63dc3-130">ID da diretiva de configuração do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="63dc3-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="63dc3-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="63dc3-131">userPreferencePayload</span></span>|<span data-ttu-id="63dc3-132">Stream</span><span class="sxs-lookup"><span data-stu-id="63dc3-132">Stream</span></span>|<span data-ttu-id="63dc3-133">Configurações de preferência JSON da cadeia de caracteres em formato binário, esses valores podem ser substituídos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="63dc3-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="63dc3-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="63dc3-134">policyPayload</span></span>|<span data-ttu-id="63dc3-135">Stream</span><span class="sxs-lookup"><span data-stu-id="63dc3-135">Stream</span></span>|<span data-ttu-id="63dc3-136">Configurações de diretiva JSON da cadeia de caracteres em formato binário, esses valores não podem ser alterados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="63dc3-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="63dc3-137">description</span><span class="sxs-lookup"><span data-stu-id="63dc3-137">description</span></span>|<span data-ttu-id="63dc3-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63dc3-138">String</span></span>|<span data-ttu-id="63dc3-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="63dc3-139">Not yet documented</span></span>|
|<span data-ttu-id="63dc3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="63dc3-140">displayName</span></span>|<span data-ttu-id="63dc3-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63dc3-141">String</span></span>|<span data-ttu-id="63dc3-142">Admin fornecida a descrição do cliente do office política de configuração.</span><span class="sxs-lookup"><span data-stu-id="63dc3-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="63dc3-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63dc3-143">lastModifiedDateTime</span></span>|<span data-ttu-id="63dc3-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="63dc3-144">DateTime</span></span>|<span data-ttu-id="63dc3-145">Carimbo de data e hora modificadas por último da política.</span><span class="sxs-lookup"><span data-stu-id="63dc3-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="63dc3-146">prioridade</span><span class="sxs-lookup"><span data-stu-id="63dc3-146">priority</span></span>|<span data-ttu-id="63dc3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="63dc3-147">Int32</span></span>|<span data-ttu-id="63dc3-148">Valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflito, valores inferiores média de prioridade é alta.</span><span class="sxs-lookup"><span data-stu-id="63dc3-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="63dc3-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="63dc3-149">userCheckinSummary</span></span>|[<span data-ttu-id="63dc3-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="63dc3-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="63dc3-151">Check-in do resumo do usuário para a política.</span><span class="sxs-lookup"><span data-stu-id="63dc3-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="63dc3-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="63dc3-152">checkinStatuses</span></span>|<span data-ttu-id="63dc3-153">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="63dc3-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="63dc3-154">Lista de status de check-in do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="63dc3-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63dc3-155">Relações</span><span class="sxs-lookup"><span data-stu-id="63dc3-155">Relationships</span></span>
|<span data-ttu-id="63dc3-156">Relação</span><span class="sxs-lookup"><span data-stu-id="63dc3-156">Relationship</span></span>|<span data-ttu-id="63dc3-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="63dc3-157">Type</span></span>|<span data-ttu-id="63dc3-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="63dc3-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63dc3-159">assignments</span><span class="sxs-lookup"><span data-stu-id="63dc3-159">assignments</span></span>|<span data-ttu-id="63dc3-160">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="63dc3-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="63dc3-161">A lista de atribuições para a política de grupo.</span><span class="sxs-lookup"><span data-stu-id="63dc3-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63dc3-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63dc3-162">JSON Representation</span></span>
<span data-ttu-id="63dc3-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63dc3-163">Here is a JSON representation of the resource.</span></span>
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



