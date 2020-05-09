---
title: Criar circularGeofenceManagementCondition
description: Criar um novo objeto circularGeofenceManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76159bf269522433cd3f3dc905d913c71cc4a3ed
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177608"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="ae288-103">Criar circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="ae288-103">Create circularGeofenceManagementCondition</span></span>

<span data-ttu-id="ae288-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae288-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae288-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae288-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae288-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae288-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae288-107">Criar um novo objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="ae288-107">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae288-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae288-108">Prerequisites</span></span>
<span data-ttu-id="ae288-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae288-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae288-111">Permission type</span></span>|<span data-ttu-id="ae288-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae288-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae288-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae288-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae288-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae288-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae288-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae288-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae288-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae288-116">Not supported.</span></span>|
|<span data-ttu-id="ae288-117">Application</span><span class="sxs-lookup"><span data-stu-id="ae288-117">Application</span></span>|<span data-ttu-id="ae288-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae288-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae288-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae288-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="ae288-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae288-120">Request headers</span></span>
|<span data-ttu-id="ae288-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae288-121">Header</span></span>|<span data-ttu-id="ae288-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ae288-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae288-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae288-123">Authorization</span></span>|<span data-ttu-id="ae288-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae288-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae288-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae288-125">Accept</span></span>|<span data-ttu-id="ae288-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae288-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae288-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae288-127">Request body</span></span>
<span data-ttu-id="ae288-128">No corpo da solicitação, forneça uma representação JSON do objeto circularGeofenceManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="ae288-128">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="ae288-129">A tabela a seguir mostra as propriedades que são necessárias ao criar circularGeofenceManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="ae288-129">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="ae288-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae288-130">Property</span></span>|<span data-ttu-id="ae288-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae288-131">Type</span></span>|<span data-ttu-id="ae288-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae288-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae288-133">id</span><span class="sxs-lookup"><span data-stu-id="ae288-133">id</span></span>|<span data-ttu-id="ae288-134">String</span><span class="sxs-lookup"><span data-stu-id="ae288-134">String</span></span>|<span data-ttu-id="ae288-135">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ae288-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="ae288-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="ae288-136">System generated value assigned when created.</span></span> <span data-ttu-id="ae288-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ae288-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ae288-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="ae288-138">uniqueName</span></span>|<span data-ttu-id="ae288-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ae288-139">String</span></span>|<span data-ttu-id="ae288-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ae288-140">Unique name for the management condition.</span></span> <span data-ttu-id="ae288-141">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ae288-141">Used in management condition expressions.</span></span> <span data-ttu-id="ae288-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ae288-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ae288-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ae288-143">displayName</span></span>|<span data-ttu-id="ae288-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae288-144">String</span></span>|<span data-ttu-id="ae288-145">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ae288-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="ae288-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ae288-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ae288-147">description</span><span class="sxs-lookup"><span data-stu-id="ae288-147">description</span></span>|<span data-ttu-id="ae288-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae288-148">String</span></span>|<span data-ttu-id="ae288-149">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ae288-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="ae288-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ae288-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ae288-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae288-151">createdDateTime</span></span>|<span data-ttu-id="ae288-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae288-152">DateTimeOffset</span></span>|<span data-ttu-id="ae288-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="ae288-153">The time the management condition was created.</span></span> <span data-ttu-id="ae288-154">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="ae288-154">Generated service side.</span></span> <span data-ttu-id="ae288-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ae288-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ae288-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae288-156">modifiedDateTime</span></span>|<span data-ttu-id="ae288-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae288-157">DateTimeOffset</span></span>|<span data-ttu-id="ae288-158">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ae288-158">The time the management condition was last modified.</span></span> <span data-ttu-id="ae288-159">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="ae288-159">Updated service side.</span></span> <span data-ttu-id="ae288-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ae288-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ae288-161">eTag</span><span class="sxs-lookup"><span data-stu-id="ae288-161">eTag</span></span>|<span data-ttu-id="ae288-162">String</span><span class="sxs-lookup"><span data-stu-id="ae288-162">String</span></span>|<span data-ttu-id="ae288-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ae288-163">ETag of the management condition.</span></span> <span data-ttu-id="ae288-164">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="ae288-164">Updated service side.</span></span> <span data-ttu-id="ae288-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ae288-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ae288-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="ae288-166">applicablePlatforms</span></span>|<span data-ttu-id="ae288-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="ae288-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="ae288-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ae288-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="ae288-169">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="ae288-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="ae288-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ae288-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="ae288-171">latitude</span><span class="sxs-lookup"><span data-stu-id="ae288-171">latitude</span></span>|<span data-ttu-id="ae288-172">Duplo</span><span class="sxs-lookup"><span data-stu-id="ae288-172">Double</span></span>|<span data-ttu-id="ae288-173">Latitude em graus, entre-90 e + 90 inclusive.</span><span class="sxs-lookup"><span data-stu-id="ae288-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="ae288-174">longitude</span><span class="sxs-lookup"><span data-stu-id="ae288-174">longitude</span></span>|<span data-ttu-id="ae288-175">Double</span><span class="sxs-lookup"><span data-stu-id="ae288-175">Double</span></span>|<span data-ttu-id="ae288-176">Longitude em graus, entre-180 e + 180 inclusive.</span><span class="sxs-lookup"><span data-stu-id="ae288-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="ae288-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="ae288-177">radiusInMeters</span></span>|<span data-ttu-id="ae288-178">Único</span><span class="sxs-lookup"><span data-stu-id="ae288-178">Single</span></span>|<span data-ttu-id="ae288-179">RADIUS em metros.</span><span class="sxs-lookup"><span data-stu-id="ae288-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="ae288-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae288-180">Response</span></span>
<span data-ttu-id="ae288-181">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae288-181">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae288-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae288-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae288-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae288-183">Request</span></span>
<span data-ttu-id="ae288-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae288-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": 2.6666666666666665,
  "longitude": 3.0,
  "radiusInMeters": 4.666666666666667
}
```

### <a name="response"></a><span data-ttu-id="ae288-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae288-185">Response</span></span>
<span data-ttu-id="ae288-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae288-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

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
  "latitude": 2.6666666666666665,
  "longitude": 3.0,
  "radiusInMeters": 4.666666666666667
}
```



