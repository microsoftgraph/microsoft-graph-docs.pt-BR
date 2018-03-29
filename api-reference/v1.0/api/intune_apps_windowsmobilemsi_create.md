# <a name="create-windowsmobilemsi"></a><span data-ttu-id="ce009-101">Criar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="ce009-101">Create windowsMobileMSI</span></span>

> <span data-ttu-id="ce009-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ce009-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce009-103">Cria um novo objeto [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="ce009-103">Create a new [plannerBucket](../resources/intune_apps_windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce009-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce009-104">Prerequisites</span></span>
<span data-ttu-id="ce009-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce009-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce009-107">Permission type</span></span>|<span data-ttu-id="ce009-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ce009-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce009-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce009-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ce009-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce009-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce009-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce009-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce009-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce009-112">Not supported.</span></span>|
|<span data-ttu-id="ce009-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce009-113">Application</span></span>|<span data-ttu-id="ce009-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce009-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce009-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce009-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ce009-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce009-116">Request headers</span></span>
|<span data-ttu-id="ce009-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce009-117">Header</span></span>|<span data-ttu-id="ce009-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ce009-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce009-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce009-119">Authorization</span></span>|<span data-ttu-id="ce009-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce009-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce009-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ce009-121">Accept</span></span>|<span data-ttu-id="ce009-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ce009-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce009-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce009-123">Request body</span></span>
<span data-ttu-id="ce009-124">No corpo da solicitação, forneça uma representação JSON para o objeto windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="ce009-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ce009-125">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="ce009-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="ce009-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce009-126">Property</span></span>|<span data-ttu-id="ce009-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce009-127">Type</span></span>|<span data-ttu-id="ce009-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce009-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce009-129">id</span><span class="sxs-lookup"><span data-stu-id="ce009-129">id</span></span>|<span data-ttu-id="ce009-130">String</span><span class="sxs-lookup"><span data-stu-id="ce009-130">String</span></span>|<span data-ttu-id="ce009-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ce009-131">Key of the setting.</span></span> <span data-ttu-id="ce009-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ce009-133">displayName</span></span>|<span data-ttu-id="ce009-134">String</span><span class="sxs-lookup"><span data-stu-id="ce009-134">String</span></span>|<span data-ttu-id="ce009-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ce009-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ce009-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-137">descrição</span><span class="sxs-lookup"><span data-stu-id="ce009-137">description</span></span>|<span data-ttu-id="ce009-138">String</span><span class="sxs-lookup"><span data-stu-id="ce009-138">String</span></span>|<span data-ttu-id="ce009-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce009-139">The description of the app.</span></span> <span data-ttu-id="ce009-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-141">publicador</span><span class="sxs-lookup"><span data-stu-id="ce009-141">Publisher</span></span>|<span data-ttu-id="ce009-142">String</span><span class="sxs-lookup"><span data-stu-id="ce009-142">String</span></span>|<span data-ttu-id="ce009-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce009-143">The publisher of the app.</span></span> <span data-ttu-id="ce009-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ce009-145">largeIcon</span></span>|[<span data-ttu-id="ce009-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ce009-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="ce009-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ce009-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ce009-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce009-149">createdDateTime</span></span>|<span data-ttu-id="ce009-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce009-150">DateTimeOffset</span></span>|<span data-ttu-id="ce009-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce009-151">The date and time the group was created.</span></span> <span data-ttu-id="ce009-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce009-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ce009-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce009-154">DateTimeOffset</span></span>|<span data-ttu-id="ce009-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ce009-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="ce009-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ce009-157">isFeatured</span></span>|<span data-ttu-id="ce009-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce009-158">Boolean</span></span>|<span data-ttu-id="ce009-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ce009-160">privacyInformationUrl</span></span>|<span data-ttu-id="ce009-161">String</span><span class="sxs-lookup"><span data-stu-id="ce009-161">String</span></span>|<span data-ttu-id="ce009-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ce009-162">The privacy statement Url.</span></span> <span data-ttu-id="ce009-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ce009-164">informationUrl</span></span>|<span data-ttu-id="ce009-165">String</span><span class="sxs-lookup"><span data-stu-id="ce009-165">String</span></span>|<span data-ttu-id="ce009-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ce009-166">The more information Url.</span></span> <span data-ttu-id="ce009-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-168">owner</span><span class="sxs-lookup"><span data-stu-id="ce009-168">owner</span></span>|<span data-ttu-id="ce009-169">String</span><span class="sxs-lookup"><span data-stu-id="ce009-169">String</span></span>|<span data-ttu-id="ce009-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ce009-170">The owner of the app.</span></span> <span data-ttu-id="ce009-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-172">developer</span><span class="sxs-lookup"><span data-stu-id="ce009-172">"developer"</span></span>|<span data-ttu-id="ce009-173">String</span><span class="sxs-lookup"><span data-stu-id="ce009-173">String</span></span>|<span data-ttu-id="ce009-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce009-174">The developer of the app.</span></span> <span data-ttu-id="ce009-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-176">Observações</span><span class="sxs-lookup"><span data-stu-id="ce009-176">Notes</span></span>|<span data-ttu-id="ce009-177">String</span><span class="sxs-lookup"><span data-stu-id="ce009-177">String</span></span>|<span data-ttu-id="ce009-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce009-178">Notes for the app.</span></span> <span data-ttu-id="ce009-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce009-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ce009-180">publishingState</span></span>|<span data-ttu-id="ce009-181">String</span><span class="sxs-lookup"><span data-stu-id="ce009-181">String</span></span>|<span data-ttu-id="ce009-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce009-182">The publishing state for the app.</span></span> <span data-ttu-id="ce009-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ce009-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ce009-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ce009-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ce009-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ce009-185">committedContentVersion</span></span>|<span data-ttu-id="ce009-186">String</span><span class="sxs-lookup"><span data-stu-id="ce009-186">String</span></span>|<span data-ttu-id="ce009-187">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="ce009-187">The internal committed content version.</span></span> <span data-ttu-id="ce009-188">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ce009-189">fileName</span><span class="sxs-lookup"><span data-stu-id="ce009-189">fileName</span></span>|<span data-ttu-id="ce009-190">String</span><span class="sxs-lookup"><span data-stu-id="ce009-190">String</span></span>|<span data-ttu-id="ce009-191">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="ce009-191">The name of the main Lob application file.</span></span> <span data-ttu-id="ce009-192">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ce009-193">size</span><span class="sxs-lookup"><span data-stu-id="ce009-193">size</span></span>|<span data-ttu-id="ce009-194">Int64</span><span class="sxs-lookup"><span data-stu-id="ce009-194">Int64</span></span>|<span data-ttu-id="ce009-195">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="ce009-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="ce009-196">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce009-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ce009-197">commandLine</span><span class="sxs-lookup"><span data-stu-id="ce009-197">commandLine</span></span>|<span data-ttu-id="ce009-198">String</span><span class="sxs-lookup"><span data-stu-id="ce009-198">String</span></span>|<span data-ttu-id="ce009-199">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="ce009-199">The command line.</span></span>|
|<span data-ttu-id="ce009-200">productCode</span><span class="sxs-lookup"><span data-stu-id="ce009-200">ProductCode</span></span>|<span data-ttu-id="ce009-201">String</span><span class="sxs-lookup"><span data-stu-id="ce009-201">String</span></span>|<span data-ttu-id="ce009-202">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="ce009-202">The product code.</span></span>|
|<span data-ttu-id="ce009-203">productVersion</span><span class="sxs-lookup"><span data-stu-id="ce009-203">productVersion</span></span>|<span data-ttu-id="ce009-204">String</span><span class="sxs-lookup"><span data-stu-id="ce009-204">String</span></span>|<span data-ttu-id="ce009-205">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="ce009-205">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ce009-206">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="ce009-206">ignoreVersionDetection</span></span>|<span data-ttu-id="ce009-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce009-207">Boolean</span></span>|<span data-ttu-id="ce009-208">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce009-208">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="ce009-209">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="ce009-209">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="ce009-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce009-210">Response</span></span>
<span data-ttu-id="ce009-211">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce009-211">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_apps_windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce009-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce009-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce009-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce009-213">Request</span></span>
<span data-ttu-id="ce009-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce009-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 919

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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

### <a name="response"></a><span data-ttu-id="ce009-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce009-215">Response</span></span>
<span data-ttu-id="ce009-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce009-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



