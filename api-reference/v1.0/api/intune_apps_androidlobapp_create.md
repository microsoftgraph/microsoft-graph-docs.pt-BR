# <a name="create-androidlobapp"></a><span data-ttu-id="df2cb-101">Criar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="df2cb-101">Create androidLobApp</span></span>

> <span data-ttu-id="df2cb-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="df2cb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df2cb-103">Cria um novo objeto [androidLobApp](../resources/intune_apps_androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="df2cb-103">Create a new [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df2cb-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df2cb-104">Prerequisites</span></span>
<span data-ttu-id="df2cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="df2cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="df2cb-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df2cb-107">Permission type</span></span>|<span data-ttu-id="df2cb-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df2cb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df2cb-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df2cb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="df2cb-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df2cb-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="df2cb-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df2cb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df2cb-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df2cb-112">Not supported.</span></span>|
|<span data-ttu-id="df2cb-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df2cb-113">Application</span></span>|<span data-ttu-id="df2cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df2cb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df2cb-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df2cb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="df2cb-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df2cb-116">Request headers</span></span>
|<span data-ttu-id="df2cb-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df2cb-117">Header</span></span>|<span data-ttu-id="df2cb-118">Valor</span><span class="sxs-lookup"><span data-stu-id="df2cb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df2cb-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="df2cb-119">Authorization</span></span>|<span data-ttu-id="df2cb-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="df2cb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df2cb-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df2cb-121">Accept</span></span>|<span data-ttu-id="df2cb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="df2cb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df2cb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df2cb-123">Request body</span></span>
<span data-ttu-id="df2cb-124">No corpo da solicitação, forneça uma representação JSON do objeto androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="df2cb-124">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="df2cb-125">A tabela a seguir mostra as propriedades obrigatórias ao criar androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="df2cb-125">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="df2cb-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df2cb-126">Property</span></span>|<span data-ttu-id="df2cb-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="df2cb-127">Type</span></span>|<span data-ttu-id="df2cb-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="df2cb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df2cb-129">id</span><span class="sxs-lookup"><span data-stu-id="df2cb-129">id</span></span>|<span data-ttu-id="df2cb-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-130">String</span></span>|<span data-ttu-id="df2cb-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="df2cb-131">Key of the entity.</span></span> <span data-ttu-id="df2cb-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="df2cb-133">displayName</span></span>|<span data-ttu-id="df2cb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-134">String</span></span>|<span data-ttu-id="df2cb-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="df2cb-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="df2cb-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-137">description</span><span class="sxs-lookup"><span data-stu-id="df2cb-137">description</span></span>|<span data-ttu-id="df2cb-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-138">String</span></span>|<span data-ttu-id="df2cb-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df2cb-139">The description of the app.</span></span> <span data-ttu-id="df2cb-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-141">publisher</span><span class="sxs-lookup"><span data-stu-id="df2cb-141">publisher</span></span>|<span data-ttu-id="df2cb-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-142">String</span></span>|<span data-ttu-id="df2cb-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df2cb-143">The publisher of the app.</span></span> <span data-ttu-id="df2cb-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="df2cb-145">largeIcon</span></span>|[<span data-ttu-id="df2cb-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df2cb-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="df2cb-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="df2cb-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="df2cb-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df2cb-149">createdDateTime</span></span>|<span data-ttu-id="df2cb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df2cb-150">DateTimeOffset</span></span>|<span data-ttu-id="df2cb-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df2cb-151">The date and time the app was created.</span></span> <span data-ttu-id="df2cb-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df2cb-153">lastModifiedDateTime</span></span>|<span data-ttu-id="df2cb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df2cb-154">DateTimeOffset</span></span>|<span data-ttu-id="df2cb-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="df2cb-155">The date and time the app was last modified.</span></span> <span data-ttu-id="df2cb-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="df2cb-157">isFeatured</span></span>|<span data-ttu-id="df2cb-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="df2cb-158">Boolean</span></span>|<span data-ttu-id="df2cb-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="df2cb-160">privacyInformationUrl</span></span>|<span data-ttu-id="df2cb-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-161">String</span></span>|<span data-ttu-id="df2cb-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="df2cb-162">The privacy statement Url.</span></span> <span data-ttu-id="df2cb-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="df2cb-164">informationUrl</span></span>|<span data-ttu-id="df2cb-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-165">String</span></span>|<span data-ttu-id="df2cb-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="df2cb-166">The more information Url.</span></span> <span data-ttu-id="df2cb-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-168">owner</span><span class="sxs-lookup"><span data-stu-id="df2cb-168">owner</span></span>|<span data-ttu-id="df2cb-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-169">String</span></span>|<span data-ttu-id="df2cb-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="df2cb-170">The owner of the app.</span></span> <span data-ttu-id="df2cb-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-172">developer</span><span class="sxs-lookup"><span data-stu-id="df2cb-172">developer</span></span>|<span data-ttu-id="df2cb-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-173">String</span></span>|<span data-ttu-id="df2cb-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df2cb-174">The developer of the app.</span></span> <span data-ttu-id="df2cb-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-176">Observações</span><span class="sxs-lookup"><span data-stu-id="df2cb-176">notes</span></span>|<span data-ttu-id="df2cb-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-177">String</span></span>|<span data-ttu-id="df2cb-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df2cb-178">Notes for the app.</span></span> <span data-ttu-id="df2cb-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="df2cb-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="df2cb-180">publishingState</span></span>|[<span data-ttu-id="df2cb-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="df2cb-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="df2cb-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df2cb-182">The publishing state for the app.</span></span> <span data-ttu-id="df2cb-183">O aplicativo não pode ser atribuído, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="df2cb-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="df2cb-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="df2cb-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="df2cb-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="df2cb-185">The possible values are:</span></span>|
|<span data-ttu-id="df2cb-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="df2cb-186">committedContentVersion</span></span>|<span data-ttu-id="df2cb-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-187">String</span></span>|<span data-ttu-id="df2cb-188">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="df2cb-188">The internal committed content version.</span></span> <span data-ttu-id="df2cb-189">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="df2cb-190">fileName</span><span class="sxs-lookup"><span data-stu-id="df2cb-190">fileName</span></span>|<span data-ttu-id="df2cb-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-191">String</span></span>|<span data-ttu-id="df2cb-192">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="df2cb-192">The name of the main Lob application file.</span></span> <span data-ttu-id="df2cb-193">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="df2cb-194">size</span><span class="sxs-lookup"><span data-stu-id="df2cb-194">size</span></span>|<span data-ttu-id="df2cb-195">Int64</span><span class="sxs-lookup"><span data-stu-id="df2cb-195">Int64</span></span>|<span data-ttu-id="df2cb-196">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="df2cb-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="df2cb-197">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="df2cb-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="df2cb-198">packageId</span><span class="sxs-lookup"><span data-stu-id="df2cb-198">packageId</span></span>|<span data-ttu-id="df2cb-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-199">String</span></span>|<span data-ttu-id="df2cb-200">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="df2cb-200">The package identifier.</span></span>|
|<span data-ttu-id="df2cb-201">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="df2cb-201">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="df2cb-202">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="df2cb-202">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="df2cb-203">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="df2cb-203">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="df2cb-204">versionName</span><span class="sxs-lookup"><span data-stu-id="df2cb-204">versionName</span></span>|<span data-ttu-id="df2cb-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-205">String</span></span>|<span data-ttu-id="df2cb-206">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="df2cb-206">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="df2cb-207">versionCode</span><span class="sxs-lookup"><span data-stu-id="df2cb-207">versionCode</span></span>|<span data-ttu-id="df2cb-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df2cb-208">String</span></span>|<span data-ttu-id="df2cb-209">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="df2cb-209">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="df2cb-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="df2cb-210">Response</span></span>
<span data-ttu-id="df2cb-211">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [androidLobApp](../resources/intune_apps_androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df2cb-211">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df2cb-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df2cb-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="df2cb-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df2cb-213">Request</span></span>
<span data-ttu-id="df2cb-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df2cb-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1139

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="df2cb-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="df2cb-215">Response</span></span>
<span data-ttu-id="df2cb-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df2cb-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



