# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="c1a0f-101">Criar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="c1a0f-101">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="c1a0f-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1a0f-103">Criar um novo objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c1a0f-103">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1a0f-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1a0f-104">Prerequisites</span></span>
<span data-ttu-id="c1a0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1a0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c1a0f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1a0f-107">Permission type</span></span>|<span data-ttu-id="c1a0f-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1a0f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1a0f-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1a0f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c1a0f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a0f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c1a0f-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1a0f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1a0f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-112">Not supported.</span></span>|
|<span data-ttu-id="c1a0f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1a0f-113">Application</span></span>|<span data-ttu-id="c1a0f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1a0f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a0f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c1a0f-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a0f-116">Request headers</span></span>
|<span data-ttu-id="c1a0f-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1a0f-117">Header</span></span>|<span data-ttu-id="c1a0f-118">Valor</span><span class="sxs-lookup"><span data-stu-id="c1a0f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1a0f-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1a0f-119">Authorization</span></span>|<span data-ttu-id="c1a0f-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1a0f-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1a0f-121">Accept</span></span>|<span data-ttu-id="c1a0f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c1a0f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1a0f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a0f-123">Request body</span></span>
<span data-ttu-id="c1a0f-124">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-124">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="c1a0f-125">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-125">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="c1a0f-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1a0f-126">Property</span></span>|<span data-ttu-id="c1a0f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1a0f-127">Type</span></span>|<span data-ttu-id="c1a0f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1a0f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1a0f-129">id</span><span class="sxs-lookup"><span data-stu-id="c1a0f-129">id</span></span>|<span data-ttu-id="c1a0f-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1a0f-130">String</span></span>|<span data-ttu-id="c1a0f-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-131">Key of the entity.</span></span>|
|<span data-ttu-id="c1a0f-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c1a0f-132">userDisplayName</span></span>|<span data-ttu-id="c1a0f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1a0f-133">String</span></span>|<span data-ttu-id="c1a0f-134">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="c1a0f-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="c1a0f-135">devicesCount</span></span>|<span data-ttu-id="c1a0f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c1a0f-136">Int32</span></span>|<span data-ttu-id="c1a0f-137">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-137">Devices count for that user.</span></span>|
|<span data-ttu-id="c1a0f-138">status</span><span class="sxs-lookup"><span data-stu-id="c1a0f-138">status</span></span>|[<span data-ttu-id="c1a0f-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c1a0f-139">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="c1a0f-140">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-140">Compliance status of the policy report.</span></span> <span data-ttu-id="c1a0f-141">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c1a0f-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1a0f-142">lastReportedDateTime</span></span>|<span data-ttu-id="c1a0f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1a0f-143">DateTimeOffset</span></span>|<span data-ttu-id="c1a0f-144">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="c1a0f-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c1a0f-145">userPrincipalName</span></span>|<span data-ttu-id="c1a0f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1a0f-146">String</span></span>|<span data-ttu-id="c1a0f-147">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-147">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="c1a0f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1a0f-148">Response</span></span>
<span data-ttu-id="c1a0f-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-149">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1a0f-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1a0f-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1a0f-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a0f-151">Request</span></span>
<span data-ttu-id="c1a0f-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="c1a0f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1a0f-153">Response</span></span>
<span data-ttu-id="c1a0f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1a0f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



