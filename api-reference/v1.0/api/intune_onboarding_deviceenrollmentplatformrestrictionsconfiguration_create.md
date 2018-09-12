# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="a0a35-101">Criar deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0a35-101">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="a0a35-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0a35-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0a35-103">Criar um novo objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0a35-103">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0a35-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0a35-104">Prerequisites</span></span>
<span data-ttu-id="a0a35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a0a35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a0a35-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0a35-107">Permission type</span></span>|<span data-ttu-id="a0a35-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0a35-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0a35-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0a35-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a0a35-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0a35-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a0a35-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0a35-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0a35-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0a35-112">Not supported.</span></span>|
|<span data-ttu-id="a0a35-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0a35-113">Application</span></span>|<span data-ttu-id="a0a35-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0a35-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0a35-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0a35-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0a35-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a35-116">Request headers</span></span>
|<span data-ttu-id="a0a35-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0a35-117">Header</span></span>|<span data-ttu-id="a0a35-118">Valor</span><span class="sxs-lookup"><span data-stu-id="a0a35-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0a35-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0a35-119">Authorization</span></span>|<span data-ttu-id="a0a35-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="a0a35-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0a35-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0a35-121">Accept</span></span>|<span data-ttu-id="a0a35-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a0a35-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0a35-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a35-123">Request body</span></span>
<span data-ttu-id="a0a35-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0a35-124">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="a0a35-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0a35-125">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="a0a35-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0a35-126">Property</span></span>|<span data-ttu-id="a0a35-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0a35-127">Type</span></span>|<span data-ttu-id="a0a35-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0a35-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0a35-129">id</span><span class="sxs-lookup"><span data-stu-id="a0a35-129">id</span></span>|<span data-ttu-id="a0a35-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0a35-130">String</span></span>|<span data-ttu-id="a0a35-131">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0a35-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a0a35-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a0a35-132">displayName</span></span>|<span data-ttu-id="a0a35-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0a35-133">String</span></span>|<span data-ttu-id="a0a35-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0a35-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a0a35-135">descrição</span><span class="sxs-lookup"><span data-stu-id="a0a35-135">description</span></span>|<span data-ttu-id="a0a35-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0a35-136">String</span></span>|<span data-ttu-id="a0a35-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0a35-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a0a35-138">prioridade</span><span class="sxs-lookup"><span data-stu-id="a0a35-138">priority</span></span>|<span data-ttu-id="a0a35-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a0a35-139">Int32</span></span>|<span data-ttu-id="a0a35-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0a35-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a0a35-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0a35-141">createdDateTime</span></span>|<span data-ttu-id="a0a35-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0a35-142">DateTimeOffset</span></span>|<span data-ttu-id="a0a35-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0a35-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a0a35-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0a35-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a0a35-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0a35-145">DateTimeOffset</span></span>|<span data-ttu-id="a0a35-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0a35-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a0a35-147">version</span><span class="sxs-lookup"><span data-stu-id="a0a35-147">version</span></span>|<span data-ttu-id="a0a35-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a0a35-148">Int32</span></span>|<span data-ttu-id="a0a35-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0a35-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a0a35-150">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="a0a35-150">iosRestriction</span></span>|[<span data-ttu-id="a0a35-151">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a0a35-151">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a0a35-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a0a35-152">Not yet documented</span></span>|
|<span data-ttu-id="a0a35-153">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="a0a35-153">windowsRestriction</span></span>|[<span data-ttu-id="a0a35-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a0a35-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a0a35-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a0a35-155">Not yet documented</span></span>|
|<span data-ttu-id="a0a35-156">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="a0a35-156">windowsMobileRestriction</span></span>|[<span data-ttu-id="a0a35-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a0a35-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a0a35-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a0a35-158">Not yet documented</span></span>|
|<span data-ttu-id="a0a35-159">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="a0a35-159">androidRestriction</span></span>|[<span data-ttu-id="a0a35-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a0a35-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a0a35-161">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a0a35-161">Not yet documented</span></span>|
|<span data-ttu-id="a0a35-162">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="a0a35-162">macOSRestriction</span></span>|[<span data-ttu-id="a0a35-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a0a35-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="a0a35-164">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a0a35-164">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a0a35-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0a35-165">Response</span></span>
<span data-ttu-id="a0a35-166">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0a35-166">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0a35-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0a35-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0a35-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0a35-168">Request</span></span>
<span data-ttu-id="a0a35-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0a35-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 1714

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
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

### <a name="response"></a><span data-ttu-id="a0a35-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0a35-170">Response</span></span>
<span data-ttu-id="a0a35-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0a35-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








