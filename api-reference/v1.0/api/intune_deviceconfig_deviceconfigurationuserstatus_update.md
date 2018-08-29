# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="97a74-101">Atualizar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="97a74-101">Update deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="97a74-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="97a74-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97a74-103">Atualizar as propriedades de um objeto [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="97a74-103">Update the properties of a [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97a74-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97a74-104">Prerequisites</span></span>
<span data-ttu-id="97a74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97a74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97a74-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97a74-107">Permission type</span></span>|<span data-ttu-id="97a74-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97a74-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97a74-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97a74-109">Delegated (work or school account)</span></span>|<span data-ttu-id="97a74-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97a74-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97a74-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97a74-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97a74-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97a74-112">Not supported.</span></span>|
|<span data-ttu-id="97a74-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97a74-113">Application</span></span>|<span data-ttu-id="97a74-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97a74-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97a74-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97a74-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="97a74-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97a74-116">Request headers</span></span>
|<span data-ttu-id="97a74-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97a74-117">Header</span></span>|<span data-ttu-id="97a74-118">Valor</span><span class="sxs-lookup"><span data-stu-id="97a74-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97a74-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="97a74-119">Authorization</span></span>|<span data-ttu-id="97a74-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="97a74-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97a74-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97a74-121">Accept</span></span>|<span data-ttu-id="97a74-122">application/json</span><span class="sxs-lookup"><span data-stu-id="97a74-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97a74-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97a74-123">Request body</span></span>
<span data-ttu-id="97a74-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="97a74-124">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="97a74-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="97a74-125">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="97a74-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97a74-126">Property</span></span>|<span data-ttu-id="97a74-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="97a74-127">Type</span></span>|<span data-ttu-id="97a74-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="97a74-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97a74-129">id</span><span class="sxs-lookup"><span data-stu-id="97a74-129">id</span></span>|<span data-ttu-id="97a74-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97a74-130">String</span></span>|<span data-ttu-id="97a74-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="97a74-131">Key of the entity.</span></span>|
|<span data-ttu-id="97a74-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="97a74-132">userDisplayName</span></span>|<span data-ttu-id="97a74-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97a74-133">String</span></span>|<span data-ttu-id="97a74-134">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="97a74-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="97a74-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="97a74-135">devicesCount</span></span>|<span data-ttu-id="97a74-136">Int32</span><span class="sxs-lookup"><span data-stu-id="97a74-136">Int32</span></span>|<span data-ttu-id="97a74-137">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="97a74-137">Devices count for that user.</span></span>|
|<span data-ttu-id="97a74-138">status</span><span class="sxs-lookup"><span data-stu-id="97a74-138">status</span></span>|[<span data-ttu-id="97a74-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="97a74-139">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="97a74-140">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="97a74-140">Compliance status of the policy report.</span></span> <span data-ttu-id="97a74-141">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="97a74-141">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="97a74-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="97a74-142">lastReportedDateTime</span></span>|<span data-ttu-id="97a74-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97a74-143">DateTimeOffset</span></span>|<span data-ttu-id="97a74-144">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="97a74-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="97a74-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="97a74-145">userPrincipalName</span></span>|<span data-ttu-id="97a74-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97a74-146">String</span></span>|<span data-ttu-id="97a74-147">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="97a74-147">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="97a74-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="97a74-148">Response</span></span>
<span data-ttu-id="97a74-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97a74-149">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97a74-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97a74-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="97a74-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97a74-151">Request</span></span>
<span data-ttu-id="97a74-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97a74-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
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

### <a name="response"></a><span data-ttu-id="97a74-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="97a74-153">Response</span></span>
<span data-ttu-id="97a74-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97a74-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



