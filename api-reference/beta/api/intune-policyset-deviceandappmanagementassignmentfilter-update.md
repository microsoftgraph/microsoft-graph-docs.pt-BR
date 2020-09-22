---
title: Atualizar deviceAndAppManagementAssignmentFilter
description: Atualiza as propriedades de um objeto deviceAndAppManagementAssignmentFilter.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff69e8d1675e9909052e286951ee2fedc5f0b4c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999871"
---
# <a name="update-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="9501a-103">Atualizar deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="9501a-103">Update deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="9501a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9501a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9501a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9501a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9501a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9501a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9501a-107">Atualiza as propriedades de um objeto [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .</span><span class="sxs-lookup"><span data-stu-id="9501a-107">Update the properties of a [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9501a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9501a-108">Prerequisites</span></span>
<span data-ttu-id="9501a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9501a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9501a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9501a-111">Permission type</span></span>|<span data-ttu-id="9501a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9501a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9501a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9501a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9501a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9501a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9501a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9501a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9501a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9501a-116">Not supported.</span></span>|
|<span data-ttu-id="9501a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9501a-117">Application</span></span>|<span data-ttu-id="9501a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9501a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9501a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9501a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a><span data-ttu-id="9501a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9501a-120">Request headers</span></span>
|<span data-ttu-id="9501a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9501a-121">Header</span></span>|<span data-ttu-id="9501a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9501a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9501a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9501a-123">Authorization</span></span>|<span data-ttu-id="9501a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9501a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9501a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9501a-125">Accept</span></span>|<span data-ttu-id="9501a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9501a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9501a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9501a-127">Request body</span></span>
<span data-ttu-id="9501a-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) .</span><span class="sxs-lookup"><span data-stu-id="9501a-128">In the request body, supply a JSON representation for the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

<span data-ttu-id="9501a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span><span class="sxs-lookup"><span data-stu-id="9501a-129">The following table shows the properties that are required when you create the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).</span></span>

|<span data-ttu-id="9501a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9501a-130">Property</span></span>|<span data-ttu-id="9501a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9501a-131">Type</span></span>|<span data-ttu-id="9501a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9501a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9501a-133">id</span><span class="sxs-lookup"><span data-stu-id="9501a-133">id</span></span>|<span data-ttu-id="9501a-134">String</span><span class="sxs-lookup"><span data-stu-id="9501a-134">String</span></span>|<span data-ttu-id="9501a-135">Chave do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="9501a-135">Key of the Assignment Filter.</span></span>|
|<span data-ttu-id="9501a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9501a-136">createdDateTime</span></span>|<span data-ttu-id="9501a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9501a-137">DateTimeOffset</span></span>|<span data-ttu-id="9501a-138">Hora de criação do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="9501a-138">Creation time of the Assignment Filter.</span></span>|
|<span data-ttu-id="9501a-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9501a-139">lastModifiedDateTime</span></span>|<span data-ttu-id="9501a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9501a-140">DateTimeOffset</span></span>|<span data-ttu-id="9501a-141">Hora da última modificação do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="9501a-141">Last modified time of the Assignment Filter.</span></span>|
|<span data-ttu-id="9501a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="9501a-142">displayName</span></span>|<span data-ttu-id="9501a-143">String</span><span class="sxs-lookup"><span data-stu-id="9501a-143">String</span></span>|<span data-ttu-id="9501a-144">DisplayName do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="9501a-144">DisplayName of the Assignment Filter.</span></span>|
|<span data-ttu-id="9501a-145">description</span><span class="sxs-lookup"><span data-stu-id="9501a-145">description</span></span>|<span data-ttu-id="9501a-146">String</span><span class="sxs-lookup"><span data-stu-id="9501a-146">String</span></span>|<span data-ttu-id="9501a-147">Descrição do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="9501a-147">Description of the Assignment Filter.</span></span>|
|<span data-ttu-id="9501a-148">plataforma</span><span class="sxs-lookup"><span data-stu-id="9501a-148">platform</span></span>|[<span data-ttu-id="9501a-149">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="9501a-149">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="9501a-150">Tipo de plataforma dos dispositivos nos quais o filtro de atribuição será aplicável.</span><span class="sxs-lookup"><span data-stu-id="9501a-150">Platform type of the devices on which the Assignment Filter will be applicable.</span></span> <span data-ttu-id="9501a-151">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="9501a-151">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="9501a-152">norma</span><span class="sxs-lookup"><span data-stu-id="9501a-152">rule</span></span>|<span data-ttu-id="9501a-153">String</span><span class="sxs-lookup"><span data-stu-id="9501a-153">String</span></span>|<span data-ttu-id="9501a-154">Definição de regra do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="9501a-154">Rule definition of the Assignment Filter.</span></span>|
|<span data-ttu-id="9501a-155">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="9501a-155">roleScopeTags</span></span>|<span data-ttu-id="9501a-156">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9501a-156">String collection</span></span>|<span data-ttu-id="9501a-157">RoleScopeTags do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="9501a-157">RoleScopeTags of the Assignment Filter.</span></span>|



## <a name="response"></a><span data-ttu-id="9501a-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="9501a-158">Response</span></span>
<span data-ttu-id="9501a-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9501a-159">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9501a-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9501a-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="9501a-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9501a-161">Request</span></span>
<span data-ttu-id="9501a-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9501a-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
Content-type: application/json
Content-length: 274

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="9501a-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9501a-163">Response</span></span>
<span data-ttu-id="9501a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9501a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "id": "819818db-18db-8198-db18-9881db189881",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```






