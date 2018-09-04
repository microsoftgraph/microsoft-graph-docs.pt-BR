# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="741f7-101">Criar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="741f7-101">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="741f7-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="741f7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="741f7-103">Criar um novo objeto [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="741f7-103">Create a new [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="741f7-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="741f7-104">Prerequisites</span></span>
<span data-ttu-id="741f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="741f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="741f7-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="741f7-107">Permission type</span></span>|<span data-ttu-id="741f7-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="741f7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="741f7-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="741f7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="741f7-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="741f7-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="741f7-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="741f7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="741f7-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="741f7-112">Not supported.</span></span>|
|<span data-ttu-id="741f7-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="741f7-113">Application</span></span>|<span data-ttu-id="741f7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="741f7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="741f7-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="741f7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="741f7-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="741f7-116">Request headers</span></span>
|<span data-ttu-id="741f7-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="741f7-117">Header</span></span>|<span data-ttu-id="741f7-118">Valor</span><span class="sxs-lookup"><span data-stu-id="741f7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="741f7-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="741f7-119">Authorization</span></span>|<span data-ttu-id="741f7-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="741f7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="741f7-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="741f7-121">Accept</span></span>|<span data-ttu-id="741f7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="741f7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="741f7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="741f7-123">Request body</span></span>
<span data-ttu-id="741f7-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="741f7-124">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="741f7-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="741f7-125">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="741f7-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="741f7-126">Property</span></span>|<span data-ttu-id="741f7-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="741f7-127">Type</span></span>|<span data-ttu-id="741f7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="741f7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="741f7-129">id</span><span class="sxs-lookup"><span data-stu-id="741f7-129">id</span></span>|<span data-ttu-id="741f7-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="741f7-130">String</span></span>|<span data-ttu-id="741f7-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="741f7-131">Key of the entity.</span></span>|
|<span data-ttu-id="741f7-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="741f7-132">deviceDisplayName</span></span>|<span data-ttu-id="741f7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="741f7-133">String</span></span>|<span data-ttu-id="741f7-134">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="741f7-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="741f7-135">userName</span><span class="sxs-lookup"><span data-stu-id="741f7-135">userName</span></span>|<span data-ttu-id="741f7-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="741f7-136">String</span></span>|<span data-ttu-id="741f7-137">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="741f7-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="741f7-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="741f7-138">deviceModel</span></span>|<span data-ttu-id="741f7-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="741f7-139">String</span></span>|<span data-ttu-id="741f7-140">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="741f7-140">The device model that is being reported</span></span>|
|<span data-ttu-id="741f7-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="741f7-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="741f7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="741f7-142">DateTimeOffset</span></span>|<span data-ttu-id="741f7-143">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="741f7-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="741f7-144">status</span><span class="sxs-lookup"><span data-stu-id="741f7-144">status</span></span>|[<span data-ttu-id="741f7-145">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="741f7-145">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="741f7-146">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="741f7-146">Compliance status of the policy report.</span></span> <span data-ttu-id="741f7-147">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="741f7-147">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="741f7-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="741f7-148">lastReportedDateTime</span></span>|<span data-ttu-id="741f7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="741f7-149">DateTimeOffset</span></span>|<span data-ttu-id="741f7-150">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="741f7-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="741f7-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="741f7-151">userPrincipalName</span></span>|<span data-ttu-id="741f7-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="741f7-152">String</span></span>|<span data-ttu-id="741f7-153">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="741f7-153">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="741f7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="741f7-154">Response</span></span>
<span data-ttu-id="741f7-155">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="741f7-155">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="741f7-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="741f7-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="741f7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="741f7-157">Request</span></span>
<span data-ttu-id="741f7-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="741f7-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="741f7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="741f7-159">Response</span></span>
<span data-ttu-id="741f7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="741f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



