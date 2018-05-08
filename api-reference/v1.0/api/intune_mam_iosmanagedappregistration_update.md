# <a name="update-iosmanagedappregistration"></a><span data-ttu-id="62822-101">Atualizar iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="62822-101">Update iosManagedAppRegistration</span></span>

> <span data-ttu-id="62822-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="62822-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62822-103">Atualizar as propriedades de um objeto [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="62822-103">Update the properties of a [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62822-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62822-104">Prerequisites</span></span>
<span data-ttu-id="62822-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="62822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="62822-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62822-107">Permission type</span></span>|<span data-ttu-id="62822-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62822-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62822-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62822-109">Delegated (work or school account)</span></span>|<span data-ttu-id="62822-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62822-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62822-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62822-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62822-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62822-112">Not supported.</span></span>|
|<span data-ttu-id="62822-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62822-113">Application</span></span>|<span data-ttu-id="62822-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62822-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62822-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62822-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="62822-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62822-116">Request headers</span></span>
|<span data-ttu-id="62822-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62822-117">Header</span></span>|<span data-ttu-id="62822-118">Valor</span><span class="sxs-lookup"><span data-stu-id="62822-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62822-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="62822-119">Authorization</span></span>|<span data-ttu-id="62822-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62822-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62822-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62822-121">Accept</span></span>|<span data-ttu-id="62822-122">application/json</span><span class="sxs-lookup"><span data-stu-id="62822-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62822-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62822-123">Request body</span></span>
<span data-ttu-id="62822-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="62822-124">In the request body, supply a JSON representation for the [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) object.</span></span>

<span data-ttu-id="62822-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="62822-125">The following table shows the properties that are required when you create the [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).</span></span>

|<span data-ttu-id="62822-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62822-126">Property</span></span>|<span data-ttu-id="62822-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="62822-127">Type</span></span>|<span data-ttu-id="62822-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="62822-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62822-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62822-129">createdDateTime</span></span>|<span data-ttu-id="62822-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62822-130">DateTimeOffset</span></span>|<span data-ttu-id="62822-131">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="62822-132">lastSyncDateTime</span></span>|<span data-ttu-id="62822-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62822-133">DateTimeOffset</span></span>|<span data-ttu-id="62822-134">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="62822-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="62822-135">Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="62822-136">applicationVersion</span></span>|<span data-ttu-id="62822-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62822-137">String</span></span>|<span data-ttu-id="62822-138">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="62822-139">managementSdkVersion</span></span>|<span data-ttu-id="62822-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62822-140">String</span></span>|<span data-ttu-id="62822-141">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="62822-142">platformVersion</span></span>|<span data-ttu-id="62822-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62822-143">String</span></span>|<span data-ttu-id="62822-144">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="62822-145">deviceType</span></span>|<span data-ttu-id="62822-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62822-146">String</span></span>|<span data-ttu-id="62822-147">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="62822-148">deviceTag</span></span>|<span data-ttu-id="62822-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62822-149">String</span></span>|<span data-ttu-id="62822-150">Uma tag gerada pelo SDK de gerenciamento que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62822-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="62822-151">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="62822-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="62822-152">Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="62822-153">deviceName</span></span>|<span data-ttu-id="62822-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62822-154">String</span></span>|<span data-ttu-id="62822-155">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="62822-156">flaggedReasons</span></span>|<span data-ttu-id="62822-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="62822-157">String collection</span></span>|<span data-ttu-id="62822-158">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62822-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="62822-159">E.g.</span><span class="sxs-lookup"><span data-stu-id="62822-159">E.g.</span></span> <span data-ttu-id="62822-160">aplicativo em execução em um dispositivo root Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Os valores possíveis são: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="62822-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="62822-161">userId</span><span class="sxs-lookup"><span data-stu-id="62822-161">userId</span></span>|<span data-ttu-id="62822-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62822-162">String</span></span>|<span data-ttu-id="62822-163">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="62822-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="62822-164">Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="62822-165">appIdentifier</span></span>|[<span data-ttu-id="62822-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="62822-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="62822-167">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-168">id</span><span class="sxs-lookup"><span data-stu-id="62822-168">id</span></span>|<span data-ttu-id="62822-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62822-169">String</span></span>|<span data-ttu-id="62822-170">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="62822-170">Key of the entity.</span></span> <span data-ttu-id="62822-171">Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="62822-172">version</span><span class="sxs-lookup"><span data-stu-id="62822-172">version</span></span>|<span data-ttu-id="62822-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62822-173">String</span></span>|<span data-ttu-id="62822-174">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="62822-174">Version of the entity.</span></span> <span data-ttu-id="62822-175">Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="62822-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="62822-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="62822-176">Response</span></span>
<span data-ttu-id="62822-177">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62822-177">If successful, this method returns a `200 OK` response code and an updated [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62822-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62822-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="62822-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62822-179">Request</span></span>
<span data-ttu-id="62822-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62822-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
Content-type: application/json
Content-length: 571

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "Bundle Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="62822-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="62822-181">Response</span></span>
<span data-ttu-id="62822-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62822-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 743

{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "Bundle Id value"
  },
  "id": "47632c19-2c19-4763-192c-6347192c6347",
  "version": "Version value"
}
```



