# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="243b3-101">Criar androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="243b3-101">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="243b3-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="243b3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="243b3-103">Cria um novo objeto [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="243b3-103">Create a new [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="243b3-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="243b3-104">Prerequisites</span></span>
<span data-ttu-id="243b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="243b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="243b3-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="243b3-107">Permission type</span></span>|<span data-ttu-id="243b3-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="243b3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="243b3-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="243b3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="243b3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="243b3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="243b3-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="243b3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="243b3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="243b3-112">Not supported.</span></span>|
|<span data-ttu-id="243b3-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="243b3-113">Application</span></span>|<span data-ttu-id="243b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="243b3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="243b3-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="243b3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="243b3-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="243b3-116">Request headers</span></span>
|<span data-ttu-id="243b3-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="243b3-117">Header</span></span>|<span data-ttu-id="243b3-118">Valor</span><span class="sxs-lookup"><span data-stu-id="243b3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="243b3-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="243b3-119">Authorization</span></span>|<span data-ttu-id="243b3-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="243b3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="243b3-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="243b3-121">Accept</span></span>|<span data-ttu-id="243b3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="243b3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="243b3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="243b3-123">Request body</span></span>
<span data-ttu-id="243b3-124">No corpo da solicitação, forneça uma representação JSON do objeto androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="243b3-124">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="243b3-125">A tabela a seguir mostra as propriedades que são necessárias ao criar androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="243b3-125">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="243b3-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="243b3-126">Property</span></span>|<span data-ttu-id="243b3-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="243b3-127">Type</span></span>|<span data-ttu-id="243b3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="243b3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="243b3-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="243b3-129">createdDateTime</span></span>|<span data-ttu-id="243b3-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="243b3-130">DateTimeOffset</span></span>|<span data-ttu-id="243b3-131">Data e hora de criação. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="243b3-132">lastSyncDateTime</span></span>|<span data-ttu-id="243b3-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="243b3-133">DateTimeOffset</span></span>|<span data-ttu-id="243b3-134">Data e hora em que o último aplicativo foi sincronizado com o serviço de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="243b3-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="243b3-135">Herdada da [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="243b3-136">applicationVersion</span></span>|<span data-ttu-id="243b3-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="243b3-137">String</span></span>|<span data-ttu-id="243b3-138">Versão do aplicativo. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="243b3-139">managementSdkVersion</span></span>|<span data-ttu-id="243b3-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="243b3-140">String</span></span>|<span data-ttu-id="243b3-141">Versão do SDK do gerenciamento de aplicativos. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="243b3-142">platformVersion</span></span>|<span data-ttu-id="243b3-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="243b3-143">String</span></span>|<span data-ttu-id="243b3-144">Versão do sistema operacional. Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="243b3-145">deviceType</span></span>|<span data-ttu-id="243b3-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="243b3-146">String</span></span>|<span data-ttu-id="243b3-147">Tipo de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="243b3-148">deviceTag</span></span>|<span data-ttu-id="243b3-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="243b3-149">String</span></span>|<span data-ttu-id="243b3-150">Uma tag gerada pelo SDK de gerenciamento, que ajuda a relacionar aplicativos hospedados no mesmo dispositivo.</span><span class="sxs-lookup"><span data-stu-id="243b3-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="243b3-151">Sem garantia de indicar aplicativos em todas as condições.</span><span class="sxs-lookup"><span data-stu-id="243b3-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="243b3-152">Herdada de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="243b3-153">deviceName</span></span>|<span data-ttu-id="243b3-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="243b3-154">String</span></span>|<span data-ttu-id="243b3-155">Nome de dispositivo do host. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="243b3-156">flaggedReasons</span></span>|<span data-ttu-id="243b3-157">coleção [managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-157">[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="243b3-158">Zero ou mais motivos para a sinalização de um registro de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="243b3-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="243b3-159">E.g.</span><span class="sxs-lookup"><span data-stu-id="243b3-159">E.g.</span></span> <span data-ttu-id="243b3-160">aplicativo em execução no dispositivo com raiz Inherited de [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="243b3-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span></span> <span data-ttu-id="243b3-161">Os valores possíveis são: `none` e `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="243b3-161">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="243b3-162">userId</span><span class="sxs-lookup"><span data-stu-id="243b3-162">userId</span></span>|<span data-ttu-id="243b3-163">String</span><span class="sxs-lookup"><span data-stu-id="243b3-163">String</span></span>|<span data-ttu-id="243b3-164">A ID de usuário à qual este registro de aplicativo pertence.</span><span class="sxs-lookup"><span data-stu-id="243b3-164">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="243b3-165">Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-165">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-166">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="243b3-166">appIdentifier</span></span>|[<span data-ttu-id="243b3-167">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="243b3-167">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="243b3-168">O Identificador de pacote do aplicativo. Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-168">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-169">id</span><span class="sxs-lookup"><span data-stu-id="243b3-169">id</span></span>|<span data-ttu-id="243b3-170">String</span><span class="sxs-lookup"><span data-stu-id="243b3-170">String</span></span>|<span data-ttu-id="243b3-171">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="243b3-171">Key of the entity.</span></span> <span data-ttu-id="243b3-172">Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-172">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="243b3-173">version</span><span class="sxs-lookup"><span data-stu-id="243b3-173">version</span></span>|<span data-ttu-id="243b3-174">String</span><span class="sxs-lookup"><span data-stu-id="243b3-174">String</span></span>|<span data-ttu-id="243b3-175">Versão da entidade.</span><span class="sxs-lookup"><span data-stu-id="243b3-175">Version of the entity.</span></span> <span data-ttu-id="243b3-176">Herdado de [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="243b3-176">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="243b3-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="243b3-177">Response</span></span>
<span data-ttu-id="243b3-178">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="243b3-178">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="243b3-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="243b3-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="243b3-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="243b3-180">Request</span></span>
<span data-ttu-id="243b3-181">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="243b3-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="243b3-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="243b3-182">Response</span></span>
<span data-ttu-id="243b3-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="243b3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```



