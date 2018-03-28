# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="bc14e-101">Criar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="bc14e-101">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="bc14e-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bc14e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc14e-103">Crie um novo objeto [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="bc14e-103">Create a new [plannerBucket](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc14e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc14e-104">Prerequisites</span></span>
<span data-ttu-id="bc14e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc14e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bc14e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc14e-107">Permission type</span></span>|<span data-ttu-id="bc14e-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc14e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc14e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc14e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bc14e-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc14e-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bc14e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc14e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc14e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc14e-112">Not supported.</span></span>|
|<span data-ttu-id="bc14e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc14e-113">Application</span></span>|<span data-ttu-id="bc14e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc14e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc14e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc14e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="bc14e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc14e-116">Request headers</span></span>
|<span data-ttu-id="bc14e-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc14e-117">Header</span></span>|<span data-ttu-id="bc14e-118">Valor</span><span class="sxs-lookup"><span data-stu-id="bc14e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc14e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc14e-119">Authorization</span></span>|<span data-ttu-id="bc14e-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc14e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bc14e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="bc14e-121">Accept</span></span>|<span data-ttu-id="bc14e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bc14e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc14e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc14e-123">Request body</span></span>
<span data-ttu-id="bc14e-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="bc14e-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="bc14e-125">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="bc14e-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="bc14e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc14e-126">Property</span></span>|<span data-ttu-id="bc14e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc14e-127">Type</span></span>|<span data-ttu-id="bc14e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc14e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc14e-129">id</span><span class="sxs-lookup"><span data-stu-id="bc14e-129">id</span></span>|<span data-ttu-id="bc14e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc14e-130">String</span></span>|<span data-ttu-id="bc14e-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bc14e-131">Not yet documented</span></span>|
|<span data-ttu-id="bc14e-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bc14e-132">lastSyncDateTime</span></span>|<span data-ttu-id="bc14e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc14e-133">DateTimeOffset</span></span>|<span data-ttu-id="bc14e-134">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="bc14e-134">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="bc14e-135">status</span><span class="sxs-lookup"><span data-stu-id="bc14e-135">status</span></span>|<span data-ttu-id="bc14e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc14e-136">String</span></span>|<span data-ttu-id="bc14e-137">Status do Exchange Connector Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="bc14e-137">Exchange Connector Status Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="bc14e-138">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="bc14e-138">primarySmtpAddress</span></span>|<span data-ttu-id="bc14e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc14e-139">String</span></span>|<span data-ttu-id="bc14e-140">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="bc14e-140">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="bc14e-141">serverName</span><span class="sxs-lookup"><span data-stu-id="bc14e-141">ServerName</span></span>|<span data-ttu-id="bc14e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc14e-142">String</span></span>|<span data-ttu-id="bc14e-143">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="bc14e-143">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="bc14e-144">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="bc14e-144">exchangeConnectorType</span></span>|<span data-ttu-id="bc14e-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc14e-145">String</span></span>|<span data-ttu-id="bc14e-146">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="bc14e-146">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="bc14e-147">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="bc14e-147">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="bc14e-148">version</span><span class="sxs-lookup"><span data-stu-id="bc14e-148">version</span></span>|<span data-ttu-id="bc14e-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc14e-149">String</span></span>|<span data-ttu-id="bc14e-150">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="bc14e-150">The version of the message.</span></span>|
|<span data-ttu-id="bc14e-151">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="bc14e-151">exchangeAlias</span></span>|<span data-ttu-id="bc14e-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc14e-152">String</span></span>|<span data-ttu-id="bc14e-153">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="bc14e-153">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="bc14e-154">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="bc14e-154">exchangeOrganization</span></span>|<span data-ttu-id="bc14e-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc14e-155">String</span></span>|<span data-ttu-id="bc14e-156">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="bc14e-156">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="bc14e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc14e-157">Response</span></span>
<span data-ttu-id="bc14e-158">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc14e-158">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc14e-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc14e-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc14e-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc14e-160">Request</span></span>
<span data-ttu-id="bc14e-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc14e-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 433

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="bc14e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc14e-162">Response</span></span>
<span data-ttu-id="bc14e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc14e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 482

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```



