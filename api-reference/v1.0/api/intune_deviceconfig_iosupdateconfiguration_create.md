# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="a0d0e-101">Criar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0d0e-101">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="a0d0e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0d0e-103">Cria um novo objeto [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0d0e-103">Create a new [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0d0e-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0d0e-104">Prerequisites</span></span>
<span data-ttu-id="a0d0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a0d0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a0d0e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0d0e-107">Permission type</span></span>|<span data-ttu-id="a0d0e-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0d0e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a0d0e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d0e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0d0e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0d0e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-112">Not supported.</span></span>|
|<span data-ttu-id="a0d0e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0d0e-113">Application</span></span>|<span data-ttu-id="a0d0e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0d0e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0d0e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0d0e-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d0e-116">Request headers</span></span>
|<span data-ttu-id="a0d0e-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0d0e-117">Header</span></span>|<span data-ttu-id="a0d0e-118">Valor</span><span class="sxs-lookup"><span data-stu-id="a0d0e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0d0e-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0d0e-119">Authorization</span></span>|<span data-ttu-id="a0d0e-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="a0d0e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0d0e-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0d0e-121">Accept</span></span>|<span data-ttu-id="a0d0e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a0d0e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0d0e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d0e-123">Request body</span></span>
<span data-ttu-id="a0d0e-124">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-124">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="a0d0e-125">A tabela a seguir mostra as propriedades obrigatórias ao criar iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-125">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="a0d0e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0d0e-126">Property</span></span>|<span data-ttu-id="a0d0e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0d0e-127">Type</span></span>|<span data-ttu-id="a0d0e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0d0e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0d0e-129">id</span><span class="sxs-lookup"><span data-stu-id="a0d0e-129">id</span></span>|<span data-ttu-id="a0d0e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0d0e-130">String</span></span>|<span data-ttu-id="a0d0e-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-131">Key of the entity.</span></span> <span data-ttu-id="a0d0e-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d0e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0d0e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a0d0e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0d0e-134">DateTimeOffset</span></span>|<span data-ttu-id="a0d0e-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-135">DateTime the object was last modified.</span></span> <span data-ttu-id="a0d0e-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d0e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0d0e-137">createdDateTime</span></span>|<span data-ttu-id="a0d0e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0d0e-138">DateTimeOffset</span></span>|<span data-ttu-id="a0d0e-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-139">DateTime the object was created.</span></span> <span data-ttu-id="a0d0e-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d0e-141">description</span><span class="sxs-lookup"><span data-stu-id="a0d0e-141">description</span></span>|<span data-ttu-id="a0d0e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0d0e-142">String</span></span>|<span data-ttu-id="a0d0e-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0d0e-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d0e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a0d0e-145">displayName</span></span>|<span data-ttu-id="a0d0e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0d0e-146">String</span></span>|<span data-ttu-id="a0d0e-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0d0e-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d0e-149">version</span><span class="sxs-lookup"><span data-stu-id="a0d0e-149">version</span></span>|<span data-ttu-id="a0d0e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a0d0e-150">Int32</span></span>|<span data-ttu-id="a0d0e-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-151">Version of the device configuration.</span></span> <span data-ttu-id="a0d0e-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0d0e-153">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="a0d0e-153">activeHoursStart</span></span>|<span data-ttu-id="a0d0e-154">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a0d0e-154">TimeOfDay</span></span>|<span data-ttu-id="a0d0e-155">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-155">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="a0d0e-156">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="a0d0e-156">activeHoursEnd</span></span>|<span data-ttu-id="a0d0e-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a0d0e-157">TimeOfDay</span></span>|<span data-ttu-id="a0d0e-158">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-158">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="a0d0e-159">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="a0d0e-159">scheduledInstallDays</span></span>|<span data-ttu-id="a0d0e-160">coleção [dayOfWeek enum](../resources/intune_deviceconfig_dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="a0d0e-160">[dayOfWeek enum](../resources/intune_deviceconfig_dayofweek.md) collection</span></span>|<span data-ttu-id="a0d0e-161">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-161">Days in week for which active hours are configured.</span></span> <span data-ttu-id="a0d0e-162">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-162">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="a0d0e-163">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-163">The possible values are `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, , , , , or .</span></span>|
|<span data-ttu-id="a0d0e-164">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="a0d0e-164">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="a0d0e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a0d0e-165">Int32</span></span>|<span data-ttu-id="a0d0e-166">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="a0d0e-166">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="a0d0e-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0d0e-167">Response</span></span>
<span data-ttu-id="a0d0e-168">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-168">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0d0e-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0d0e-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0d0e-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d0e-170">Request</span></span>
<span data-ttu-id="a0d0e-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

### <a name="response"></a><span data-ttu-id="a0d0e-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0d0e-172">Response</span></span>
<span data-ttu-id="a0d0e-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0d0e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```



