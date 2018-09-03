# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="88154-101">Atualizar deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="88154-101">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="88154-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="88154-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88154-103">Atualizar as propriedades de um objeto [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="88154-103">Update the properties of a [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88154-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88154-104">Prerequisites</span></span>
<span data-ttu-id="88154-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="88154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="88154-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88154-107">Permission type</span></span>|<span data-ttu-id="88154-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88154-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88154-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88154-109">Delegated (work or school account)</span></span>|<span data-ttu-id="88154-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88154-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="88154-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88154-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88154-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88154-112">Not supported.</span></span>|
|<span data-ttu-id="88154-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88154-113">Application</span></span>|<span data-ttu-id="88154-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88154-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88154-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88154-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="88154-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88154-116">Request headers</span></span>
|<span data-ttu-id="88154-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88154-117">Header</span></span>|<span data-ttu-id="88154-118">Valor</span><span class="sxs-lookup"><span data-stu-id="88154-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88154-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="88154-119">Authorization</span></span>|<span data-ttu-id="88154-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="88154-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88154-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88154-121">Accept</span></span>|<span data-ttu-id="88154-122">application/json</span><span class="sxs-lookup"><span data-stu-id="88154-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88154-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88154-123">Request body</span></span>
<span data-ttu-id="88154-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="88154-124">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="88154-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="88154-125">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="88154-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88154-126">Property</span></span>|<span data-ttu-id="88154-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="88154-127">Type</span></span>|<span data-ttu-id="88154-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="88154-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88154-129">id</span><span class="sxs-lookup"><span data-stu-id="88154-129">id</span></span>|<span data-ttu-id="88154-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88154-130">String</span></span>|<span data-ttu-id="88154-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="88154-131">Not yet documented</span></span>|
|<span data-ttu-id="88154-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="88154-132">lastSyncDateTime</span></span>|<span data-ttu-id="88154-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88154-133">DateTimeOffset</span></span>|<span data-ttu-id="88154-134">Hora da última sincronização do Exchange Connector</span><span class="sxs-lookup"><span data-stu-id="88154-134">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="88154-135">status</span><span class="sxs-lookup"><span data-stu-id="88154-135">status</span></span>|[<span data-ttu-id="88154-136">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="88154-136">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="88154-137">Status do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="88154-137">Exchange Connector Status Possible values are: , , , .</span></span> <span data-ttu-id="88154-138">Os valores possíveis são: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="88154-138">The possible values are `none`, `connectionPending`, `connected`, `disconnected`, , , , , , , , or .</span></span>|
|<span data-ttu-id="88154-139">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="88154-139">primarySmtpAddress</span></span>|<span data-ttu-id="88154-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88154-140">String</span></span>|<span data-ttu-id="88154-141">Endereço de email usado para configurar o serviço a serviço do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="88154-141">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="88154-142">serverName</span><span class="sxs-lookup"><span data-stu-id="88154-142">serverName</span></span>|<span data-ttu-id="88154-143">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="88154-143">String</span></span>|<span data-ttu-id="88154-144">O nome do servidor do Exchange.</span><span class="sxs-lookup"><span data-stu-id="88154-144">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="88154-145">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="88154-145">connectorServerName</span></span>|<span data-ttu-id="88154-146">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="88154-146">String</span></span>|<span data-ttu-id="88154-147">O nome do servidor que hospeda o Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="88154-147">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="88154-148">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="88154-148">exchangeConnectorType</span></span>|[<span data-ttu-id="88154-149">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="88154-149">deviceManagementExchangeConnectorType</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectortype.md)|<span data-ttu-id="88154-150">O tipo de Exchange Connector configurado.</span><span class="sxs-lookup"><span data-stu-id="88154-150">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="88154-151">Os valores possíveis são: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="88154-151">The possible values are `onPremises`, `hosted`, `serviceToService`, `dedicated`, , , , , , , , or .</span></span>|
|<span data-ttu-id="88154-152">versão</span><span class="sxs-lookup"><span data-stu-id="88154-152">version</span></span>|<span data-ttu-id="88154-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88154-153">String</span></span>|<span data-ttu-id="88154-154">A versão do ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="88154-154">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="88154-155">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="88154-155">exchangeAlias</span></span>|<span data-ttu-id="88154-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88154-156">String</span></span>|<span data-ttu-id="88154-157">Um alias atribuído a um servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="88154-157">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="88154-158">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="88154-158">exchangeOrganization</span></span>|<span data-ttu-id="88154-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88154-159">String</span></span>|<span data-ttu-id="88154-160">Organização do Exchange no servidor Exchange</span><span class="sxs-lookup"><span data-stu-id="88154-160">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="88154-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="88154-161">Response</span></span>
<span data-ttu-id="88154-162">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88154-162">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88154-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88154-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="88154-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88154-164">Request</span></span>
<span data-ttu-id="88154-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88154-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
Content-type: application/json
Content-length: 418

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="88154-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="88154-166">Response</span></span>
<span data-ttu-id="88154-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88154-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```



