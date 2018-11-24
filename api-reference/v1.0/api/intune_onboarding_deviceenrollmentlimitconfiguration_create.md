# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="d610a-101">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="d610a-101">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="d610a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d610a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d610a-103">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d610a-103">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d610a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d610a-104">Prerequisites</span></span>
<span data-ttu-id="d610a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d610a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d610a-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d610a-107">Permission type</span></span>|<span data-ttu-id="d610a-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d610a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d610a-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d610a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d610a-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d610a-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d610a-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d610a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d610a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d610a-112">Not supported.</span></span>|
|<span data-ttu-id="d610a-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d610a-113">Application</span></span>|<span data-ttu-id="d610a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d610a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d610a-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d610a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d610a-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d610a-116">Request headers</span></span>
|<span data-ttu-id="d610a-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d610a-117">Header</span></span>|<span data-ttu-id="d610a-118">Valor</span><span class="sxs-lookup"><span data-stu-id="d610a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d610a-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d610a-119">Authorization</span></span>|<span data-ttu-id="d610a-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d610a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d610a-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d610a-121">Accept</span></span>|<span data-ttu-id="d610a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d610a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d610a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d610a-123">Request body</span></span>
<span data-ttu-id="d610a-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d610a-124">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="d610a-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d610a-125">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="d610a-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d610a-126">Property</span></span>|<span data-ttu-id="d610a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d610a-127">Type</span></span>|<span data-ttu-id="d610a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d610a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d610a-129">id</span><span class="sxs-lookup"><span data-stu-id="d610a-129">id</span></span>|<span data-ttu-id="d610a-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d610a-130">String</span></span>|<span data-ttu-id="d610a-131">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d610a-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d610a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d610a-132">displayName</span></span>|<span data-ttu-id="d610a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d610a-133">String</span></span>|<span data-ttu-id="d610a-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d610a-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d610a-135">descrição</span><span class="sxs-lookup"><span data-stu-id="d610a-135">description</span></span>|<span data-ttu-id="d610a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d610a-136">String</span></span>|<span data-ttu-id="d610a-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d610a-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d610a-138">prioridade</span><span class="sxs-lookup"><span data-stu-id="d610a-138">priority</span></span>|<span data-ttu-id="d610a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d610a-139">Int32</span></span>|<span data-ttu-id="d610a-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d610a-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d610a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d610a-141">createdDateTime</span></span>|<span data-ttu-id="d610a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d610a-142">DateTimeOffset</span></span>|<span data-ttu-id="d610a-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d610a-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d610a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d610a-144">lastModifiedDateTime</span></span>|<span data-ttu-id="d610a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d610a-145">DateTimeOffset</span></span>|<span data-ttu-id="d610a-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d610a-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d610a-147">version</span><span class="sxs-lookup"><span data-stu-id="d610a-147">version</span></span>|<span data-ttu-id="d610a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d610a-148">Int32</span></span>|<span data-ttu-id="d610a-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d610a-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d610a-150">limite</span><span class="sxs-lookup"><span data-stu-id="d610a-150">limit</span></span>|<span data-ttu-id="d610a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d610a-151">Int32</span></span>|<span data-ttu-id="d610a-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d610a-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d610a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d610a-153">Response</span></span>
<span data-ttu-id="d610a-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d610a-154">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d610a-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d610a-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="d610a-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d610a-156">Request</span></span>
<span data-ttu-id="d610a-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d610a-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="d610a-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d610a-158">Response</span></span>
<span data-ttu-id="d610a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d610a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```



