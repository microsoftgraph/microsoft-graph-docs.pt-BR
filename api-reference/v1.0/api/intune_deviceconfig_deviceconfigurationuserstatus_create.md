# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="83072-101">Criar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="83072-101">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="83072-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="83072-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83072-103">Criar um novo objeto [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="83072-103">Create a new [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83072-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83072-104">Prerequisites</span></span>
<span data-ttu-id="83072-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="83072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="83072-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83072-107">Permission type</span></span>|<span data-ttu-id="83072-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="83072-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83072-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83072-109">Delegated (work or school account)</span></span>|<span data-ttu-id="83072-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83072-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83072-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83072-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83072-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83072-112">Not supported.</span></span>|
|<span data-ttu-id="83072-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83072-113">Application</span></span>|<span data-ttu-id="83072-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83072-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83072-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83072-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="83072-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83072-116">Request headers</span></span>
|<span data-ttu-id="83072-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83072-117">Header</span></span>|<span data-ttu-id="83072-118">Valor</span><span class="sxs-lookup"><span data-stu-id="83072-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83072-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="83072-119">Authorization</span></span>|<span data-ttu-id="83072-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="83072-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83072-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83072-121">Accept</span></span>|<span data-ttu-id="83072-122">application/json</span><span class="sxs-lookup"><span data-stu-id="83072-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83072-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83072-123">Request body</span></span>
<span data-ttu-id="83072-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="83072-124">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="83072-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="83072-125">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="83072-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83072-126">Property</span></span>|<span data-ttu-id="83072-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="83072-127">Type</span></span>|<span data-ttu-id="83072-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="83072-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83072-129">id</span><span class="sxs-lookup"><span data-stu-id="83072-129">id</span></span>|<span data-ttu-id="83072-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83072-130">String</span></span>|<span data-ttu-id="83072-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="83072-131">Key of the entity.</span></span>|
|<span data-ttu-id="83072-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="83072-132">userDisplayName</span></span>|<span data-ttu-id="83072-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83072-133">String</span></span>|<span data-ttu-id="83072-134">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="83072-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="83072-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="83072-135">devicesCount</span></span>|<span data-ttu-id="83072-136">Int32</span><span class="sxs-lookup"><span data-stu-id="83072-136">Int32</span></span>|<span data-ttu-id="83072-137">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="83072-137">Devices count for that user.</span></span>|
|<span data-ttu-id="83072-138">status</span><span class="sxs-lookup"><span data-stu-id="83072-138">status</span></span>|[<span data-ttu-id="83072-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="83072-139">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="83072-140">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="83072-140">Compliance status of the policy report.</span></span> <span data-ttu-id="83072-141">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="83072-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="83072-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="83072-142">lastReportedDateTime</span></span>|<span data-ttu-id="83072-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83072-143">DateTimeOffset</span></span>|<span data-ttu-id="83072-144">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="83072-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="83072-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="83072-145">userPrincipalName</span></span>|<span data-ttu-id="83072-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83072-146">String</span></span>|<span data-ttu-id="83072-147">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="83072-147">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="83072-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="83072-148">Response</span></span>
<span data-ttu-id="83072-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83072-149">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83072-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83072-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="83072-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83072-151">Request</span></span>
<span data-ttu-id="83072-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83072-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="83072-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="83072-153">Response</span></span>
<span data-ttu-id="83072-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83072-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








