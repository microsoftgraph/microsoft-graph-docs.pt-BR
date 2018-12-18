---
title: Criar circularGeofenceManagementCondition
description: Crie um novo objeto de circularGeofenceManagementCondition.
author: tfitzmac
ms.openlocfilehash: fe99dd39aeeee3f9db3e15bdb61c0f3df1c937ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352112"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="06689-103">Criar circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="06689-103">Create circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="06689-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06689-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06689-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06689-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06689-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="06689-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06689-107">Crie um novo objeto de [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="06689-107">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06689-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06689-108">Prerequisites</span></span>
<span data-ttu-id="06689-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06689-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06689-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06689-111">Permission type</span></span>|<span data-ttu-id="06689-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06689-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06689-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06689-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06689-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06689-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06689-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06689-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06689-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06689-116">Not supported.</span></span>|
|<span data-ttu-id="06689-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06689-117">Application</span></span>|<span data-ttu-id="06689-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06689-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06689-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06689-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="06689-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06689-120">Request headers</span></span>
|<span data-ttu-id="06689-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06689-121">Header</span></span>|<span data-ttu-id="06689-122">Valor</span><span class="sxs-lookup"><span data-stu-id="06689-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06689-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="06689-123">Authorization</span></span>|<span data-ttu-id="06689-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06689-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06689-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06689-125">Accept</span></span>|<span data-ttu-id="06689-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06689-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06689-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06689-127">Request body</span></span>
<span data-ttu-id="06689-128">No corpo da solicitação, fornece uma representação JSON para o objeto circularGeofenceManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="06689-128">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="06689-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o circularGeofenceManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="06689-129">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="06689-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06689-130">Property</span></span>|<span data-ttu-id="06689-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="06689-131">Type</span></span>|<span data-ttu-id="06689-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="06689-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06689-133">id</span><span class="sxs-lookup"><span data-stu-id="06689-133">id</span></span>|<span data-ttu-id="06689-134">String</span><span class="sxs-lookup"><span data-stu-id="06689-134">String</span></span>|<span data-ttu-id="06689-135">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06689-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="06689-136">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="06689-136">System generated value assigned when created.</span></span> <span data-ttu-id="06689-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06689-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06689-138">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="06689-138">uniqueName</span></span>|<span data-ttu-id="06689-139">String</span><span class="sxs-lookup"><span data-stu-id="06689-139">String</span></span>|<span data-ttu-id="06689-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06689-140">Unique name for the management condition.</span></span> <span data-ttu-id="06689-141">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06689-141">Used in management condition expressions.</span></span> <span data-ttu-id="06689-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06689-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06689-143">displayName</span><span class="sxs-lookup"><span data-stu-id="06689-143">displayName</span></span>|<span data-ttu-id="06689-144">String</span><span class="sxs-lookup"><span data-stu-id="06689-144">String</span></span>|<span data-ttu-id="06689-145">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06689-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="06689-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06689-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06689-147">description</span><span class="sxs-lookup"><span data-stu-id="06689-147">description</span></span>|<span data-ttu-id="06689-148">String</span><span class="sxs-lookup"><span data-stu-id="06689-148">String</span></span>|<span data-ttu-id="06689-149">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06689-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="06689-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06689-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06689-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06689-151">createdDateTime</span></span>|<span data-ttu-id="06689-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06689-152">DateTimeOffset</span></span>|<span data-ttu-id="06689-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="06689-153">The time the management condition was created.</span></span> <span data-ttu-id="06689-154">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="06689-154">Generated service side.</span></span> <span data-ttu-id="06689-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06689-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06689-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06689-156">modifiedDateTime</span></span>|<span data-ttu-id="06689-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06689-157">DateTimeOffset</span></span>|<span data-ttu-id="06689-158">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06689-158">The time the management condition was last modified.</span></span> <span data-ttu-id="06689-159">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="06689-159">Updated service side.</span></span> <span data-ttu-id="06689-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06689-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06689-161">eTag</span><span class="sxs-lookup"><span data-stu-id="06689-161">eTag</span></span>|<span data-ttu-id="06689-162">String</span><span class="sxs-lookup"><span data-stu-id="06689-162">String</span></span>|<span data-ttu-id="06689-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06689-163">ETag of the management condition.</span></span> <span data-ttu-id="06689-164">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="06689-164">Updated service side.</span></span> <span data-ttu-id="06689-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="06689-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="06689-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="06689-166">applicablePlatforms</span></span>|<span data-ttu-id="06689-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="06689-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="06689-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="06689-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="06689-169">Herdada do [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="06689-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="06689-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="06689-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="06689-171">latitude</span><span class="sxs-lookup"><span data-stu-id="06689-171">latitude</span></span>|<span data-ttu-id="06689-172">Double</span><span class="sxs-lookup"><span data-stu-id="06689-172">Double</span></span>|<span data-ttu-id="06689-173">Latitude em graus, entre -90 e + 90 inclusive.</span><span class="sxs-lookup"><span data-stu-id="06689-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="06689-174">longitude</span><span class="sxs-lookup"><span data-stu-id="06689-174">longitude</span></span>|<span data-ttu-id="06689-175">Double</span><span class="sxs-lookup"><span data-stu-id="06689-175">Double</span></span>|<span data-ttu-id="06689-176">Longitude em graus, entre-180 e + 180 inclusive.</span><span class="sxs-lookup"><span data-stu-id="06689-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="06689-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="06689-177">radiusInMeters</span></span>|<span data-ttu-id="06689-178">Single</span><span class="sxs-lookup"><span data-stu-id="06689-178">Single</span></span>|<span data-ttu-id="06689-179">Raio em metros.</span><span class="sxs-lookup"><span data-stu-id="06689-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="06689-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="06689-180">Response</span></span>
<span data-ttu-id="06689-181">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06689-181">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06689-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06689-182">Example</span></span>
### <a name="request"></a><span data-ttu-id="06689-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06689-183">Request</span></span>
<span data-ttu-id="06689-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06689-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06689-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="06689-185">Response</span></span>
<span data-ttu-id="06689-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06689-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





