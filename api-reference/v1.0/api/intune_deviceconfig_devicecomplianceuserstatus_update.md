# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="b1e4e-101">Atualizar deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="b1e4e-101">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="b1e4e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1e4e-103">Atualizar as propriedades de um objeto [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b1e4e-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1e4e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1e4e-104">Prerequisites</span></span>
<span data-ttu-id="b1e4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1e4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1e4e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1e4e-107">Permission type</span></span>|<span data-ttu-id="b1e4e-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1e4e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1e4e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1e4e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b1e4e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1e4e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1e4e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1e4e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1e4e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-112">Not supported.</span></span>|
|<span data-ttu-id="b1e4e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1e4e-113">Application</span></span>|<span data-ttu-id="b1e4e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1e4e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1e4e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b1e4e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e4e-116">Request headers</span></span>
|<span data-ttu-id="b1e4e-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1e4e-117">Header</span></span>|<span data-ttu-id="b1e4e-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b1e4e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1e4e-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1e4e-119">Authorization</span></span>|<span data-ttu-id="b1e4e-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b1e4e-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1e4e-121">Accept</span></span>|<span data-ttu-id="b1e4e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b1e4e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1e4e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e4e-123">Request body</span></span>
<span data-ttu-id="b1e4e-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b1e4e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="b1e4e-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b1e4e-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="b1e4e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1e4e-126">Property</span></span>|<span data-ttu-id="b1e4e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1e4e-127">Type</span></span>|<span data-ttu-id="b1e4e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1e4e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1e4e-129">id</span><span class="sxs-lookup"><span data-stu-id="b1e4e-129">id</span></span>|<span data-ttu-id="b1e4e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e4e-130">String</span></span>|<span data-ttu-id="b1e4e-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-131">Key of the setting.</span></span>|
|<span data-ttu-id="b1e4e-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1e4e-132">userDisplayName</span></span>|<span data-ttu-id="b1e4e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e4e-133">String</span></span>|<span data-ttu-id="b1e4e-134">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b1e4e-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="b1e4e-135">devicesCount</span></span>|<span data-ttu-id="b1e4e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b1e4e-136">Int32</span></span>|<span data-ttu-id="b1e4e-137">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-137">Devices count for that user.</span></span>|
|<span data-ttu-id="b1e4e-138">status</span><span class="sxs-lookup"><span data-stu-id="b1e4e-138">status</span></span>|<span data-ttu-id="b1e4e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e4e-139">String</span></span>|<span data-ttu-id="b1e4e-140">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-140">Compliance status of the policy report.</span></span> <span data-ttu-id="b1e4e-141">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="b1e4e-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1e4e-142">lastReportedDateTime</span></span>|<span data-ttu-id="b1e4e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1e4e-143">DateTimeOffset</span></span>|<span data-ttu-id="b1e4e-144">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b1e4e-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1e4e-145">userPrincipalName</span></span>|<span data-ttu-id="b1e4e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e4e-146">String</span></span>|<span data-ttu-id="b1e4e-147">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-147">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="b1e4e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1e4e-148">Response</span></span>
<span data-ttu-id="b1e4e-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1e4e-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1e4e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1e4e-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e4e-151">Request</span></span>
<span data-ttu-id="b1e4e-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
Content-type: application/json
Content-length: 222

{
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="b1e4e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1e4e-153">Response</span></span>
<span data-ttu-id="b1e4e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1e4e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



