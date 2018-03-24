# <a name="create-devicemanagementpartner"></a><span data-ttu-id="8bad1-101">Criar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8bad1-101">Create deviceManagementPartner</span></span>

> <span data-ttu-id="8bad1-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8bad1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bad1-103">Criar um novo objeto [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="8bad1-103">Create a new [plannerBucket](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8bad1-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8bad1-104">Prerequisites</span></span>
<span data-ttu-id="8bad1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8bad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8bad1-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bad1-107">Permission type</span></span>|<span data-ttu-id="8bad1-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8bad1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bad1-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bad1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8bad1-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bad1-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8bad1-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bad1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bad1-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bad1-112">Not supported.</span></span>|
|<span data-ttu-id="8bad1-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bad1-113">Application</span></span>|<span data-ttu-id="8bad1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bad1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bad1-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bad1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="8bad1-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bad1-116">Request headers</span></span>
|<span data-ttu-id="8bad1-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8bad1-117">Header</span></span>|<span data-ttu-id="8bad1-118">Valor</span><span class="sxs-lookup"><span data-stu-id="8bad1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bad1-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bad1-119">Authorization</span></span>|<span data-ttu-id="8bad1-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bad1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8bad1-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8bad1-121">Accept</span></span>|<span data-ttu-id="8bad1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8bad1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bad1-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bad1-123">Request body</span></span>
<span data-ttu-id="8bad1-124">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="8bad1-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="8bad1-125">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="8bad1-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="8bad1-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8bad1-126">Property</span></span>|<span data-ttu-id="8bad1-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bad1-127">Type</span></span>|<span data-ttu-id="8bad1-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bad1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bad1-129">id</span><span class="sxs-lookup"><span data-stu-id="8bad1-129">id</span></span>|<span data-ttu-id="8bad1-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bad1-130">String</span></span>|<span data-ttu-id="8bad1-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8bad1-131">Not yet documented</span></span>|
|<span data-ttu-id="8bad1-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="8bad1-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="8bad1-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bad1-133">DateTimeOffset</span></span>|<span data-ttu-id="8bad1-134">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="8bad1-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="8bad1-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="8bad1-135">partnerState</span></span>|<span data-ttu-id="8bad1-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bad1-136">String</span></span>|<span data-ttu-id="8bad1-137">Estado de parceiro desse locatário Os valores possíveis são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="8bad1-137">Partner state of this tenant Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="8bad1-138">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="8bad1-138">partnerAppType</span></span>|<span data-ttu-id="8bad1-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bad1-139">String</span></span>|<span data-ttu-id="8bad1-140">Tipo de aplicativos do parceiro Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="8bad1-140">Partner App type Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="8bad1-141">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="8bad1-141">singleTenantAppId</span></span>|<span data-ttu-id="8bad1-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bad1-142">String</span></span>|<span data-ttu-id="8bad1-143">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="8bad1-143">Partner Single tenant App id</span></span>|
|<span data-ttu-id="8bad1-144">displayName</span><span class="sxs-lookup"><span data-stu-id="8bad1-144">displayName</span></span>|<span data-ttu-id="8bad1-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bad1-145">String</span></span>|<span data-ttu-id="8bad1-146">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="8bad1-146">Partner display name</span></span>|
|<span data-ttu-id="8bad1-147">isConfigured</span><span class="sxs-lookup"><span data-stu-id="8bad1-147">isConfigured</span></span>|<span data-ttu-id="8bad1-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="8bad1-148">Boolean</span></span>|<span data-ttu-id="8bad1-149">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="8bad1-149">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="8bad1-150">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bad1-150">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="8bad1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bad1-151">DateTimeOffset</span></span>|<span data-ttu-id="8bad1-152">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="8bad1-152">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="8bad1-153">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="8bad1-153">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="8bad1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bad1-154">DateTimeOffset</span></span>|<span data-ttu-id="8bad1-155">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="8bad1-155">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="8bad1-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bad1-156">Response</span></span>
<span data-ttu-id="8bad1-157">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bad1-157">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bad1-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bad1-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="8bad1-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bad1-159">Request</span></span>
<span data-ttu-id="8bad1-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bad1-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8bad1-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bad1-161">Response</span></span>
<span data-ttu-id="8bad1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bad1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



