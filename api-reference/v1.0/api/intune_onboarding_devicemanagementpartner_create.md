# <a name="create-devicemanagementpartner"></a><span data-ttu-id="4dad7-101">Criar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4dad7-101">Create deviceManagementPartner</span></span>

> <span data-ttu-id="4dad7-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4dad7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4dad7-103">Criar um novo objeto [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="4dad7-103">Create a new [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4dad7-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4dad7-104">Prerequisites</span></span>
<span data-ttu-id="4dad7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4dad7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4dad7-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dad7-107">Permission type</span></span>|<span data-ttu-id="4dad7-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4dad7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dad7-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dad7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4dad7-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dad7-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4dad7-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dad7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dad7-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dad7-112">Not supported.</span></span>|
|<span data-ttu-id="4dad7-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dad7-113">Application</span></span>|<span data-ttu-id="4dad7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dad7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dad7-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dad7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="4dad7-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dad7-116">Request headers</span></span>
|<span data-ttu-id="4dad7-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4dad7-117">Header</span></span>|<span data-ttu-id="4dad7-118">Valor</span><span class="sxs-lookup"><span data-stu-id="4dad7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dad7-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dad7-119">Authorization</span></span>|<span data-ttu-id="4dad7-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="4dad7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dad7-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4dad7-121">Accept</span></span>|<span data-ttu-id="4dad7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4dad7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dad7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dad7-123">Request body</span></span>
<span data-ttu-id="4dad7-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="4dad7-124">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="4dad7-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="4dad7-125">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="4dad7-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dad7-126">Property</span></span>|<span data-ttu-id="4dad7-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dad7-127">Type</span></span>|<span data-ttu-id="4dad7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dad7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dad7-129">id</span><span class="sxs-lookup"><span data-stu-id="4dad7-129">id</span></span>|<span data-ttu-id="4dad7-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dad7-130">String</span></span>|<span data-ttu-id="4dad7-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4dad7-131">Not yet documented</span></span>|
|<span data-ttu-id="4dad7-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="4dad7-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="4dad7-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dad7-133">DateTimeOffset</span></span>|<span data-ttu-id="4dad7-134">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="4dad7-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="4dad7-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="4dad7-135">partnerState</span></span>|[<span data-ttu-id="4dad7-136">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="4dad7-136">deviceManagementPartnerTenantState</span></span>](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|<span data-ttu-id="4dad7-p102">Estado de parceiro desse locatário. Os valores possíveis são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="4dad7-p102">Partner state of this tenant Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="4dad7-139">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="4dad7-139">partnerAppType</span></span>|[<span data-ttu-id="4dad7-140">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="4dad7-140">deviceManagementPartnerAppType</span></span>](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|<span data-ttu-id="4dad7-p103">Tipo de aplicativo do parceiro. Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="4dad7-p103">Partner App type Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="4dad7-143">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="4dad7-143">singleTenantAppId</span></span>|<span data-ttu-id="4dad7-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dad7-144">String</span></span>|<span data-ttu-id="4dad7-145">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="4dad7-145">Partner Single tenant App id</span></span>|
|<span data-ttu-id="4dad7-146">displayName</span><span class="sxs-lookup"><span data-stu-id="4dad7-146">displayName</span></span>|<span data-ttu-id="4dad7-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dad7-147">String</span></span>|<span data-ttu-id="4dad7-148">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="4dad7-148">Partner display name</span></span>|
|<span data-ttu-id="4dad7-149">isConfigured</span><span class="sxs-lookup"><span data-stu-id="4dad7-149">isConfigured</span></span>|<span data-ttu-id="4dad7-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dad7-150">Boolean</span></span>|<span data-ttu-id="4dad7-151">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="4dad7-151">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="4dad7-152">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="4dad7-152">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="4dad7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dad7-153">DateTimeOffset</span></span>|<span data-ttu-id="4dad7-154">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="4dad7-154">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="4dad7-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="4dad7-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="4dad7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dad7-156">DateTimeOffset</span></span>|<span data-ttu-id="4dad7-157">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="4dad7-157">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="4dad7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dad7-158">Response</span></span>
<span data-ttu-id="4dad7-159">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4dad7-159">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dad7-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dad7-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="4dad7-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dad7-161">Request</span></span>
<span data-ttu-id="4dad7-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dad7-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="4dad7-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dad7-163">Response</span></span>
<span data-ttu-id="4dad7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4dad7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```








