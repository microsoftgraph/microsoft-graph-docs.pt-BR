# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="ba0fa-101">Atualizar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba0fa-101">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="ba0fa-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ba0fa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba0fa-103">Atualizar as propriedades de um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba0fa-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ba0fa-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba0fa-104">Prerequisites</span></span>
<span data-ttu-id="ba0fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba0fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ba0fa-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba0fa-107">Permission type</span></span>|<span data-ttu-id="ba0fa-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba0fa-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba0fa-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba0fa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ba0fa-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba0fa-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ba0fa-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba0fa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba0fa-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba0fa-112">Not supported.</span></span>|
|<span data-ttu-id="ba0fa-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba0fa-113">Application</span></span>|<span data-ttu-id="ba0fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba0fa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba0fa-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba0fa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ba0fa-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba0fa-116">Request headers</span></span>
|<span data-ttu-id="ba0fa-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba0fa-117">Header</span></span>|<span data-ttu-id="ba0fa-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ba0fa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba0fa-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba0fa-119">Authorization</span></span>|<span data-ttu-id="ba0fa-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba0fa-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ba0fa-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba0fa-121">Accept</span></span>|<span data-ttu-id="ba0fa-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ba0fa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba0fa-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba0fa-123">Request body</span></span>
<span data-ttu-id="ba0fa-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba0fa-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="ba0fa-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba0fa-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="ba0fa-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba0fa-126">Property</span></span>|<span data-ttu-id="ba0fa-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba0fa-127">Type</span></span>|<span data-ttu-id="ba0fa-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba0fa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba0fa-129">id</span><span class="sxs-lookup"><span data-stu-id="ba0fa-129">id</span></span>|<span data-ttu-id="ba0fa-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba0fa-130">String</span></span>|<span data-ttu-id="ba0fa-131">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba0fa-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba0fa-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ba0fa-132">displayName</span></span>|<span data-ttu-id="ba0fa-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba0fa-133">String</span></span>|<span data-ttu-id="ba0fa-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba0fa-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba0fa-135">descrição</span><span class="sxs-lookup"><span data-stu-id="ba0fa-135">description</span></span>|<span data-ttu-id="ba0fa-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba0fa-136">String</span></span>|<span data-ttu-id="ba0fa-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba0fa-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba0fa-138">prioridade</span><span class="sxs-lookup"><span data-stu-id="ba0fa-138">priority</span></span>|<span data-ttu-id="ba0fa-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ba0fa-139">Int32</span></span>|<span data-ttu-id="ba0fa-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba0fa-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba0fa-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba0fa-141">createdDateTime</span></span>|<span data-ttu-id="ba0fa-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba0fa-142">DateTimeOffset</span></span>|<span data-ttu-id="ba0fa-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba0fa-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba0fa-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba0fa-144">lastModifiedDateTime</span></span>|<span data-ttu-id="ba0fa-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba0fa-145">DateTimeOffset</span></span>|<span data-ttu-id="ba0fa-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba0fa-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba0fa-147">version</span><span class="sxs-lookup"><span data-stu-id="ba0fa-147">version</span></span>|<span data-ttu-id="ba0fa-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ba0fa-148">Int32</span></span>|<span data-ttu-id="ba0fa-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba0fa-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba0fa-150">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="ba0fa-150">iosRestriction</span></span>|[<span data-ttu-id="ba0fa-151">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ba0fa-151">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ba0fa-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ba0fa-152">Not yet documented</span></span>|
|<span data-ttu-id="ba0fa-153">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="ba0fa-153">windowsRestriction</span></span>|[<span data-ttu-id="ba0fa-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ba0fa-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ba0fa-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ba0fa-155">Not yet documented</span></span>|
|<span data-ttu-id="ba0fa-156">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="ba0fa-156">windowsMobileRestriction</span></span>|[<span data-ttu-id="ba0fa-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ba0fa-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ba0fa-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ba0fa-158">Not yet documented</span></span>|
|<span data-ttu-id="ba0fa-159">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="ba0fa-159">androidRestriction</span></span>|[<span data-ttu-id="ba0fa-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ba0fa-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ba0fa-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ba0fa-161">Not yet documented</span></span>|
|<span data-ttu-id="ba0fa-162">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="ba0fa-162">macOSRestriction</span></span>|[<span data-ttu-id="ba0fa-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ba0fa-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ba0fa-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ba0fa-164">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ba0fa-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba0fa-165">Response</span></span>
<span data-ttu-id="ba0fa-166">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba0fa-166">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba0fa-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba0fa-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="ba0fa-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba0fa-168">Request</span></span>
<span data-ttu-id="ba0fa-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba0fa-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 1626

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="ba0fa-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba0fa-170">Response</span></span>
<span data-ttu-id="ba0fa-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba0fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1822

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```



