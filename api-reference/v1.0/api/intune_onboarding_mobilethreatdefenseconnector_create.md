# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="cc133-101">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="cc133-101">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="cc133-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cc133-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc133-103">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="cc133-103">Create a new [plannerBucket](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cc133-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc133-104">Prerequisites</span></span>
<span data-ttu-id="cc133-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cc133-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc133-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc133-107">Permission type</span></span>|<span data-ttu-id="cc133-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc133-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc133-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc133-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cc133-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc133-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cc133-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc133-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc133-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc133-112">Not supported.</span></span>|
|<span data-ttu-id="cc133-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc133-113">Application</span></span>|<span data-ttu-id="cc133-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc133-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc133-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc133-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="cc133-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc133-116">Request headers</span></span>
|<span data-ttu-id="cc133-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc133-117">Header</span></span>|<span data-ttu-id="cc133-118">Valor</span><span class="sxs-lookup"><span data-stu-id="cc133-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc133-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc133-119">Authorization</span></span>|<span data-ttu-id="cc133-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc133-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cc133-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc133-121">Accept</span></span>|<span data-ttu-id="cc133-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cc133-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc133-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc133-123">Request body</span></span>
<span data-ttu-id="cc133-124">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="cc133-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="cc133-125">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="cc133-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="cc133-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc133-126">Property</span></span>|<span data-ttu-id="cc133-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc133-127">Type</span></span>|<span data-ttu-id="cc133-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc133-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc133-129">id</span><span class="sxs-lookup"><span data-stu-id="cc133-129">id</span></span>|<span data-ttu-id="cc133-130">String</span><span class="sxs-lookup"><span data-stu-id="cc133-130">String</span></span>|<span data-ttu-id="cc133-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cc133-131">Not yet documented</span></span>|
|<span data-ttu-id="cc133-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="cc133-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="cc133-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc133-133">DateTimeOffset</span></span>|<span data-ttu-id="cc133-134">Carimbo de data/hora da última pulsação após a opção habilitada pelo administrador Conectar-se ao MTP</span><span class="sxs-lookup"><span data-stu-id="cc133-134">Timestamp of last heartbeat after admin enabled option Connect to MTP</span></span>|
|<span data-ttu-id="cc133-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="cc133-135">partnerState</span></span>|<span data-ttu-id="cc133-136">String</span><span class="sxs-lookup"><span data-stu-id="cc133-136">String</span></span>|<span data-ttu-id="cc133-137">Estado do parceiro deste locatário. Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="cc133-137">Partner state of this tenant Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="cc133-138">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="cc133-138">androidEnabled</span></span>|<span data-ttu-id="cc133-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc133-139">Boolean</span></span>|<span data-ttu-id="cc133-140">Botão Ativar ou Desativar do Android</span><span class="sxs-lookup"><span data-stu-id="cc133-140">Android Toggle On or Off</span></span>|
|<span data-ttu-id="cc133-141">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="cc133-141">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="cc133-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc133-142">Boolean</span></span>|<span data-ttu-id="cc133-143">Para o Android, os administradores com permissão para configurar devem receber dados do parceiro de sincronização de dados antes de serem considerados compatíveis</span><span class="sxs-lookup"><span data-stu-id="cc133-143">For Android, Allows admin to config must receive data from the data sync partner prior to being considered compliant</span></span>|
|<span data-ttu-id="cc133-144">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="cc133-144">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="cc133-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc133-145">Boolean</span></span>|<span data-ttu-id="cc133-146">Para o iOS, os administradores com permissão para configurar devem receber dados do parceiro de sincronização de dados antes de serem considerados compatíveis</span><span class="sxs-lookup"><span data-stu-id="cc133-146">For IOS, Allows admin to config must receive data from the data sync partner prior to being considered compliant</span></span>|
|<span data-ttu-id="cc133-147">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="cc133-147">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="cc133-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc133-148">Boolean</span></span>|<span data-ttu-id="cc133-149">Permite que o administrador bloqueie dispositivos nas plataformas habilitadas que não atenderem aos requisitos de versão mínima</span><span class="sxs-lookup"><span data-stu-id="cc133-149">Allows admin to block devices on the enabled platforms that do not meet minimum version requirements</span></span>|
|<span data-ttu-id="cc133-150">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="cc133-150">iosEnabled</span></span>|<span data-ttu-id="cc133-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc133-151">Boolean</span></span>|<span data-ttu-id="cc133-152">Botão Ativar ou Desativar do iOS</span><span class="sxs-lookup"><span data-stu-id="cc133-152">IOS Toggle On or Off</span></span>|
|<span data-ttu-id="cc133-153">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="cc133-153">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="cc133-154">Int32</span><span class="sxs-lookup"><span data-stu-id="cc133-154">Int32</span></span>|<span data-ttu-id="cc133-155">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="cc133-155">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="cc133-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc133-156">Response</span></span>
<span data-ttu-id="cc133-157">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc133-157">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc133-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc133-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc133-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc133-159">Request</span></span>
<span data-ttu-id="cc133-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc133-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="cc133-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc133-161">Response</span></span>
<span data-ttu-id="cc133-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc133-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



