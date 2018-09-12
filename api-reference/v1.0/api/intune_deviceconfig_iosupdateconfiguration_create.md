# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="76a7b-101">Criar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="76a7b-101">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="76a7b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="76a7b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76a7b-103">Cria um novo objeto [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76a7b-103">Create a new [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="76a7b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76a7b-104">Prerequisites</span></span>
<span data-ttu-id="76a7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="76a7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76a7b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76a7b-107">Permission type</span></span>|<span data-ttu-id="76a7b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76a7b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76a7b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76a7b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="76a7b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76a7b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76a7b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76a7b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76a7b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76a7b-112">Not supported.</span></span>|
|<span data-ttu-id="76a7b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76a7b-113">Application</span></span>|<span data-ttu-id="76a7b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76a7b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76a7b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76a7b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="76a7b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76a7b-116">Request headers</span></span>
|<span data-ttu-id="76a7b-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76a7b-117">Header</span></span>|<span data-ttu-id="76a7b-118">Valor</span><span class="sxs-lookup"><span data-stu-id="76a7b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76a7b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="76a7b-119">Authorization</span></span>|<span data-ttu-id="76a7b-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="76a7b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76a7b-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76a7b-121">Accept</span></span>|<span data-ttu-id="76a7b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="76a7b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76a7b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76a7b-123">Request body</span></span>
<span data-ttu-id="76a7b-124">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="76a7b-124">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="76a7b-125">A tabela a seguir mostra as propriedades obrigatórias ao criar iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="76a7b-125">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="76a7b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76a7b-126">Property</span></span>|<span data-ttu-id="76a7b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="76a7b-127">Type</span></span>|<span data-ttu-id="76a7b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="76a7b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76a7b-129">id</span><span class="sxs-lookup"><span data-stu-id="76a7b-129">id</span></span>|<span data-ttu-id="76a7b-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76a7b-130">String</span></span>|<span data-ttu-id="76a7b-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="76a7b-131">Key of the entity.</span></span> <span data-ttu-id="76a7b-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76a7b-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76a7b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76a7b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="76a7b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76a7b-134">DateTimeOffset</span></span>|<span data-ttu-id="76a7b-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="76a7b-135">DateTime the object was last modified.</span></span> <span data-ttu-id="76a7b-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76a7b-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76a7b-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76a7b-137">createdDateTime</span></span>|<span data-ttu-id="76a7b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76a7b-138">DateTimeOffset</span></span>|<span data-ttu-id="76a7b-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="76a7b-139">DateTime the object was created.</span></span> <span data-ttu-id="76a7b-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76a7b-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76a7b-141">description</span><span class="sxs-lookup"><span data-stu-id="76a7b-141">description</span></span>|<span data-ttu-id="76a7b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76a7b-142">String</span></span>|<span data-ttu-id="76a7b-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76a7b-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="76a7b-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76a7b-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76a7b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="76a7b-145">displayName</span></span>|<span data-ttu-id="76a7b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76a7b-146">String</span></span>|<span data-ttu-id="76a7b-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76a7b-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="76a7b-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76a7b-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76a7b-149">version</span><span class="sxs-lookup"><span data-stu-id="76a7b-149">version</span></span>|<span data-ttu-id="76a7b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="76a7b-150">Int32</span></span>|<span data-ttu-id="76a7b-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76a7b-151">Version of the device configuration.</span></span> <span data-ttu-id="76a7b-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76a7b-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76a7b-153">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="76a7b-153">activeHoursStart</span></span>|<span data-ttu-id="76a7b-154">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="76a7b-154">TimeOfDay</span></span>|<span data-ttu-id="76a7b-155">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="76a7b-155">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="76a7b-156">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="76a7b-156">activeHoursEnd</span></span>|<span data-ttu-id="76a7b-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="76a7b-157">TimeOfDay</span></span>|<span data-ttu-id="76a7b-158">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="76a7b-158">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="76a7b-159">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="76a7b-159">scheduledInstallDays</span></span>|<span data-ttu-id="76a7b-160">coleção [dayOfWeek enum](../resources/intune_deviceconfig_dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="76a7b-160">dayOfWeek collection</span></span>|<span data-ttu-id="76a7b-p108">Dias na semana para os quais as horas ativas são configuradas. Essa coleção pode conter um máximo de 7 elementos. Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="76a7b-p108">Days in week for which active hours are configured. This collection can contain a maximum of 7 elements. The possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="76a7b-164">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="76a7b-164">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="76a7b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="76a7b-165">Int32</span></span>|<span data-ttu-id="76a7b-166">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="76a7b-166">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="76a7b-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="76a7b-167">Response</span></span>
<span data-ttu-id="76a7b-168">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76a7b-168">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76a7b-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76a7b-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="76a7b-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76a7b-170">Request</span></span>
<span data-ttu-id="76a7b-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76a7b-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76a7b-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="76a7b-172">Response</span></span>
<span data-ttu-id="76a7b-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76a7b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








