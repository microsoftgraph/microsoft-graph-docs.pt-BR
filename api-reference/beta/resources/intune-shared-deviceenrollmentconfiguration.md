---
title: Tipo de recurso deviceEnrollmentConfiguration
description: A classe base da configuração de registro do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79941f498efae8167e6d9abcd9bcdf78b9557677
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199615"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="b39ca-103">Tipo de recurso deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="b39ca-103">deviceEnrollmentConfiguration resource type</span></span>

> <span data-ttu-id="b39ca-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b39ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b39ca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b39ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b39ca-106">A classe base da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b39ca-106">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="b39ca-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b39ca-107">Methods</span></span>
|<span data-ttu-id="b39ca-108">Método</span><span class="sxs-lookup"><span data-stu-id="b39ca-108">Method</span></span>|<span data-ttu-id="b39ca-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b39ca-109">Return Type</span></span>|<span data-ttu-id="b39ca-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b39ca-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b39ca-111">Listar deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="b39ca-111">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="b39ca-112">Conjunto [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b39ca-112">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="b39ca-113">Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b39ca-113">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b39ca-114">Obter deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="b39ca-114">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="b39ca-115">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="b39ca-115">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="b39ca-116">Ler propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b39ca-116">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="b39ca-117">**Integração**</span><span class="sxs-lookup"><span data-stu-id="b39ca-117">**Onboarding**</span></span>|
|[<span data-ttu-id="b39ca-118">Ação setPriority</span><span class="sxs-lookup"><span data-stu-id="b39ca-118">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="b39ca-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b39ca-119">None</span></span>|<span data-ttu-id="b39ca-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b39ca-120">Not yet documented</span></span>|
|[<span data-ttu-id="b39ca-121">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="b39ca-121">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="b39ca-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b39ca-122">None</span></span>|<span data-ttu-id="b39ca-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b39ca-123">Not yet documented</span></span>|
|<span data-ttu-id="b39ca-124">**Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="b39ca-124">**Policy Set**</span></span>|
|[<span data-ttu-id="b39ca-125">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="b39ca-125">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="b39ca-126">coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="b39ca-126">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="b39ca-127">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b39ca-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b39ca-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b39ca-128">Properties</span></span>
|<span data-ttu-id="b39ca-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b39ca-129">Property</span></span>|<span data-ttu-id="b39ca-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b39ca-130">Type</span></span>|<span data-ttu-id="b39ca-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b39ca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b39ca-132">id</span><span class="sxs-lookup"><span data-stu-id="b39ca-132">id</span></span>|<span data-ttu-id="b39ca-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b39ca-133">String</span></span>|<span data-ttu-id="b39ca-134">Identificador exclusivo para a conta</span><span class="sxs-lookup"><span data-stu-id="b39ca-134">Unique Identifier for the account</span></span>|
|<span data-ttu-id="b39ca-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b39ca-135">displayName</span></span>|<span data-ttu-id="b39ca-136">String</span><span class="sxs-lookup"><span data-stu-id="b39ca-136">String</span></span>|<span data-ttu-id="b39ca-137">O nome de exibição da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b39ca-137">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="b39ca-138">descrição</span><span class="sxs-lookup"><span data-stu-id="b39ca-138">description</span></span>|<span data-ttu-id="b39ca-139">String</span><span class="sxs-lookup"><span data-stu-id="b39ca-139">String</span></span>|<span data-ttu-id="b39ca-140">A descrição da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b39ca-140">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="b39ca-141">prioridade</span><span class="sxs-lookup"><span data-stu-id="b39ca-141">priority</span></span>|<span data-ttu-id="b39ca-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b39ca-142">Int32</span></span>|<span data-ttu-id="b39ca-143">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="b39ca-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="b39ca-144">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="b39ca-144">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="b39ca-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b39ca-145">createdDateTime</span></span>|<span data-ttu-id="b39ca-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b39ca-146">DateTimeOffset</span></span>|<span data-ttu-id="b39ca-147">Data e hora de criação em UTC da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b39ca-147">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="b39ca-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b39ca-148">lastModifiedDateTime</span></span>|<span data-ttu-id="b39ca-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b39ca-149">DateTimeOffset</span></span>|<span data-ttu-id="b39ca-150">Data e hora da última modificação em UTC da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b39ca-150">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="b39ca-151">versão</span><span class="sxs-lookup"><span data-stu-id="b39ca-151">version</span></span>|<span data-ttu-id="b39ca-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b39ca-152">Int32</span></span>|<span data-ttu-id="b39ca-153">A versão da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b39ca-153">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="b39ca-154">Relações</span><span class="sxs-lookup"><span data-stu-id="b39ca-154">Relationships</span></span>
|<span data-ttu-id="b39ca-155">Relação</span><span class="sxs-lookup"><span data-stu-id="b39ca-155">Relationship</span></span>|<span data-ttu-id="b39ca-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="b39ca-156">Type</span></span>|<span data-ttu-id="b39ca-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="b39ca-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b39ca-158">**Integração**</span><span class="sxs-lookup"><span data-stu-id="b39ca-158">**Onboarding**</span></span>|
|<span data-ttu-id="b39ca-159">atribuições</span><span class="sxs-lookup"><span data-stu-id="b39ca-159">assignments</span></span>|<span data-ttu-id="b39ca-160">Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b39ca-160">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b39ca-161">A lista de atribuições de grupo para o perfil de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b39ca-161">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b39ca-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b39ca-162">JSON Representation</span></span>
<span data-ttu-id="b39ca-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b39ca-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```



