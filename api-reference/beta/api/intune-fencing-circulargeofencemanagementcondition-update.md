---
title: Atualizar circularGeofenceManagementCondition
description: Atualiza as propriedades de um objeto circularGeofenceManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de4ff2a3903e71a3af2a7de090766cc45bcec127
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442256"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="3ff06-103">Atualizar circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="3ff06-103">Update circularGeofenceManagementCondition</span></span>

<span data-ttu-id="3ff06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ff06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ff06-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ff06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ff06-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ff06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ff06-107">Atualiza as propriedades de um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="3ff06-107">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ff06-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ff06-108">Prerequisites</span></span>
<span data-ttu-id="3ff06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ff06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ff06-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ff06-111">Permission type</span></span>|<span data-ttu-id="3ff06-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3ff06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ff06-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ff06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ff06-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ff06-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ff06-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ff06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ff06-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ff06-116">Not supported.</span></span>|
|<span data-ttu-id="3ff06-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ff06-117">Application</span></span>|<span data-ttu-id="3ff06-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ff06-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ff06-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ff06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="3ff06-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ff06-120">Request headers</span></span>
|<span data-ttu-id="3ff06-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ff06-121">Header</span></span>|<span data-ttu-id="3ff06-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3ff06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ff06-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ff06-123">Authorization</span></span>|<span data-ttu-id="3ff06-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ff06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ff06-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ff06-125">Accept</span></span>|<span data-ttu-id="3ff06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ff06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ff06-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ff06-127">Request body</span></span>
<span data-ttu-id="3ff06-128">No corpo da solicitação, forneça uma representação JSON do objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="3ff06-128">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="3ff06-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="3ff06-129">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="3ff06-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ff06-130">Property</span></span>|<span data-ttu-id="3ff06-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ff06-131">Type</span></span>|<span data-ttu-id="3ff06-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ff06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ff06-133">id</span><span class="sxs-lookup"><span data-stu-id="3ff06-133">id</span></span>|<span data-ttu-id="3ff06-134">String</span><span class="sxs-lookup"><span data-stu-id="3ff06-134">String</span></span>|<span data-ttu-id="3ff06-135">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3ff06-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="3ff06-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="3ff06-136">System generated value assigned when created.</span></span> <span data-ttu-id="3ff06-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3ff06-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3ff06-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="3ff06-138">uniqueName</span></span>|<span data-ttu-id="3ff06-139">String</span><span class="sxs-lookup"><span data-stu-id="3ff06-139">String</span></span>|<span data-ttu-id="3ff06-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3ff06-140">Unique name for the management condition.</span></span> <span data-ttu-id="3ff06-141">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3ff06-141">Used in management condition expressions.</span></span> <span data-ttu-id="3ff06-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3ff06-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3ff06-143">displayName</span><span class="sxs-lookup"><span data-stu-id="3ff06-143">displayName</span></span>|<span data-ttu-id="3ff06-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ff06-144">String</span></span>|<span data-ttu-id="3ff06-145">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3ff06-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="3ff06-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3ff06-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3ff06-147">description</span><span class="sxs-lookup"><span data-stu-id="3ff06-147">description</span></span>|<span data-ttu-id="3ff06-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ff06-148">String</span></span>|<span data-ttu-id="3ff06-149">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3ff06-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="3ff06-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3ff06-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3ff06-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ff06-151">createdDateTime</span></span>|<span data-ttu-id="3ff06-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ff06-152">DateTimeOffset</span></span>|<span data-ttu-id="3ff06-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="3ff06-153">The time the management condition was created.</span></span> <span data-ttu-id="3ff06-154">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="3ff06-154">Generated service side.</span></span> <span data-ttu-id="3ff06-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3ff06-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3ff06-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ff06-156">modifiedDateTime</span></span>|<span data-ttu-id="3ff06-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ff06-157">DateTimeOffset</span></span>|<span data-ttu-id="3ff06-158">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3ff06-158">The time the management condition was last modified.</span></span> <span data-ttu-id="3ff06-159">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="3ff06-159">Updated service side.</span></span> <span data-ttu-id="3ff06-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3ff06-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3ff06-161">eTag</span><span class="sxs-lookup"><span data-stu-id="3ff06-161">eTag</span></span>|<span data-ttu-id="3ff06-162">String</span><span class="sxs-lookup"><span data-stu-id="3ff06-162">String</span></span>|<span data-ttu-id="3ff06-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3ff06-163">ETag of the management condition.</span></span> <span data-ttu-id="3ff06-164">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="3ff06-164">Updated service side.</span></span> <span data-ttu-id="3ff06-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="3ff06-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="3ff06-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="3ff06-166">applicablePlatforms</span></span>|<span data-ttu-id="3ff06-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="3ff06-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="3ff06-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="3ff06-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="3ff06-169">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="3ff06-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="3ff06-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3ff06-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="3ff06-171">latitude</span><span class="sxs-lookup"><span data-stu-id="3ff06-171">latitude</span></span>|<span data-ttu-id="3ff06-172">Duplo</span><span class="sxs-lookup"><span data-stu-id="3ff06-172">Double</span></span>|<span data-ttu-id="3ff06-173">Latitude em graus, entre-90 e + 90 inclusive.</span><span class="sxs-lookup"><span data-stu-id="3ff06-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="3ff06-174">longitude</span><span class="sxs-lookup"><span data-stu-id="3ff06-174">longitude</span></span>|<span data-ttu-id="3ff06-175">Double</span><span class="sxs-lookup"><span data-stu-id="3ff06-175">Double</span></span>|<span data-ttu-id="3ff06-176">Longitude em graus, entre-180 e + 180 inclusive.</span><span class="sxs-lookup"><span data-stu-id="3ff06-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="3ff06-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="3ff06-177">radiusInMeters</span></span>|<span data-ttu-id="3ff06-178">Único</span><span class="sxs-lookup"><span data-stu-id="3ff06-178">Single</span></span>|<span data-ttu-id="3ff06-179">RADIUS em metros.</span><span class="sxs-lookup"><span data-stu-id="3ff06-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="3ff06-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ff06-180">Response</span></span>
<span data-ttu-id="3ff06-181">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ff06-181">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ff06-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ff06-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ff06-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ff06-183">Request</span></span>
<span data-ttu-id="3ff06-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ff06-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
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

### <a name="response"></a><span data-ttu-id="3ff06-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ff06-185">Response</span></span>
<span data-ttu-id="3ff06-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ff06-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



