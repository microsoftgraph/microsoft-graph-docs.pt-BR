# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="c5422-101">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="c5422-101">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="c5422-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c5422-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5422-103">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="c5422-103">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5422-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5422-104">Prerequisites</span></span>
<span data-ttu-id="c5422-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c5422-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5422-107">Permission type</span></span>|<span data-ttu-id="c5422-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5422-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5422-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5422-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c5422-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5422-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5422-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5422-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5422-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5422-112">Not supported.</span></span>|
|<span data-ttu-id="c5422-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5422-113">Application</span></span>|<span data-ttu-id="c5422-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5422-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5422-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5422-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="c5422-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5422-116">Request headers</span></span>
|<span data-ttu-id="c5422-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5422-117">Header</span></span>|<span data-ttu-id="c5422-118">Valor</span><span class="sxs-lookup"><span data-stu-id="c5422-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5422-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5422-119">Authorization</span></span>|<span data-ttu-id="c5422-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="c5422-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5422-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5422-121">Accept</span></span>|<span data-ttu-id="c5422-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c5422-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5422-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5422-123">Request body</span></span>
<span data-ttu-id="c5422-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="c5422-124">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="c5422-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="c5422-125">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="c5422-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5422-126">Property</span></span>|<span data-ttu-id="c5422-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5422-127">Type</span></span>|<span data-ttu-id="c5422-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5422-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5422-129">id</span><span class="sxs-lookup"><span data-stu-id="c5422-129">id</span></span>|<span data-ttu-id="c5422-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5422-130">String</span></span>|<span data-ttu-id="c5422-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c5422-131">Key of the entity.</span></span>|
|<span data-ttu-id="c5422-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="c5422-132">pendingCount</span></span>|<span data-ttu-id="c5422-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c5422-133">Int32</span></span>|<span data-ttu-id="c5422-134">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="c5422-134">Number of pending Users</span></span>|
|<span data-ttu-id="c5422-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c5422-135">notApplicableCount</span></span>|<span data-ttu-id="c5422-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c5422-136">Int32</span></span>|<span data-ttu-id="c5422-137">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="c5422-137">Number of not applicable users.</span></span>|
|<span data-ttu-id="c5422-138">successCount</span><span class="sxs-lookup"><span data-stu-id="c5422-138">successCount</span></span>|<span data-ttu-id="c5422-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c5422-139">Int32</span></span>|<span data-ttu-id="c5422-140">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="c5422-140">Number of succeeded Users</span></span>|
|<span data-ttu-id="c5422-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="c5422-141">errorCount</span></span>|<span data-ttu-id="c5422-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c5422-142">Int32</span></span>|<span data-ttu-id="c5422-143">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="c5422-143">Number of error Users</span></span>|
|<span data-ttu-id="c5422-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="c5422-144">failedCount</span></span>|<span data-ttu-id="c5422-145">Int32</span><span class="sxs-lookup"><span data-stu-id="c5422-145">Int32</span></span>|<span data-ttu-id="c5422-146">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="c5422-146">Number of failed Users</span></span>|
|<span data-ttu-id="c5422-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="c5422-147">lastUpdateDateTime</span></span>|<span data-ttu-id="c5422-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5422-148">DateTimeOffset</span></span>|<span data-ttu-id="c5422-149">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="c5422-149">Last update time</span></span>|
|<span data-ttu-id="c5422-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="c5422-150">configurationVersion</span></span>|<span data-ttu-id="c5422-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c5422-151">Int32</span></span>|<span data-ttu-id="c5422-152">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="c5422-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="c5422-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5422-153">Response</span></span>
<span data-ttu-id="c5422-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5422-154">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5422-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5422-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5422-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5422-156">Request</span></span>
<span data-ttu-id="c5422-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5422-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 212

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="c5422-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5422-158">Response</span></span>
<span data-ttu-id="c5422-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5422-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```








