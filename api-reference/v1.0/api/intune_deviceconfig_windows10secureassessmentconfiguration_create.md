# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="2f92c-101">Criar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f92c-101">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="2f92c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2f92c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f92c-103">Cria um novo objeto [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f92c-103">Create a new [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f92c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f92c-104">Prerequisites</span></span>
<span data-ttu-id="2f92c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f92c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f92c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f92c-107">Permission type</span></span>|<span data-ttu-id="2f92c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f92c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f92c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f92c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2f92c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f92c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f92c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f92c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f92c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f92c-112">Not supported.</span></span>|
|<span data-ttu-id="2f92c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f92c-113">Application</span></span>|<span data-ttu-id="2f92c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f92c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f92c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f92c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f92c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f92c-116">Request headers</span></span>
|<span data-ttu-id="2f92c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f92c-117">Header</span></span>|<span data-ttu-id="2f92c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="2f92c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f92c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f92c-119">Authorization</span></span>|<span data-ttu-id="2f92c-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="2f92c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f92c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f92c-121">Accept</span></span>|<span data-ttu-id="2f92c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2f92c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f92c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f92c-123">Request body</span></span>
<span data-ttu-id="2f92c-124">No corpo da solicitação, forneça uma representação JSON do objeto windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f92c-124">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="2f92c-125">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f92c-125">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="2f92c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f92c-126">Property</span></span>|<span data-ttu-id="2f92c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f92c-127">Type</span></span>|<span data-ttu-id="2f92c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f92c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f92c-129">id</span><span class="sxs-lookup"><span data-stu-id="2f92c-129">id</span></span>|<span data-ttu-id="2f92c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f92c-130">String</span></span>|<span data-ttu-id="2f92c-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f92c-131">Key of the entity.</span></span> <span data-ttu-id="2f92c-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92c-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f92c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2f92c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f92c-134">DateTimeOffset</span></span>|<span data-ttu-id="2f92c-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2f92c-135">DateTime the object was last modified.</span></span> <span data-ttu-id="2f92c-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92c-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f92c-137">createdDateTime</span></span>|<span data-ttu-id="2f92c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f92c-138">DateTimeOffset</span></span>|<span data-ttu-id="2f92c-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2f92c-139">DateTime the object was created.</span></span> <span data-ttu-id="2f92c-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92c-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92c-141">descrição</span><span class="sxs-lookup"><span data-stu-id="2f92c-141">description</span></span>|<span data-ttu-id="2f92c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f92c-142">String</span></span>|<span data-ttu-id="2f92c-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f92c-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f92c-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92c-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="2f92c-145">displayName</span></span>|<span data-ttu-id="2f92c-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f92c-146">String</span></span>|<span data-ttu-id="2f92c-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f92c-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f92c-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92c-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92c-149">version</span><span class="sxs-lookup"><span data-stu-id="2f92c-149">version</span></span>|<span data-ttu-id="2f92c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2f92c-150">Int32</span></span>|<span data-ttu-id="2f92c-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f92c-151">Version of the device configuration.</span></span> <span data-ttu-id="2f92c-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92c-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92c-153">launchUri</span><span class="sxs-lookup"><span data-stu-id="2f92c-153">launchUri</span></span>|<span data-ttu-id="2f92c-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f92c-154">String</span></span>|<span data-ttu-id="2f92c-155">Link da URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="2f92c-155">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="2f92c-156">Ele precisa ser uma URL válida (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="2f92c-156">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="2f92c-157">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="2f92c-157">configurationAccount</span></span>|<span data-ttu-id="2f92c-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f92c-158">String</span></span>|<span data-ttu-id="2f92c-159">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="2f92c-159">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="2f92c-160">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="2f92c-160">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="2f92c-161">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="2f92c-161">allowPrinting</span></span>|<span data-ttu-id="2f92c-162">Booleano</span><span class="sxs-lookup"><span data-stu-id="2f92c-162">Boolean</span></span>|<span data-ttu-id="2f92c-163">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="2f92c-163">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="2f92c-164">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="2f92c-164">allowScreenCapture</span></span>|<span data-ttu-id="2f92c-165">Booleano</span><span class="sxs-lookup"><span data-stu-id="2f92c-165">Boolean</span></span>|<span data-ttu-id="2f92c-166">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="2f92c-166">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="2f92c-167">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="2f92c-167">allowTextSuggestion</span></span>|<span data-ttu-id="2f92c-168">Booleano</span><span class="sxs-lookup"><span data-stu-id="2f92c-168">Boolean</span></span>|<span data-ttu-id="2f92c-169">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="2f92c-169">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="2f92c-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f92c-170">Response</span></span>
<span data-ttu-id="2f92c-171">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f92c-171">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f92c-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f92c-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f92c-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f92c-173">Request</span></span>
<span data-ttu-id="2f92c-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f92c-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 423

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="2f92c-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f92c-175">Response</span></span>
<span data-ttu-id="2f92c-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f92c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```








