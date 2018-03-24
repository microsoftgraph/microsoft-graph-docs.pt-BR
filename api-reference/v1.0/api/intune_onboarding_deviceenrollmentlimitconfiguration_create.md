# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="3e4e9-101">Criar deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e4e9-101">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="3e4e9-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3e4e9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e4e9-103">Criar um novo objeto [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e4e9-103">Create a new [plannerBucket](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e4e9-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e4e9-104">Prerequisites</span></span>
<span data-ttu-id="3e4e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3e4e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3e4e9-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e4e9-107">Permission type</span></span>|<span data-ttu-id="3e4e9-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3e4e9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e4e9-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e4e9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3e4e9-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e4e9-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3e4e9-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e4e9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e4e9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e4e9-112">Not supported.</span></span>|
|<span data-ttu-id="3e4e9-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e4e9-113">Application</span></span>|<span data-ttu-id="3e4e9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e4e9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e4e9-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e4e9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3e4e9-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e4e9-116">Request headers</span></span>
|<span data-ttu-id="3e4e9-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e4e9-117">Header</span></span>|<span data-ttu-id="3e4e9-118">Valor</span><span class="sxs-lookup"><span data-stu-id="3e4e9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e4e9-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e4e9-119">Authorization</span></span>|<span data-ttu-id="3e4e9-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e4e9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3e4e9-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3e4e9-121">Accept</span></span>|<span data-ttu-id="3e4e9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3e4e9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e4e9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e4e9-123">Request body</span></span>
<span data-ttu-id="3e4e9-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3e4e9-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="3e4e9-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3e4e9-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="3e4e9-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e4e9-126">Property</span></span>|<span data-ttu-id="3e4e9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e4e9-127">Type</span></span>|<span data-ttu-id="3e4e9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e4e9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e4e9-129">id</span><span class="sxs-lookup"><span data-stu-id="3e4e9-129">id</span></span>|<span data-ttu-id="3e4e9-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e4e9-130">String</span></span>|<span data-ttu-id="3e4e9-131">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e4e9-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e4e9-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3e4e9-132">displayName</span></span>|<span data-ttu-id="3e4e9-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e4e9-133">String</span></span>|<span data-ttu-id="3e4e9-134">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e4e9-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e4e9-135">descrição</span><span class="sxs-lookup"><span data-stu-id="3e4e9-135">description</span></span>|<span data-ttu-id="3e4e9-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e4e9-136">String</span></span>|<span data-ttu-id="3e4e9-137">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e4e9-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e4e9-138">prioridade</span><span class="sxs-lookup"><span data-stu-id="3e4e9-138">priority</span></span>|<span data-ttu-id="3e4e9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4e9-139">Int32</span></span>|<span data-ttu-id="3e4e9-140">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e4e9-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e4e9-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e4e9-141">createdDateTime</span></span>|<span data-ttu-id="3e4e9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e4e9-142">DateTimeOffset</span></span>|<span data-ttu-id="3e4e9-143">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e4e9-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e4e9-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e4e9-144">lastModifiedDateTime</span></span>|<span data-ttu-id="3e4e9-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e4e9-145">DateTimeOffset</span></span>|<span data-ttu-id="3e4e9-146">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e4e9-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e4e9-147">version</span><span class="sxs-lookup"><span data-stu-id="3e4e9-147">version</span></span>|<span data-ttu-id="3e4e9-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4e9-148">Int32</span></span>|<span data-ttu-id="3e4e9-149">Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e4e9-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3e4e9-150">limite</span><span class="sxs-lookup"><span data-stu-id="3e4e9-150">Limit</span></span>|<span data-ttu-id="3e4e9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4e9-151">Int32</span></span>|<span data-ttu-id="3e4e9-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e4e9-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3e4e9-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e4e9-153">Response</span></span>
<span data-ttu-id="3e4e9-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e4e9-154">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e4e9-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e4e9-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e4e9-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e4e9-156">Request</span></span>
<span data-ttu-id="3e4e9-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e4e9-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="3e4e9-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e4e9-158">Response</span></span>
<span data-ttu-id="3e4e9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e4e9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



