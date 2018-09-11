# <a name="update-windowsmobilemsi"></a><span data-ttu-id="823aa-101">Atualizar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="823aa-101">Update windowsMobileMSI</span></span>

> <span data-ttu-id="823aa-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="823aa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="823aa-103">Atualiza as propriedades de um objeto [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="823aa-103">Update the properties of a [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="823aa-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="823aa-104">Prerequisites</span></span>
<span data-ttu-id="823aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="823aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="823aa-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="823aa-107">Permission type</span></span>|<span data-ttu-id="823aa-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="823aa-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="823aa-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="823aa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="823aa-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="823aa-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="823aa-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="823aa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="823aa-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="823aa-112">Not supported.</span></span>|
|<span data-ttu-id="823aa-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="823aa-113">Application</span></span>|<span data-ttu-id="823aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="823aa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="823aa-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="823aa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="823aa-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="823aa-116">Request headers</span></span>
|<span data-ttu-id="823aa-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="823aa-117">Header</span></span>|<span data-ttu-id="823aa-118">Valor</span><span class="sxs-lookup"><span data-stu-id="823aa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="823aa-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="823aa-119">Authorization</span></span>|<span data-ttu-id="823aa-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="823aa-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="823aa-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="823aa-121">Accept</span></span>|<span data-ttu-id="823aa-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="823aa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="823aa-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="823aa-123">Request body</span></span>
<span data-ttu-id="823aa-124">No corpo da solicitação, forneça uma representação JSON para o objeto [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="823aa-124">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="823aa-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="823aa-125">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span></span>

|<span data-ttu-id="823aa-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="823aa-126">Property</span></span>|<span data-ttu-id="823aa-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="823aa-127">Type</span></span>|<span data-ttu-id="823aa-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="823aa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="823aa-129">id</span><span class="sxs-lookup"><span data-stu-id="823aa-129">id</span></span>|<span data-ttu-id="823aa-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-130">String</span></span>|<span data-ttu-id="823aa-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="823aa-131">Key of the entity.</span></span> <span data-ttu-id="823aa-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="823aa-133">displayName</span></span>|<span data-ttu-id="823aa-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-134">String</span></span>|<span data-ttu-id="823aa-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="823aa-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="823aa-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-137">description</span><span class="sxs-lookup"><span data-stu-id="823aa-137">description</span></span>|<span data-ttu-id="823aa-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-138">String</span></span>|<span data-ttu-id="823aa-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="823aa-139">The description of the app.</span></span> <span data-ttu-id="823aa-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-141">publisher</span><span class="sxs-lookup"><span data-stu-id="823aa-141">publisher</span></span>|<span data-ttu-id="823aa-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-142">String</span></span>|<span data-ttu-id="823aa-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="823aa-143">The publisher of the app.</span></span> <span data-ttu-id="823aa-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="823aa-145">largeIcon</span></span>|[<span data-ttu-id="823aa-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="823aa-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="823aa-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="823aa-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="823aa-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="823aa-149">createdDateTime</span></span>|<span data-ttu-id="823aa-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="823aa-150">DateTimeOffset</span></span>|<span data-ttu-id="823aa-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="823aa-151">The date and time the app was created.</span></span> <span data-ttu-id="823aa-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="823aa-153">lastModifiedDateTime</span></span>|<span data-ttu-id="823aa-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="823aa-154">DateTimeOffset</span></span>|<span data-ttu-id="823aa-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="823aa-155">The date and time the app was last modified.</span></span> <span data-ttu-id="823aa-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="823aa-157">isFeatured</span></span>|<span data-ttu-id="823aa-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="823aa-158">Boolean</span></span>|<span data-ttu-id="823aa-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="823aa-160">privacyInformationUrl</span></span>|<span data-ttu-id="823aa-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-161">String</span></span>|<span data-ttu-id="823aa-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="823aa-162">The privacy statement Url.</span></span> <span data-ttu-id="823aa-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="823aa-164">informationUrl</span></span>|<span data-ttu-id="823aa-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-165">String</span></span>|<span data-ttu-id="823aa-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="823aa-166">The more information Url.</span></span> <span data-ttu-id="823aa-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-168">owner</span><span class="sxs-lookup"><span data-stu-id="823aa-168">owner</span></span>|<span data-ttu-id="823aa-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-169">String</span></span>|<span data-ttu-id="823aa-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="823aa-170">The owner of the app.</span></span> <span data-ttu-id="823aa-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-172">developer</span><span class="sxs-lookup"><span data-stu-id="823aa-172">developer</span></span>|<span data-ttu-id="823aa-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-173">String</span></span>|<span data-ttu-id="823aa-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="823aa-174">The developer of the app.</span></span> <span data-ttu-id="823aa-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-176">Observações</span><span class="sxs-lookup"><span data-stu-id="823aa-176">notes</span></span>|<span data-ttu-id="823aa-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-177">String</span></span>|<span data-ttu-id="823aa-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="823aa-178">Notes for the app.</span></span> <span data-ttu-id="823aa-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="823aa-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="823aa-180">publishingState</span></span>|[<span data-ttu-id="823aa-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="823aa-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="823aa-p114">O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos que esteja publicado. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="823aa-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="823aa-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="823aa-186">committedContentVersion</span></span>|<span data-ttu-id="823aa-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-187">String</span></span>|<span data-ttu-id="823aa-188">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="823aa-188">The internal committed content version.</span></span> <span data-ttu-id="823aa-189">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="823aa-190">fileName</span><span class="sxs-lookup"><span data-stu-id="823aa-190">fileName</span></span>|<span data-ttu-id="823aa-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-191">String</span></span>|<span data-ttu-id="823aa-192">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="823aa-192">The name of the main Lob application file.</span></span> <span data-ttu-id="823aa-193">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="823aa-194">size</span><span class="sxs-lookup"><span data-stu-id="823aa-194">size</span></span>|<span data-ttu-id="823aa-195">Int64</span><span class="sxs-lookup"><span data-stu-id="823aa-195">Int64</span></span>|<span data-ttu-id="823aa-196">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="823aa-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="823aa-197">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="823aa-198">commandLine</span><span class="sxs-lookup"><span data-stu-id="823aa-198">commandLine</span></span>|<span data-ttu-id="823aa-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-199">String</span></span>|<span data-ttu-id="823aa-200">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="823aa-200">The command line.</span></span>|
|<span data-ttu-id="823aa-201">productCode</span><span class="sxs-lookup"><span data-stu-id="823aa-201">productCode</span></span>|<span data-ttu-id="823aa-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-202">String</span></span>|<span data-ttu-id="823aa-203">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="823aa-203">The product code.</span></span>|
|<span data-ttu-id="823aa-204">productVersion</span><span class="sxs-lookup"><span data-stu-id="823aa-204">productVersion</span></span>|<span data-ttu-id="823aa-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="823aa-205">String</span></span>|<span data-ttu-id="823aa-206">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="823aa-206">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="823aa-207">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="823aa-207">ignoreVersionDetection</span></span>|<span data-ttu-id="823aa-208">Booleano</span><span class="sxs-lookup"><span data-stu-id="823aa-208">Boolean</span></span>|<span data-ttu-id="823aa-209">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="823aa-209">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="823aa-210">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="823aa-210">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="823aa-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="823aa-211">Response</span></span>
<span data-ttu-id="823aa-212">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="823aa-212">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="823aa-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="823aa-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="823aa-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="823aa-214">Request</span></span>
<span data-ttu-id="823aa-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="823aa-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 864

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="823aa-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="823aa-216">Response</span></span>
<span data-ttu-id="823aa-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="823aa-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```








