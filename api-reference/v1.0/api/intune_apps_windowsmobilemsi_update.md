# <a name="update-windowsmobilemsi"></a><span data-ttu-id="69abd-101">Atualizar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="69abd-101">Update windowsMobileMSI</span></span>

> <span data-ttu-id="69abd-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="69abd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69abd-103">Atualiza as propriedades de um objeto [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="69abd-103">Update the properties of a [calendar](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69abd-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69abd-104">Prerequisites</span></span>
<span data-ttu-id="69abd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="69abd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="69abd-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69abd-107">Permission type</span></span>|<span data-ttu-id="69abd-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69abd-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69abd-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69abd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="69abd-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69abd-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="69abd-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69abd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69abd-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69abd-112">Not supported.</span></span>|
|<span data-ttu-id="69abd-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69abd-113">Application</span></span>|<span data-ttu-id="69abd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69abd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69abd-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69abd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="69abd-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69abd-116">Request headers</span></span>
|<span data-ttu-id="69abd-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69abd-117">Header</span></span>|<span data-ttu-id="69abd-118">Valor</span><span class="sxs-lookup"><span data-stu-id="69abd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69abd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="69abd-119">Authorization</span></span>|<span data-ttu-id="69abd-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69abd-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="69abd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="69abd-121">Accept</span></span>|<span data-ttu-id="69abd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="69abd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69abd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69abd-123">Request body</span></span>
<span data-ttu-id="69abd-124">No corpo da solicitação, forneça uma representação JSON para o objeto [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="69abd-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="69abd-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="69abd-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="69abd-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69abd-126">Property</span></span>|<span data-ttu-id="69abd-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="69abd-127">Type</span></span>|<span data-ttu-id="69abd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="69abd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69abd-129">id</span><span class="sxs-lookup"><span data-stu-id="69abd-129">id</span></span>|<span data-ttu-id="69abd-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-130">String</span></span>|<span data-ttu-id="69abd-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="69abd-131">Key of the setting.</span></span> <span data-ttu-id="69abd-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="69abd-133">displayName</span></span>|<span data-ttu-id="69abd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-134">String</span></span>|<span data-ttu-id="69abd-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="69abd-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="69abd-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-137">description</span><span class="sxs-lookup"><span data-stu-id="69abd-137">description</span></span>|<span data-ttu-id="69abd-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-138">String</span></span>|<span data-ttu-id="69abd-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69abd-139">The description of the app.</span></span> <span data-ttu-id="69abd-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-141">publisher</span><span class="sxs-lookup"><span data-stu-id="69abd-141">Publisher</span></span>|<span data-ttu-id="69abd-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-142">String</span></span>|<span data-ttu-id="69abd-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69abd-143">The publisher of the app.</span></span> <span data-ttu-id="69abd-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="69abd-145">largeIcon</span></span>|[<span data-ttu-id="69abd-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="69abd-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="69abd-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="69abd-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="69abd-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69abd-149">createdDateTime</span></span>|<span data-ttu-id="69abd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69abd-150">DateTimeOffset</span></span>|<span data-ttu-id="69abd-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69abd-151">The date and time the group was created.</span></span> <span data-ttu-id="69abd-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69abd-153">lastModifiedDateTime</span></span>|<span data-ttu-id="69abd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69abd-154">DateTimeOffset</span></span>|<span data-ttu-id="69abd-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="69abd-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="69abd-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="69abd-157">isFeatured</span></span>|<span data-ttu-id="69abd-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="69abd-158">Boolean</span></span>|<span data-ttu-id="69abd-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="69abd-160">privacyInformationUrl</span></span>|<span data-ttu-id="69abd-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-161">String</span></span>|<span data-ttu-id="69abd-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="69abd-162">The privacy statement Url.</span></span> <span data-ttu-id="69abd-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="69abd-164">informationUrl</span></span>|<span data-ttu-id="69abd-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-165">String</span></span>|<span data-ttu-id="69abd-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="69abd-166">The more information Url.</span></span> <span data-ttu-id="69abd-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-168">owner</span><span class="sxs-lookup"><span data-stu-id="69abd-168">owner</span></span>|<span data-ttu-id="69abd-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-169">String</span></span>|<span data-ttu-id="69abd-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="69abd-170">The owner of the app.</span></span> <span data-ttu-id="69abd-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-172">developer</span><span class="sxs-lookup"><span data-stu-id="69abd-172">"developer"</span></span>|<span data-ttu-id="69abd-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-173">String</span></span>|<span data-ttu-id="69abd-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69abd-174">The developer of the app.</span></span> <span data-ttu-id="69abd-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-176">notes</span><span class="sxs-lookup"><span data-stu-id="69abd-176">Notes</span></span>|<span data-ttu-id="69abd-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-177">String</span></span>|<span data-ttu-id="69abd-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69abd-178">Notes for the app.</span></span> <span data-ttu-id="69abd-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="69abd-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="69abd-180">publishingState</span></span>|<span data-ttu-id="69abd-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-181">String</span></span>|<span data-ttu-id="69abd-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69abd-182">The publishing state for the app.</span></span> <span data-ttu-id="69abd-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="69abd-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="69abd-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="69abd-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="69abd-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="69abd-185">committedContentVersion</span></span>|<span data-ttu-id="69abd-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-186">String</span></span>|<span data-ttu-id="69abd-187">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="69abd-187">The internal committed content version.</span></span> <span data-ttu-id="69abd-188">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="69abd-189">fileName</span><span class="sxs-lookup"><span data-stu-id="69abd-189">fileName</span></span>|<span data-ttu-id="69abd-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-190">String</span></span>|<span data-ttu-id="69abd-191">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="69abd-191">The name of the main Lob application file.</span></span> <span data-ttu-id="69abd-192">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="69abd-193">size</span><span class="sxs-lookup"><span data-stu-id="69abd-193">size</span></span>|<span data-ttu-id="69abd-194">Int64</span><span class="sxs-lookup"><span data-stu-id="69abd-194">Int64</span></span>|<span data-ttu-id="69abd-195">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="69abd-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="69abd-196">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="69abd-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="69abd-197">commandLine</span><span class="sxs-lookup"><span data-stu-id="69abd-197">commandLine</span></span>|<span data-ttu-id="69abd-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-198">String</span></span>|<span data-ttu-id="69abd-199">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="69abd-199">The command line.</span></span>|
|<span data-ttu-id="69abd-200">productCode</span><span class="sxs-lookup"><span data-stu-id="69abd-200">ProductCode</span></span>|<span data-ttu-id="69abd-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-201">String</span></span>|<span data-ttu-id="69abd-202">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="69abd-202">The product code.</span></span>|
|<span data-ttu-id="69abd-203">productVersion</span><span class="sxs-lookup"><span data-stu-id="69abd-203">productVersion</span></span>|<span data-ttu-id="69abd-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abd-204">String</span></span>|<span data-ttu-id="69abd-205">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="69abd-205">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="69abd-206">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="69abd-206">ignoreVersionDetection</span></span>|<span data-ttu-id="69abd-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="69abd-207">Boolean</span></span>|<span data-ttu-id="69abd-208">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69abd-208">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="69abd-209">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="69abd-209">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="69abd-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="69abd-210">Response</span></span>
<span data-ttu-id="69abd-211">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69abd-211">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69abd-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69abd-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="69abd-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69abd-213">Request</span></span>
<span data-ttu-id="69abd-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69abd-214">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="69abd-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="69abd-215">Response</span></span>
<span data-ttu-id="69abd-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69abd-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



