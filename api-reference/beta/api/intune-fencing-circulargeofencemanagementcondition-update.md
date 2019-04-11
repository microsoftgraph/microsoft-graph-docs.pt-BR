---
title: Atualizar circularGeofenceManagementCondition
description: Atualiza as propriedades de um objeto circularGeofenceManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa9c306ad3e79967223af5c55a628c84c34978b4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776567"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="d2ae7-103">Atualizar circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="d2ae7-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="d2ae7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2ae7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2ae7-106">Atualiza as propriedades de um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="d2ae7-106">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2ae7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2ae7-107">Prerequisites</span></span>
<span data-ttu-id="d2ae7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2ae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2ae7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2ae7-110">Permission type</span></span>|<span data-ttu-id="d2ae7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2ae7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2ae7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2ae7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2ae7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2ae7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-115">Not supported.</span></span>|
|<span data-ttu-id="d2ae7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2ae7-116">Application</span></span>|<span data-ttu-id="d2ae7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2ae7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2ae7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="d2ae7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2ae7-119">Request headers</span></span>
|<span data-ttu-id="d2ae7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2ae7-120">Header</span></span>|<span data-ttu-id="d2ae7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d2ae7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2ae7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2ae7-122">Authorization</span></span>|<span data-ttu-id="d2ae7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2ae7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2ae7-124">Accept</span></span>|<span data-ttu-id="d2ae7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2ae7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2ae7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2ae7-126">Request body</span></span>
<span data-ttu-id="d2ae7-127">No corpo da solicitação, forneça uma representação JSON do objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="d2ae7-127">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="d2ae7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="d2ae7-128">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="d2ae7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2ae7-129">Property</span></span>|<span data-ttu-id="d2ae7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2ae7-130">Type</span></span>|<span data-ttu-id="d2ae7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2ae7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2ae7-132">id</span><span class="sxs-lookup"><span data-stu-id="d2ae7-132">id</span></span>|<span data-ttu-id="d2ae7-133">String</span><span class="sxs-lookup"><span data-stu-id="d2ae7-133">String</span></span>|<span data-ttu-id="d2ae7-134">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="d2ae7-135">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-135">System generated value assigned when created.</span></span> <span data-ttu-id="d2ae7-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2ae7-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="d2ae7-137">uniqueName</span></span>|<span data-ttu-id="d2ae7-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2ae7-138">String</span></span>|<span data-ttu-id="d2ae7-139">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-139">Unique name for the management condition.</span></span> <span data-ttu-id="d2ae7-140">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-140">Used in management condition expressions.</span></span> <span data-ttu-id="d2ae7-141">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2ae7-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d2ae7-142">displayName</span></span>|<span data-ttu-id="d2ae7-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2ae7-143">String</span></span>|<span data-ttu-id="d2ae7-144">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="d2ae7-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2ae7-146">description</span><span class="sxs-lookup"><span data-stu-id="d2ae7-146">description</span></span>|<span data-ttu-id="d2ae7-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2ae7-147">String</span></span>|<span data-ttu-id="d2ae7-148">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="d2ae7-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2ae7-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2ae7-150">createdDateTime</span></span>|<span data-ttu-id="d2ae7-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2ae7-151">DateTimeOffset</span></span>|<span data-ttu-id="d2ae7-152">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-152">The time the management condition was created.</span></span> <span data-ttu-id="d2ae7-153">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-153">Generated service side.</span></span> <span data-ttu-id="d2ae7-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2ae7-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2ae7-155">modifiedDateTime</span></span>|<span data-ttu-id="d2ae7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2ae7-156">DateTimeOffset</span></span>|<span data-ttu-id="d2ae7-157">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-157">The time the management condition was last modified.</span></span> <span data-ttu-id="d2ae7-158">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-158">Updated service side.</span></span> <span data-ttu-id="d2ae7-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2ae7-160">eTag</span><span class="sxs-lookup"><span data-stu-id="d2ae7-160">eTag</span></span>|<span data-ttu-id="d2ae7-161">String</span><span class="sxs-lookup"><span data-stu-id="d2ae7-161">String</span></span>|<span data-ttu-id="d2ae7-162">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-162">ETag of the management condition.</span></span> <span data-ttu-id="d2ae7-163">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-163">Updated service side.</span></span> <span data-ttu-id="d2ae7-164">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d2ae7-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="d2ae7-165">applicablePlatforms</span></span>|<span data-ttu-id="d2ae7-166">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="d2ae7-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="d2ae7-167">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="d2ae7-168">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="d2ae7-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="d2ae7-169">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="d2ae7-170">latitude</span><span class="sxs-lookup"><span data-stu-id="d2ae7-170">latitude</span></span>|<span data-ttu-id="d2ae7-171">Duplo</span><span class="sxs-lookup"><span data-stu-id="d2ae7-171">Double</span></span>|<span data-ttu-id="d2ae7-172">Latitude em graus, entre-90 e + 90 inclusive.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="d2ae7-173">longitude</span><span class="sxs-lookup"><span data-stu-id="d2ae7-173">longitude</span></span>|<span data-ttu-id="d2ae7-174">Double</span><span class="sxs-lookup"><span data-stu-id="d2ae7-174">Double</span></span>|<span data-ttu-id="d2ae7-175">Longitude em graus, entre-180 e + 180 inclusive.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="d2ae7-176">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="d2ae7-176">radiusInMeters</span></span>|<span data-ttu-id="d2ae7-177">Único</span><span class="sxs-lookup"><span data-stu-id="d2ae7-177">Single</span></span>|<span data-ttu-id="d2ae7-178">RADIUS em metros.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="d2ae7-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2ae7-179">Response</span></span>
<span data-ttu-id="d2ae7-180">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-180">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2ae7-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2ae7-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2ae7-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2ae7-182">Request</span></span>
<span data-ttu-id="d2ae7-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d2ae7-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2ae7-184">Response</span></span>
<span data-ttu-id="d2ae7-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2ae7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





