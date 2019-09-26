---
title: Criar circularGeofenceManagementCondition
description: Criar um novo objeto circularGeofenceManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e1c27e62eb8f05f5ecd8c0cc8642217fc81f090
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187510"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="0e86a-103">Criar circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="0e86a-103">Create circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="0e86a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e86a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e86a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e86a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e86a-106">Criar um novo objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="0e86a-106">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e86a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e86a-107">Prerequisites</span></span>
<span data-ttu-id="0e86a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e86a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e86a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e86a-110">Permission type</span></span>|<span data-ttu-id="0e86a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0e86a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e86a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e86a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e86a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e86a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e86a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e86a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e86a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e86a-115">Not supported.</span></span>|
|<span data-ttu-id="0e86a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e86a-116">Application</span></span>|<span data-ttu-id="0e86a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e86a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e86a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e86a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="0e86a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e86a-119">Request headers</span></span>
|<span data-ttu-id="0e86a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e86a-120">Header</span></span>|<span data-ttu-id="0e86a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0e86a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e86a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e86a-122">Authorization</span></span>|<span data-ttu-id="0e86a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e86a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e86a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e86a-124">Accept</span></span>|<span data-ttu-id="0e86a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e86a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e86a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e86a-126">Request body</span></span>
<span data-ttu-id="0e86a-127">No corpo da solicitação, forneça uma representação JSON do objeto circularGeofenceManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="0e86a-127">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="0e86a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar circularGeofenceManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="0e86a-128">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="0e86a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e86a-129">Property</span></span>|<span data-ttu-id="0e86a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e86a-130">Type</span></span>|<span data-ttu-id="0e86a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e86a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e86a-132">id</span><span class="sxs-lookup"><span data-stu-id="0e86a-132">id</span></span>|<span data-ttu-id="0e86a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e86a-133">String</span></span>|<span data-ttu-id="0e86a-134">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0e86a-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="0e86a-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="0e86a-135">System generated value assigned when created.</span></span> <span data-ttu-id="0e86a-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e86a-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e86a-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="0e86a-137">uniqueName</span></span>|<span data-ttu-id="0e86a-138">String</span><span class="sxs-lookup"><span data-stu-id="0e86a-138">String</span></span>|<span data-ttu-id="0e86a-139">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0e86a-139">Unique name for the management condition.</span></span> <span data-ttu-id="0e86a-140">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0e86a-140">Used in management condition expressions.</span></span> <span data-ttu-id="0e86a-141">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e86a-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e86a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="0e86a-142">displayName</span></span>|<span data-ttu-id="0e86a-143">String</span><span class="sxs-lookup"><span data-stu-id="0e86a-143">String</span></span>|<span data-ttu-id="0e86a-144">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0e86a-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="0e86a-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e86a-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e86a-146">descrição</span><span class="sxs-lookup"><span data-stu-id="0e86a-146">description</span></span>|<span data-ttu-id="0e86a-147">String</span><span class="sxs-lookup"><span data-stu-id="0e86a-147">String</span></span>|<span data-ttu-id="0e86a-148">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0e86a-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="0e86a-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e86a-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e86a-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e86a-150">createdDateTime</span></span>|<span data-ttu-id="0e86a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e86a-151">DateTimeOffset</span></span>|<span data-ttu-id="0e86a-152">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="0e86a-152">The time the management condition was created.</span></span> <span data-ttu-id="0e86a-153">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="0e86a-153">Generated service side.</span></span> <span data-ttu-id="0e86a-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e86a-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e86a-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e86a-155">modifiedDateTime</span></span>|<span data-ttu-id="0e86a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e86a-156">DateTimeOffset</span></span>|<span data-ttu-id="0e86a-157">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0e86a-157">The time the management condition was last modified.</span></span> <span data-ttu-id="0e86a-158">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="0e86a-158">Updated service side.</span></span> <span data-ttu-id="0e86a-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e86a-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e86a-160">eTag</span><span class="sxs-lookup"><span data-stu-id="0e86a-160">eTag</span></span>|<span data-ttu-id="0e86a-161">String</span><span class="sxs-lookup"><span data-stu-id="0e86a-161">String</span></span>|<span data-ttu-id="0e86a-162">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0e86a-162">ETag of the management condition.</span></span> <span data-ttu-id="0e86a-163">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="0e86a-163">Updated service side.</span></span> <span data-ttu-id="0e86a-164">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0e86a-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0e86a-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0e86a-165">applicablePlatforms</span></span>|<span data-ttu-id="0e86a-166">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="0e86a-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0e86a-167">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0e86a-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="0e86a-168">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="0e86a-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="0e86a-169">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0e86a-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="0e86a-170">latitude</span><span class="sxs-lookup"><span data-stu-id="0e86a-170">latitude</span></span>|<span data-ttu-id="0e86a-171">Duplo</span><span class="sxs-lookup"><span data-stu-id="0e86a-171">Double</span></span>|<span data-ttu-id="0e86a-172">Latitude em graus, entre-90 e + 90 inclusive.</span><span class="sxs-lookup"><span data-stu-id="0e86a-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="0e86a-173">longitude</span><span class="sxs-lookup"><span data-stu-id="0e86a-173">longitude</span></span>|<span data-ttu-id="0e86a-174">Double</span><span class="sxs-lookup"><span data-stu-id="0e86a-174">Double</span></span>|<span data-ttu-id="0e86a-175">Longitude em graus, entre-180 e + 180 inclusive.</span><span class="sxs-lookup"><span data-stu-id="0e86a-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="0e86a-176">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="0e86a-176">radiusInMeters</span></span>|<span data-ttu-id="0e86a-177">Único</span><span class="sxs-lookup"><span data-stu-id="0e86a-177">Single</span></span>|<span data-ttu-id="0e86a-178">RADIUS em metros.</span><span class="sxs-lookup"><span data-stu-id="0e86a-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="0e86a-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e86a-179">Response</span></span>
<span data-ttu-id="0e86a-180">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e86a-180">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e86a-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e86a-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e86a-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e86a-182">Request</span></span>
<span data-ttu-id="0e86a-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e86a-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```

### <a name="response"></a><span data-ttu-id="0e86a-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e86a-184">Response</span></span>
<span data-ttu-id="0e86a-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e86a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 612

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "30ee27b6-27b6-30ee-b627-ee30b627ee30",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```




