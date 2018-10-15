# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="aace5-101">Atualizar managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="aace5-101">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="aace5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="aace5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aace5-103">Atualizar as propriedades de um objeto [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="aace5-103">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aace5-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aace5-104">Prerequisites</span></span>
<span data-ttu-id="aace5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aace5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aace5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aace5-107">Permission type</span></span>|<span data-ttu-id="aace5-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aace5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aace5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aace5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="aace5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aace5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aace5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aace5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aace5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aace5-112">Not supported.</span></span>|
|<span data-ttu-id="aace5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aace5-113">Application</span></span>|<span data-ttu-id="aace5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aace5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aace5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aace5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="request-headers"></a><span data-ttu-id="aace5-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aace5-116">Request headers</span></span>
|<span data-ttu-id="aace5-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aace5-117">Header</span></span>|<span data-ttu-id="aace5-118">Valor</span><span class="sxs-lookup"><span data-stu-id="aace5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aace5-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="aace5-119">Authorization</span></span>|<span data-ttu-id="aace5-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="aace5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aace5-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aace5-121">Accept</span></span>|<span data-ttu-id="aace5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="aace5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aace5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aace5-123">Request body</span></span>
<span data-ttu-id="aace5-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="aace5-124">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="aace5-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="aace5-125">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="aace5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aace5-126">Property</span></span>|<span data-ttu-id="aace5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="aace5-127">Type</span></span>|<span data-ttu-id="aace5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="aace5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aace5-129">displayName</span><span class="sxs-lookup"><span data-stu-id="aace5-129">displayName</span></span>|<span data-ttu-id="aace5-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aace5-130">String</span></span>|<span data-ttu-id="aace5-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="aace5-131">Not yet documented</span></span>|
|<span data-ttu-id="aace5-132">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="aace5-132">configurationDeployedUserCount</span></span>|<span data-ttu-id="aace5-133">Int32</span><span class="sxs-lookup"><span data-stu-id="aace5-133">Int32</span></span>|<span data-ttu-id="aace5-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="aace5-134">Not yet documented</span></span>|
|<span data-ttu-id="aace5-135">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="aace5-135">lastRefreshTime</span></span>|<span data-ttu-id="aace5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aace5-136">DateTimeOffset</span></span>|<span data-ttu-id="aace5-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="aace5-137">Not yet documented</span></span>|
|<span data-ttu-id="aace5-138">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="aace5-138">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="aace5-139">Conjunto [managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="aace5-139">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="aace5-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="aace5-140">Not yet documented</span></span>|
|<span data-ttu-id="aace5-141">id</span><span class="sxs-lookup"><span data-stu-id="aace5-141">id</span></span>|<span data-ttu-id="aace5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aace5-142">String</span></span>|<span data-ttu-id="aace5-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aace5-143">Key of the entity.</span></span>|
|<span data-ttu-id="aace5-144">version</span><span class="sxs-lookup"><span data-stu-id="aace5-144">version</span></span>|<span data-ttu-id="aace5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aace5-145">String</span></span>|<span data-ttu-id="aace5-146">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="aace5-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="aace5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="aace5-147">Response</span></span>
<span data-ttu-id="aace5-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aace5-148">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aace5-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aace5-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="aace5-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aace5-150">Request</span></span>
<span data-ttu-id="aace5-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aace5-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 516

{
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="aace5-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="aace5-152">Response</span></span>
<span data-ttu-id="aace5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aace5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
  "version": "Version value"
}
```








