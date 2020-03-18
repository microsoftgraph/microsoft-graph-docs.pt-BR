---
title: Atualizar circularGeofenceManagementCondition
description: Atualiza as propriedades de um objeto circularGeofenceManagementCondition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de97fcec3e071c1fa93fbe7aceaa4d6e438bb681
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804811"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="cfdbf-103">Atualizar circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="cfdbf-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="cfdbf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfdbf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfdbf-106">Atualiza as propriedades de um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="cfdbf-106">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfdbf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cfdbf-107">Prerequisites</span></span>
<span data-ttu-id="cfdbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfdbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfdbf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfdbf-110">Permission type</span></span>|<span data-ttu-id="cfdbf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfdbf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cfdbf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdbf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cfdbf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfdbf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-115">Not supported.</span></span>|
|<span data-ttu-id="cfdbf-116">Application</span><span class="sxs-lookup"><span data-stu-id="cfdbf-116">Application</span></span>|<span data-ttu-id="cfdbf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdbf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfdbf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfdbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="cfdbf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdbf-119">Request headers</span></span>
|<span data-ttu-id="cfdbf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfdbf-120">Header</span></span>|<span data-ttu-id="cfdbf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cfdbf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfdbf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfdbf-122">Authorization</span></span>|<span data-ttu-id="cfdbf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfdbf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cfdbf-124">Accept</span></span>|<span data-ttu-id="cfdbf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cfdbf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfdbf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdbf-126">Request body</span></span>
<span data-ttu-id="cfdbf-127">No corpo da solicitação, forneça uma representação JSON do objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="cfdbf-127">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="cfdbf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="cfdbf-128">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="cfdbf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfdbf-129">Property</span></span>|<span data-ttu-id="cfdbf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfdbf-130">Type</span></span>|<span data-ttu-id="cfdbf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfdbf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfdbf-132">id</span><span class="sxs-lookup"><span data-stu-id="cfdbf-132">id</span></span>|<span data-ttu-id="cfdbf-133">String</span><span class="sxs-lookup"><span data-stu-id="cfdbf-133">String</span></span>|<span data-ttu-id="cfdbf-134">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="cfdbf-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-135">System generated value assigned when created.</span></span> <span data-ttu-id="cfdbf-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cfdbf-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="cfdbf-137">uniqueName</span></span>|<span data-ttu-id="cfdbf-138">String</span><span class="sxs-lookup"><span data-stu-id="cfdbf-138">String</span></span>|<span data-ttu-id="cfdbf-139">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-139">Unique name for the management condition.</span></span> <span data-ttu-id="cfdbf-140">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-140">Used in management condition expressions.</span></span> <span data-ttu-id="cfdbf-141">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cfdbf-142">displayName</span><span class="sxs-lookup"><span data-stu-id="cfdbf-142">displayName</span></span>|<span data-ttu-id="cfdbf-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfdbf-143">String</span></span>|<span data-ttu-id="cfdbf-144">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="cfdbf-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cfdbf-146">description</span><span class="sxs-lookup"><span data-stu-id="cfdbf-146">description</span></span>|<span data-ttu-id="cfdbf-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfdbf-147">String</span></span>|<span data-ttu-id="cfdbf-148">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="cfdbf-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cfdbf-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfdbf-150">createdDateTime</span></span>|<span data-ttu-id="cfdbf-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfdbf-151">DateTimeOffset</span></span>|<span data-ttu-id="cfdbf-152">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-152">The time the management condition was created.</span></span> <span data-ttu-id="cfdbf-153">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-153">Generated service side.</span></span> <span data-ttu-id="cfdbf-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cfdbf-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfdbf-155">modifiedDateTime</span></span>|<span data-ttu-id="cfdbf-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfdbf-156">DateTimeOffset</span></span>|<span data-ttu-id="cfdbf-157">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-157">The time the management condition was last modified.</span></span> <span data-ttu-id="cfdbf-158">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-158">Updated service side.</span></span> <span data-ttu-id="cfdbf-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cfdbf-160">eTag</span><span class="sxs-lookup"><span data-stu-id="cfdbf-160">eTag</span></span>|<span data-ttu-id="cfdbf-161">String</span><span class="sxs-lookup"><span data-stu-id="cfdbf-161">String</span></span>|<span data-ttu-id="cfdbf-162">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-162">ETag of the management condition.</span></span> <span data-ttu-id="cfdbf-163">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-163">Updated service side.</span></span> <span data-ttu-id="cfdbf-164">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cfdbf-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="cfdbf-165">applicablePlatforms</span></span>|<span data-ttu-id="cfdbf-166">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="cfdbf-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="cfdbf-167">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="cfdbf-168">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="cfdbf-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="cfdbf-169">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="cfdbf-170">latitude</span><span class="sxs-lookup"><span data-stu-id="cfdbf-170">latitude</span></span>|<span data-ttu-id="cfdbf-171">Duplo</span><span class="sxs-lookup"><span data-stu-id="cfdbf-171">Double</span></span>|<span data-ttu-id="cfdbf-172">Latitude em graus, entre-90 e + 90 inclusive.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="cfdbf-173">longitude</span><span class="sxs-lookup"><span data-stu-id="cfdbf-173">longitude</span></span>|<span data-ttu-id="cfdbf-174">Double</span><span class="sxs-lookup"><span data-stu-id="cfdbf-174">Double</span></span>|<span data-ttu-id="cfdbf-175">Longitude em graus, entre-180 e + 180 inclusive.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="cfdbf-176">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="cfdbf-176">radiusInMeters</span></span>|<span data-ttu-id="cfdbf-177">Único</span><span class="sxs-lookup"><span data-stu-id="cfdbf-177">Single</span></span>|<span data-ttu-id="cfdbf-178">RADIUS em metros.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="cfdbf-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfdbf-179">Response</span></span>
<span data-ttu-id="cfdbf-180">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-180">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfdbf-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfdbf-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfdbf-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdbf-182">Request</span></span>
<span data-ttu-id="cfdbf-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cfdbf-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfdbf-184">Response</span></span>
<span data-ttu-id="cfdbf-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfdbf-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




