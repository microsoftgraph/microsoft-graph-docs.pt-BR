# <a name="update-androidlobapp"></a><span data-ttu-id="55681-101">Atualizar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="55681-101">Update androidLobApp</span></span>

> <span data-ttu-id="55681-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="55681-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55681-103">Atualiza as propriedades de um objeto [androidLobApp](../resources/intune_apps_androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="55681-103">Update the properties of a [calendar](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55681-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55681-104">Prerequisites</span></span>
<span data-ttu-id="55681-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="55681-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="55681-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55681-107">Permission type</span></span>|<span data-ttu-id="55681-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55681-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55681-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55681-109">Delegated (work or school account)</span></span>|<span data-ttu-id="55681-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55681-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="55681-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55681-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55681-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55681-112">Not supported.</span></span>|
|<span data-ttu-id="55681-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55681-113">Application</span></span>|<span data-ttu-id="55681-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55681-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55681-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55681-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="55681-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55681-116">Request headers</span></span>
|<span data-ttu-id="55681-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55681-117">Header</span></span>|<span data-ttu-id="55681-118">Valor</span><span class="sxs-lookup"><span data-stu-id="55681-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55681-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="55681-119">Authorization</span></span>|<span data-ttu-id="55681-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55681-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="55681-121">Accept</span><span class="sxs-lookup"><span data-stu-id="55681-121">Accept</span></span>|<span data-ttu-id="55681-122">application/json</span><span class="sxs-lookup"><span data-stu-id="55681-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55681-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55681-123">Request body</span></span>
<span data-ttu-id="55681-124">No corpo da solicitação, forneça uma representação JSON do objeto [androidLobApp](../resources/intune_apps_androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="55681-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_androidlobapp.md) object.</span></span>

<span data-ttu-id="55681-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidLobApp](../resources/intune_apps_androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="55681-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="55681-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55681-126">Property</span></span>|<span data-ttu-id="55681-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="55681-127">Type</span></span>|<span data-ttu-id="55681-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="55681-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55681-129">id</span><span class="sxs-lookup"><span data-stu-id="55681-129">id</span></span>|<span data-ttu-id="55681-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-130">String</span></span>|<span data-ttu-id="55681-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="55681-131">Key of the setting.</span></span> <span data-ttu-id="55681-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-133">displayName</span><span class="sxs-lookup"><span data-stu-id="55681-133">displayName</span></span>|<span data-ttu-id="55681-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-134">String</span></span>|<span data-ttu-id="55681-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="55681-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="55681-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-137">description</span><span class="sxs-lookup"><span data-stu-id="55681-137">description</span></span>|<span data-ttu-id="55681-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-138">String</span></span>|<span data-ttu-id="55681-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55681-139">The description of the app.</span></span> <span data-ttu-id="55681-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-141">publisher</span><span class="sxs-lookup"><span data-stu-id="55681-141">Publisher</span></span>|<span data-ttu-id="55681-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-142">String</span></span>|<span data-ttu-id="55681-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55681-143">The publisher of the app.</span></span> <span data-ttu-id="55681-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="55681-145">largeIcon</span></span>|[<span data-ttu-id="55681-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="55681-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="55681-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="55681-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="55681-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55681-149">createdDateTime</span></span>|<span data-ttu-id="55681-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55681-150">DateTimeOffset</span></span>|<span data-ttu-id="55681-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55681-151">The date and time the group was created.</span></span> <span data-ttu-id="55681-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55681-153">lastModifiedDateTime</span></span>|<span data-ttu-id="55681-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55681-154">DateTimeOffset</span></span>|<span data-ttu-id="55681-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="55681-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="55681-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="55681-157">isFeatured</span></span>|<span data-ttu-id="55681-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="55681-158">Boolean</span></span>|<span data-ttu-id="55681-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="55681-160">privacyInformationUrl</span></span>|<span data-ttu-id="55681-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-161">String</span></span>|<span data-ttu-id="55681-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="55681-162">The privacy statement Url.</span></span> <span data-ttu-id="55681-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="55681-164">informationUrl</span></span>|<span data-ttu-id="55681-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-165">String</span></span>|<span data-ttu-id="55681-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="55681-166">The more information Url.</span></span> <span data-ttu-id="55681-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-168">owner</span><span class="sxs-lookup"><span data-stu-id="55681-168">owner</span></span>|<span data-ttu-id="55681-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-169">String</span></span>|<span data-ttu-id="55681-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="55681-170">The owner of the app.</span></span> <span data-ttu-id="55681-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-172">developer</span><span class="sxs-lookup"><span data-stu-id="55681-172">"developer"</span></span>|<span data-ttu-id="55681-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-173">String</span></span>|<span data-ttu-id="55681-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55681-174">The developer of the app.</span></span> <span data-ttu-id="55681-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-176">notes</span><span class="sxs-lookup"><span data-stu-id="55681-176">Notes</span></span>|<span data-ttu-id="55681-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-177">String</span></span>|<span data-ttu-id="55681-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55681-178">Notes for the app.</span></span> <span data-ttu-id="55681-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="55681-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="55681-180">publishingState</span></span>|<span data-ttu-id="55681-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-181">String</span></span>|<span data-ttu-id="55681-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55681-182">The publishing state for the app.</span></span> <span data-ttu-id="55681-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="55681-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="55681-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="55681-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="55681-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="55681-185">committedContentVersion</span></span>|<span data-ttu-id="55681-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-186">String</span></span>|<span data-ttu-id="55681-187">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="55681-187">The internal committed content version.</span></span> <span data-ttu-id="55681-188">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="55681-189">fileName</span><span class="sxs-lookup"><span data-stu-id="55681-189">fileName</span></span>|<span data-ttu-id="55681-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-190">String</span></span>|<span data-ttu-id="55681-191">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="55681-191">The name of the main Lob application file.</span></span> <span data-ttu-id="55681-192">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="55681-193">size</span><span class="sxs-lookup"><span data-stu-id="55681-193">size</span></span>|<span data-ttu-id="55681-194">Int64</span><span class="sxs-lookup"><span data-stu-id="55681-194">Int64</span></span>|<span data-ttu-id="55681-195">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="55681-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="55681-196">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="55681-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="55681-197">packageId</span><span class="sxs-lookup"><span data-stu-id="55681-197">packageId</span></span>|<span data-ttu-id="55681-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-198">String</span></span>|<span data-ttu-id="55681-199">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="55681-199">The package identifier.</span></span>|
|<span data-ttu-id="55681-200">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="55681-200">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="55681-201">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="55681-201">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="55681-202">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="55681-202">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="55681-203">versionName</span><span class="sxs-lookup"><span data-stu-id="55681-203">versionName</span></span>|<span data-ttu-id="55681-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-204">String</span></span>|<span data-ttu-id="55681-205">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="55681-205">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="55681-206">versionCode</span><span class="sxs-lookup"><span data-stu-id="55681-206">versionCode</span></span>|<span data-ttu-id="55681-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55681-207">String</span></span>|<span data-ttu-id="55681-208">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="55681-208">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="55681-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="55681-209">Response</span></span>
<span data-ttu-id="55681-210">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidLobApp](../resources/intune_apps_androidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55681-210">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55681-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55681-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="55681-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55681-212">Request</span></span>
<span data-ttu-id="55681-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55681-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1087

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

### <a name="response"></a><span data-ttu-id="55681-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="55681-214">Response</span></span>
<span data-ttu-id="55681-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55681-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



