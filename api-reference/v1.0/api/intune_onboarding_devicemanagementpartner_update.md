# <a name="update-devicemanagementpartner"></a><span data-ttu-id="b5d72-101">Atualizar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="b5d72-101">Update deviceManagementPartner</span></span>

> <span data-ttu-id="b5d72-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b5d72-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5d72-103">Atualize as propriedades de um objeto [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="b5d72-103">Update the properties of a [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5d72-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5d72-104">Prerequisites</span></span>
<span data-ttu-id="b5d72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5d72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b5d72-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5d72-107">Permission type</span></span>|<span data-ttu-id="b5d72-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b5d72-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5d72-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5d72-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b5d72-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d72-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b5d72-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5d72-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5d72-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5d72-112">Not supported.</span></span>|
|<span data-ttu-id="b5d72-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5d72-113">Application</span></span>|<span data-ttu-id="b5d72-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5d72-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5d72-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5d72-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="b5d72-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5d72-116">Request headers</span></span>
|<span data-ttu-id="b5d72-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5d72-117">Header</span></span>|<span data-ttu-id="b5d72-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b5d72-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5d72-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5d72-119">Authorization</span></span>|<span data-ttu-id="b5d72-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5d72-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5d72-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b5d72-121">Accept</span></span>|<span data-ttu-id="b5d72-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b5d72-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5d72-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5d72-123">Request body</span></span>
<span data-ttu-id="b5d72-124">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="b5d72-124">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="b5d72-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="b5d72-125">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span></span>

|<span data-ttu-id="b5d72-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5d72-126">Property</span></span>|<span data-ttu-id="b5d72-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5d72-127">Type</span></span>|<span data-ttu-id="b5d72-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5d72-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5d72-129">id</span><span class="sxs-lookup"><span data-stu-id="b5d72-129">id</span></span>|<span data-ttu-id="b5d72-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5d72-130">String</span></span>|<span data-ttu-id="b5d72-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b5d72-131">Not yet documented</span></span>|
|<span data-ttu-id="b5d72-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="b5d72-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="b5d72-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5d72-133">DateTimeOffset</span></span>|<span data-ttu-id="b5d72-134">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="b5d72-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="b5d72-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="b5d72-135">partnerState</span></span>|[<span data-ttu-id="b5d72-136">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="b5d72-136">deviceManagementPartnerTenantState</span></span>](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|<span data-ttu-id="b5d72-137">Estado de parceiro deste locatário.</span><span class="sxs-lookup"><span data-stu-id="b5d72-137">Partner state of this tenant.</span></span> <span data-ttu-id="b5d72-138">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="b5d72-138">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="b5d72-139">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="b5d72-139">partnerAppType</span></span>|[<span data-ttu-id="b5d72-140">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="b5d72-140">deviceManagementPartnerAppType</span></span>](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|<span data-ttu-id="b5d72-141">Tipo de aplicativo de parceiro.</span><span class="sxs-lookup"><span data-stu-id="b5d72-141">Partner App type.</span></span> <span data-ttu-id="b5d72-142">Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="b5d72-142">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="b5d72-143">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="b5d72-143">singleTenantAppId</span></span>|<span data-ttu-id="b5d72-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5d72-144">String</span></span>|<span data-ttu-id="b5d72-145">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="b5d72-145">Partner Single tenant App id</span></span>|
|<span data-ttu-id="b5d72-146">displayName</span><span class="sxs-lookup"><span data-stu-id="b5d72-146">displayName</span></span>|<span data-ttu-id="b5d72-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5d72-147">String</span></span>|<span data-ttu-id="b5d72-148">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="b5d72-148">Partner display name</span></span>|
|<span data-ttu-id="b5d72-149">isConfigured</span><span class="sxs-lookup"><span data-stu-id="b5d72-149">isConfigured</span></span>|<span data-ttu-id="b5d72-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5d72-150">Boolean</span></span>|<span data-ttu-id="b5d72-151">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="b5d72-151">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="b5d72-152">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5d72-152">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="b5d72-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5d72-153">DateTimeOffset</span></span>|<span data-ttu-id="b5d72-154">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="b5d72-154">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="b5d72-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="b5d72-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="b5d72-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5d72-156">DateTimeOffset</span></span>|<span data-ttu-id="b5d72-157">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="b5d72-157">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="b5d72-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5d72-158">Response</span></span>
<span data-ttu-id="b5d72-159">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5d72-159">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5d72-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5d72-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5d72-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5d72-161">Request</span></span>
<span data-ttu-id="b5d72-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5d72-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
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

### <a name="response"></a><span data-ttu-id="b5d72-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5d72-163">Response</span></span>
<span data-ttu-id="b5d72-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5d72-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



