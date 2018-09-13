# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="37440-101">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="37440-101">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="37440-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="37440-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37440-103">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="37440-103">Create a new [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37440-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37440-104">Prerequisites</span></span>
<span data-ttu-id="37440-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="37440-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="37440-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37440-107">Permission type</span></span>|<span data-ttu-id="37440-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37440-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37440-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37440-109">Delegated (work or school account)</span></span>|<span data-ttu-id="37440-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37440-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="37440-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37440-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37440-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37440-112">Not supported.</span></span>|
|<span data-ttu-id="37440-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37440-113">Application</span></span>|<span data-ttu-id="37440-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37440-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37440-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37440-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="37440-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37440-116">Request headers</span></span>
|<span data-ttu-id="37440-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37440-117">Header</span></span>|<span data-ttu-id="37440-118">Valor</span><span class="sxs-lookup"><span data-stu-id="37440-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37440-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="37440-119">Authorization</span></span>|<span data-ttu-id="37440-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="37440-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37440-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37440-121">Accept</span></span>|<span data-ttu-id="37440-122">application/json</span><span class="sxs-lookup"><span data-stu-id="37440-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37440-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37440-123">Request body</span></span>
<span data-ttu-id="37440-124">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="37440-124">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="37440-125">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="37440-125">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="37440-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37440-126">Property</span></span>|<span data-ttu-id="37440-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="37440-127">Type</span></span>|<span data-ttu-id="37440-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="37440-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37440-129">id</span><span class="sxs-lookup"><span data-stu-id="37440-129">id</span></span>|<span data-ttu-id="37440-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37440-130">String</span></span>|<span data-ttu-id="37440-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="37440-131">Not yet documented</span></span>|
|<span data-ttu-id="37440-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="37440-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="37440-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37440-133">DateTimeOffset</span></span>|<span data-ttu-id="37440-134">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="37440-134">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="37440-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="37440-135">partnerState</span></span>|[<span data-ttu-id="37440-136">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="37440-136">mobileThreatPartnerTenantState</span></span>](../resources/intune_onboarding_mobilethreatpartnertenantstate.md)|<span data-ttu-id="37440-p102">Estado do Parceiro de Sincronização de Dados para essa conta. Os valores possíveis são: `unavailable` `available` `enabled` `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="37440-p102">Data Sync Partner state for this account Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="37440-139">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="37440-139">androidEnabled</span></span>|<span data-ttu-id="37440-140">Booleano</span><span class="sxs-lookup"><span data-stu-id="37440-140">Boolean</span></span>|<span data-ttu-id="37440-141">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="37440-141">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="37440-142">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="37440-142">iosEnabled</span></span>|<span data-ttu-id="37440-143">Booleano</span><span class="sxs-lookup"><span data-stu-id="37440-143">Boolean</span></span>|<span data-ttu-id="37440-144">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="37440-144">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="37440-145">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="37440-145">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="37440-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="37440-146">Boolean</span></span>|<span data-ttu-id="37440-147">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="37440-147">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="37440-148">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="37440-148">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="37440-149">Booleano</span><span class="sxs-lookup"><span data-stu-id="37440-149">Boolean</span></span>|<span data-ttu-id="37440-150">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="37440-150">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="37440-151">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="37440-151">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="37440-152">Booleano</span><span class="sxs-lookup"><span data-stu-id="37440-152">Boolean</span></span>|<span data-ttu-id="37440-153">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="37440-153">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="37440-154">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="37440-154">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="37440-155">Int32</span><span class="sxs-lookup"><span data-stu-id="37440-155">Int32</span></span>|<span data-ttu-id="37440-156">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="37440-156">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="37440-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="37440-157">Response</span></span>
<span data-ttu-id="37440-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37440-158">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37440-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37440-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="37440-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37440-160">Request</span></span>
<span data-ttu-id="37440-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37440-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="37440-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="37440-162">Response</span></span>
<span data-ttu-id="37440-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37440-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```








