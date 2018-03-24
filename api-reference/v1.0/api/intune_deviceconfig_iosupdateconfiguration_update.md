# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="03ee5-101">Atualizar iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="03ee5-101">Update iosUpdateConfiguration</span></span>

> <span data-ttu-id="03ee5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="03ee5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03ee5-103">Atualizar as propriedades de um objeto [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03ee5-103">Update the properties of a [calendar](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03ee5-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03ee5-104">Prerequisites</span></span>
<span data-ttu-id="03ee5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="03ee5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="03ee5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03ee5-107">Permission type</span></span>|<span data-ttu-id="03ee5-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03ee5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03ee5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03ee5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="03ee5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03ee5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03ee5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03ee5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03ee5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03ee5-112">Not supported.</span></span>|
|<span data-ttu-id="03ee5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03ee5-113">Application</span></span>|<span data-ttu-id="03ee5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03ee5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03ee5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03ee5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="03ee5-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03ee5-116">Request headers</span></span>
|<span data-ttu-id="03ee5-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03ee5-117">Header</span></span>|<span data-ttu-id="03ee5-118">Valor</span><span class="sxs-lookup"><span data-stu-id="03ee5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03ee5-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="03ee5-119">Authorization</span></span>|<span data-ttu-id="03ee5-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03ee5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="03ee5-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03ee5-121">Accept</span></span>|<span data-ttu-id="03ee5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="03ee5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03ee5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03ee5-123">Request body</span></span>
<span data-ttu-id="03ee5-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03ee5-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="03ee5-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03ee5-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="03ee5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03ee5-126">Property</span></span>|<span data-ttu-id="03ee5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="03ee5-127">Type</span></span>|<span data-ttu-id="03ee5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="03ee5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03ee5-129">id</span><span class="sxs-lookup"><span data-stu-id="03ee5-129">id</span></span>|<span data-ttu-id="03ee5-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03ee5-130">String</span></span>|<span data-ttu-id="03ee5-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="03ee5-131">Key of the setting.</span></span> <span data-ttu-id="03ee5-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03ee5-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03ee5-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03ee5-133">lastModifiedDateTime</span></span>|<span data-ttu-id="03ee5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03ee5-134">DateTimeOffset</span></span>|<span data-ttu-id="03ee5-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="03ee5-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="03ee5-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03ee5-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03ee5-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03ee5-137">createdDateTime</span></span>|<span data-ttu-id="03ee5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03ee5-138">DateTimeOffset</span></span>|<span data-ttu-id="03ee5-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="03ee5-139">DateTime the object was created.</span></span> <span data-ttu-id="03ee5-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03ee5-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03ee5-141">descrição</span><span class="sxs-lookup"><span data-stu-id="03ee5-141">description</span></span>|<span data-ttu-id="03ee5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03ee5-142">String</span></span>|<span data-ttu-id="03ee5-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03ee5-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03ee5-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03ee5-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03ee5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="03ee5-145">displayName</span></span>|<span data-ttu-id="03ee5-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03ee5-146">String</span></span>|<span data-ttu-id="03ee5-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03ee5-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03ee5-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03ee5-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03ee5-149">version</span><span class="sxs-lookup"><span data-stu-id="03ee5-149">version</span></span>|<span data-ttu-id="03ee5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="03ee5-150">Int32</span></span>|<span data-ttu-id="03ee5-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03ee5-151">Version of the device configuration.</span></span> <span data-ttu-id="03ee5-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03ee5-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03ee5-153">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="03ee5-153">activeHoursStart</span></span>|<span data-ttu-id="03ee5-154">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="03ee5-154">TimeOfDay</span></span>|<span data-ttu-id="03ee5-155">Início do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="03ee5-155">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="03ee5-156">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="03ee5-156">activeHoursEnd</span></span>|<span data-ttu-id="03ee5-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="03ee5-157">TimeOfDay</span></span>|<span data-ttu-id="03ee5-158">Término do Horário Ativo (o horário ativo significa a janela de tempo quando a instalação das atualizações não deve acontecer)</span><span class="sxs-lookup"><span data-stu-id="03ee5-158">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="03ee5-159">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="03ee5-159">scheduledInstallDays</span></span>|<span data-ttu-id="03ee5-160">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="03ee5-160">String collection</span></span>|<span data-ttu-id="03ee5-161">Dias na semana para os quais o horário ativo está configurado.</span><span class="sxs-lookup"><span data-stu-id="03ee5-161">Days in week for which active hours are configured.</span></span> <span data-ttu-id="03ee5-162">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="03ee5-162">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="03ee5-163">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="03ee5-163">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="03ee5-164">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="03ee5-164">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="03ee5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="03ee5-165">Int32</span></span>|<span data-ttu-id="03ee5-166">Deslocamento do horário UTC indicado em minutos</span><span class="sxs-lookup"><span data-stu-id="03ee5-166">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="03ee5-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="03ee5-167">Response</span></span>
<span data-ttu-id="03ee5-168">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03ee5-168">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03ee5-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03ee5-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="03ee5-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03ee5-170">Request</span></span>
<span data-ttu-id="03ee5-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03ee5-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 328

{
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

### <a name="response"></a><span data-ttu-id="03ee5-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="03ee5-172">Response</span></span>
<span data-ttu-id="03ee5-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03ee5-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



