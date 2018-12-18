---
title: tipo de recurso de officeClientConfiguration
description: Configuração do cliente do Office.
author: tfitzmac
ms.openlocfilehash: 67a7845a2e0327e2e5de37d424274f6e2ee35604
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303833"
---
# <a name="officeclientconfiguration-resource-type"></a><span data-ttu-id="b7624-103">tipo de recurso de officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7624-103">officeClientConfiguration resource type</span></span>

> <span data-ttu-id="b7624-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b7624-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7624-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b7624-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7624-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b7624-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7624-107">Configuração do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="b7624-107">Office Client Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="b7624-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b7624-108">Methods</span></span>
|<span data-ttu-id="b7624-109">Método</span><span class="sxs-lookup"><span data-stu-id="b7624-109">Method</span></span>|<span data-ttu-id="b7624-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b7624-110">Return Type</span></span>|<span data-ttu-id="b7624-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7624-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b7624-112">Lista officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="b7624-112">List officeClientConfigurations</span></span>](../api/intune-cirrus-officeclientconfiguration-list.md)|<span data-ttu-id="b7624-113">coleção [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7624-113">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="b7624-114">Lista as propriedades e os relacionamentos dos objetos [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b7624-114">List properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b7624-115">Obter officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7624-115">Get officeClientConfiguration</span></span>](../api/intune-cirrus-officeclientconfiguration-get.md)|[<span data-ttu-id="b7624-116">officeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7624-116">officeClientConfiguration</span></span>](../resources/intune-cirrus-officeclientconfiguration.md)|<span data-ttu-id="b7624-117">Leia as propriedades e os relacionamentos do objeto [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b7624-117">Read properties and relationships of the [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b7624-118">Ação assign</span><span class="sxs-lookup"><span data-stu-id="b7624-118">assign action</span></span>](../api/intune-cirrus-officeclientconfiguration-assign.md)|<span data-ttu-id="b7624-119">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b7624-119">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b7624-120">Substitua direcionados todos os grupos de uma política.</span><span class="sxs-lookup"><span data-stu-id="b7624-120">Replace all targeted groups for a policy.</span></span>|
|[<span data-ttu-id="b7624-121">ação de updatePriorities</span><span class="sxs-lookup"><span data-stu-id="b7624-121">updatePriorities action</span></span>](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|<span data-ttu-id="b7624-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7624-122">None</span></span>|<span data-ttu-id="b7624-123">Atualize as prioridades de política.</span><span class="sxs-lookup"><span data-stu-id="b7624-123">Update policy priorities.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7624-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7624-124">Properties</span></span>
|<span data-ttu-id="b7624-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7624-125">Property</span></span>|<span data-ttu-id="b7624-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7624-126">Type</span></span>|<span data-ttu-id="b7624-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7624-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7624-128">id</span><span class="sxs-lookup"><span data-stu-id="b7624-128">id</span></span>|<span data-ttu-id="b7624-129">String</span><span class="sxs-lookup"><span data-stu-id="b7624-129">String</span></span>|<span data-ttu-id="b7624-130">ID da diretiva de configuração do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="b7624-130">Id of the office client configuration policy.</span></span>|
|<span data-ttu-id="b7624-131">userPreferencePayload</span><span class="sxs-lookup"><span data-stu-id="b7624-131">userPreferencePayload</span></span>|<span data-ttu-id="b7624-132">Stream</span><span class="sxs-lookup"><span data-stu-id="b7624-132">Stream</span></span>|<span data-ttu-id="b7624-133">Configurações de preferência JSON da cadeia de caracteres em formato binário, esses valores podem ser substituídos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b7624-133">Preference settings JSON string in binary format, these values can be overridden by the user.</span></span>|
|<span data-ttu-id="b7624-134">policyPayload</span><span class="sxs-lookup"><span data-stu-id="b7624-134">policyPayload</span></span>|<span data-ttu-id="b7624-135">Stream</span><span class="sxs-lookup"><span data-stu-id="b7624-135">Stream</span></span>|<span data-ttu-id="b7624-136">Configurações de diretiva JSON da cadeia de caracteres em formato binário, esses valores não podem ser alterados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b7624-136">Policy settings JSON string in binary format, these values cannot be changed by the user.</span></span>|
|<span data-ttu-id="b7624-137">description</span><span class="sxs-lookup"><span data-stu-id="b7624-137">description</span></span>|<span data-ttu-id="b7624-138">String</span><span class="sxs-lookup"><span data-stu-id="b7624-138">String</span></span>|<span data-ttu-id="b7624-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b7624-139">Not yet documented</span></span>|
|<span data-ttu-id="b7624-140">displayName</span><span class="sxs-lookup"><span data-stu-id="b7624-140">displayName</span></span>|<span data-ttu-id="b7624-141">String</span><span class="sxs-lookup"><span data-stu-id="b7624-141">String</span></span>|<span data-ttu-id="b7624-142">Admin fornecida a descrição do cliente do office política de configuração.</span><span class="sxs-lookup"><span data-stu-id="b7624-142">Admin provided description of the office client configuration policy.</span></span>|
|<span data-ttu-id="b7624-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7624-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b7624-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="b7624-144">DateTime</span></span>|<span data-ttu-id="b7624-145">Carimbo de data e hora modificadas por último da política.</span><span class="sxs-lookup"><span data-stu-id="b7624-145">Last modified datetime stamp of the policy.</span></span>|
|<span data-ttu-id="b7624-146">prioridade</span><span class="sxs-lookup"><span data-stu-id="b7624-146">priority</span></span>|<span data-ttu-id="b7624-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b7624-147">Int32</span></span>|<span data-ttu-id="b7624-148">Valor de prioridade deve ser um valor exclusivo para cada política em um locatário e será usado para resolução de conflito, valores inferiores média de prioridade é alta.</span><span class="sxs-lookup"><span data-stu-id="b7624-148">Priority value should be unique value for each policy under a tenant and will be used for conflict resolution, lower values mean priority is high.</span></span>|
|<span data-ttu-id="b7624-149">userCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b7624-149">userCheckinSummary</span></span>|[<span data-ttu-id="b7624-150">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b7624-150">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="b7624-151">Check-in do resumo do usuário para a política.</span><span class="sxs-lookup"><span data-stu-id="b7624-151">User check-in summary for the policy.</span></span>|
|<span data-ttu-id="b7624-152">checkinStatuses</span><span class="sxs-lookup"><span data-stu-id="b7624-152">checkinStatuses</span></span>|<span data-ttu-id="b7624-153">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b7624-153">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="b7624-154">Lista de status de check-in do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="b7624-154">List of office Client check-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7624-155">Relações</span><span class="sxs-lookup"><span data-stu-id="b7624-155">Relationships</span></span>
|<span data-ttu-id="b7624-156">Relação</span><span class="sxs-lookup"><span data-stu-id="b7624-156">Relationship</span></span>|<span data-ttu-id="b7624-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7624-157">Type</span></span>|<span data-ttu-id="b7624-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7624-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7624-159">assignments</span><span class="sxs-lookup"><span data-stu-id="b7624-159">assignments</span></span>|<span data-ttu-id="b7624-160">coleção [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b7624-160">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b7624-161">A lista de atribuições para a política de grupo.</span><span class="sxs-lookup"><span data-stu-id="b7624-161">The list of group assignments for the policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7624-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7624-162">JSON Representation</span></span>
<span data-ttu-id="b7624-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7624-163">Here is a JSON representation of the resource.</span></span>
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



