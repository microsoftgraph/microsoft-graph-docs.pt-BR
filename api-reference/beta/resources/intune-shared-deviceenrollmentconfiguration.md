---
title: Tipo de recurso deviceEnrollmentConfiguration
description: A Classe Base de Configuração de Registro de Dispositivo
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d46e446aab9806ad856f71cb8ac57c2f75f1b55
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865793"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="8db00-103">Tipo de recurso deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="8db00-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="8db00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8db00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8db00-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8db00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8db00-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8db00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8db00-107">A Classe Base de Configuração de Registro de Dispositivo</span><span class="sxs-lookup"><span data-stu-id="8db00-107">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="8db00-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8db00-108">Methods</span></span>
|<span data-ttu-id="8db00-109">Método</span><span class="sxs-lookup"><span data-stu-id="8db00-109">Method</span></span>|<span data-ttu-id="8db00-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8db00-110">Return Type</span></span>|<span data-ttu-id="8db00-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8db00-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8db00-112">Listar deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="8db00-112">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="8db00-113">Conjunto [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8db00-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="8db00-114">Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8db00-114">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8db00-115">Obter deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="8db00-115">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="8db00-116">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="8db00-116">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="8db00-117">Ler propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8db00-117">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="8db00-118">**Integração**</span><span class="sxs-lookup"><span data-stu-id="8db00-118">**Onboarding**</span></span>|
|[<span data-ttu-id="8db00-119">Ação setPriority</span><span class="sxs-lookup"><span data-stu-id="8db00-119">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="8db00-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8db00-120">None</span></span>|<span data-ttu-id="8db00-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8db00-121">Not yet documented</span></span>|
|[<span data-ttu-id="8db00-122">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="8db00-122">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="8db00-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8db00-123">None</span></span>|<span data-ttu-id="8db00-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8db00-124">Not yet documented</span></span>|
|<span data-ttu-id="8db00-125">**Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="8db00-125">**Policy Set**</span></span>|
|[<span data-ttu-id="8db00-126">Ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="8db00-126">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="8db00-127">[coleção hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="8db00-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="8db00-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8db00-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8db00-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8db00-129">Properties</span></span>
|<span data-ttu-id="8db00-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8db00-130">Property</span></span>|<span data-ttu-id="8db00-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8db00-131">Type</span></span>|<span data-ttu-id="8db00-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8db00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8db00-133">id</span><span class="sxs-lookup"><span data-stu-id="8db00-133">id</span></span>|<span data-ttu-id="8db00-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8db00-134">String</span></span>|<span data-ttu-id="8db00-135">Identificador exclusivo da conta</span><span class="sxs-lookup"><span data-stu-id="8db00-135">Unique Identifier for the account</span></span>|
|<span data-ttu-id="8db00-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8db00-136">displayName</span></span>|<span data-ttu-id="8db00-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8db00-137">String</span></span>|<span data-ttu-id="8db00-138">O nome de exibição da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8db00-138">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="8db00-139">description</span><span class="sxs-lookup"><span data-stu-id="8db00-139">description</span></span>|<span data-ttu-id="8db00-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8db00-140">String</span></span>|<span data-ttu-id="8db00-141">A descrição da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8db00-141">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="8db00-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="8db00-142">priority</span></span>|<span data-ttu-id="8db00-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8db00-143">Int32</span></span>|<span data-ttu-id="8db00-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="8db00-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="8db00-145">Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo.</span><span class="sxs-lookup"><span data-stu-id="8db00-145">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="8db00-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8db00-146">createdDateTime</span></span>|<span data-ttu-id="8db00-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8db00-147">DateTimeOffset</span></span>|<span data-ttu-id="8db00-148">Hora de data criada no UTC da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8db00-148">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="8db00-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8db00-149">lastModifiedDateTime</span></span>|<span data-ttu-id="8db00-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8db00-150">DateTimeOffset</span></span>|<span data-ttu-id="8db00-151">Última data de modificação no UTC da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8db00-151">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="8db00-152">versão</span><span class="sxs-lookup"><span data-stu-id="8db00-152">version</span></span>|<span data-ttu-id="8db00-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8db00-153">Int32</span></span>|<span data-ttu-id="8db00-154">A versão da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8db00-154">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="8db00-155">Relações</span><span class="sxs-lookup"><span data-stu-id="8db00-155">Relationships</span></span>
|<span data-ttu-id="8db00-156">Relação</span><span class="sxs-lookup"><span data-stu-id="8db00-156">Relationship</span></span>|<span data-ttu-id="8db00-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="8db00-157">Type</span></span>|<span data-ttu-id="8db00-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="8db00-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8db00-159">**Integração**</span><span class="sxs-lookup"><span data-stu-id="8db00-159">**Onboarding**</span></span>|
|<span data-ttu-id="8db00-160">atribuições</span><span class="sxs-lookup"><span data-stu-id="8db00-160">assignments</span></span>|<span data-ttu-id="8db00-161">Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8db00-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8db00-162">A lista de atribuições de grupo para o perfil de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8db00-162">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8db00-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8db00-163">JSON Representation</span></span>
<span data-ttu-id="8db00-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8db00-164">Here is a JSON representation of the resource.</span></span>
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




