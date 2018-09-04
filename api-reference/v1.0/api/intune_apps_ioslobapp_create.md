# <a name="create-ioslobapp"></a><span data-ttu-id="ce3ee-101">Criar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="ce3ee-101">Create iosLobApp</span></span>

> <span data-ttu-id="ce3ee-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce3ee-103">Cria um novo objeto [iosLobApp](../resources/intune_apps_ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce3ee-103">Create a new [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce3ee-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce3ee-104">Prerequisites</span></span>
<span data-ttu-id="ce3ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce3ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce3ee-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce3ee-107">Permission type</span></span>|<span data-ttu-id="ce3ee-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce3ee-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ce3ee-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce3ee-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce3ee-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce3ee-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-112">Not supported.</span></span>|
|<span data-ttu-id="ce3ee-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce3ee-113">Application</span></span>|<span data-ttu-id="ce3ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce3ee-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce3ee-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ce3ee-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce3ee-116">Request headers</span></span>
|<span data-ttu-id="ce3ee-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce3ee-117">Header</span></span>|<span data-ttu-id="ce3ee-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ce3ee-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce3ee-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce3ee-119">Authorization</span></span>|<span data-ttu-id="ce3ee-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="ce3ee-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce3ee-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ce3ee-121">Accept</span></span>|<span data-ttu-id="ce3ee-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ce3ee-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce3ee-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce3ee-123">Request body</span></span>
<span data-ttu-id="ce3ee-124">No corpo da solicitação, forneça uma representação JSON do objeto iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-124">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="ce3ee-125">A tabela a seguir mostra as propriedades obrigatórias ao criar iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-125">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="ce3ee-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce3ee-126">Property</span></span>|<span data-ttu-id="ce3ee-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce3ee-127">Type</span></span>|<span data-ttu-id="ce3ee-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce3ee-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce3ee-129">id</span><span class="sxs-lookup"><span data-stu-id="ce3ee-129">id</span></span>|<span data-ttu-id="ce3ee-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-130">String</span></span>|<span data-ttu-id="ce3ee-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-131">Key of the entity.</span></span> <span data-ttu-id="ce3ee-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ce3ee-133">displayName</span></span>|<span data-ttu-id="ce3ee-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-134">String</span></span>|<span data-ttu-id="ce3ee-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ce3ee-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-137">description</span><span class="sxs-lookup"><span data-stu-id="ce3ee-137">description</span></span>|<span data-ttu-id="ce3ee-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-138">String</span></span>|<span data-ttu-id="ce3ee-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-139">The description of the app.</span></span> <span data-ttu-id="ce3ee-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-141">publisher</span><span class="sxs-lookup"><span data-stu-id="ce3ee-141">publisher</span></span>|<span data-ttu-id="ce3ee-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-142">String</span></span>|<span data-ttu-id="ce3ee-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-143">The publisher of the app.</span></span> <span data-ttu-id="ce3ee-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ce3ee-145">largeIcon</span></span>|[<span data-ttu-id="ce3ee-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ce3ee-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="ce3ee-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ce3ee-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce3ee-149">createdDateTime</span></span>|<span data-ttu-id="ce3ee-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce3ee-150">DateTimeOffset</span></span>|<span data-ttu-id="ce3ee-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-151">The date and time the app was created.</span></span> <span data-ttu-id="ce3ee-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce3ee-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ce3ee-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce3ee-154">DateTimeOffset</span></span>|<span data-ttu-id="ce3ee-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-155">The date and time the app was last modified.</span></span> <span data-ttu-id="ce3ee-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ce3ee-157">isFeatured</span></span>|<span data-ttu-id="ce3ee-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="ce3ee-158">Boolean</span></span>|<span data-ttu-id="ce3ee-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ce3ee-160">privacyInformationUrl</span></span>|<span data-ttu-id="ce3ee-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-161">String</span></span>|<span data-ttu-id="ce3ee-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-162">The privacy statement Url.</span></span> <span data-ttu-id="ce3ee-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ce3ee-164">informationUrl</span></span>|<span data-ttu-id="ce3ee-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-165">String</span></span>|<span data-ttu-id="ce3ee-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-166">The more information Url.</span></span> <span data-ttu-id="ce3ee-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-168">owner</span><span class="sxs-lookup"><span data-stu-id="ce3ee-168">owner</span></span>|<span data-ttu-id="ce3ee-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-169">String</span></span>|<span data-ttu-id="ce3ee-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-170">The owner of the app.</span></span> <span data-ttu-id="ce3ee-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-172">developer</span><span class="sxs-lookup"><span data-stu-id="ce3ee-172">developer</span></span>|<span data-ttu-id="ce3ee-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-173">String</span></span>|<span data-ttu-id="ce3ee-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-174">The developer of the app.</span></span> <span data-ttu-id="ce3ee-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-176">Observações</span><span class="sxs-lookup"><span data-stu-id="ce3ee-176">notes</span></span>|<span data-ttu-id="ce3ee-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-177">String</span></span>|<span data-ttu-id="ce3ee-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-178">Notes for the app.</span></span> <span data-ttu-id="ce3ee-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ce3ee-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ce3ee-180">publishingState</span></span>|[<span data-ttu-id="ce3ee-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ce3ee-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="ce3ee-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-182">The publishing state for the app.</span></span> <span data-ttu-id="ce3ee-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ce3ee-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce3ee-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="ce3ee-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-185">The possible values are:</span></span>|
|<span data-ttu-id="ce3ee-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ce3ee-186">committedContentVersion</span></span>|<span data-ttu-id="ce3ee-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-187">String</span></span>|<span data-ttu-id="ce3ee-188">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-188">The internal committed content version.</span></span> <span data-ttu-id="ce3ee-189">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ce3ee-190">fileName</span><span class="sxs-lookup"><span data-stu-id="ce3ee-190">fileName</span></span>|<span data-ttu-id="ce3ee-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-191">String</span></span>|<span data-ttu-id="ce3ee-192">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-192">The name of the main Lob application file.</span></span> <span data-ttu-id="ce3ee-193">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ce3ee-194">size</span><span class="sxs-lookup"><span data-stu-id="ce3ee-194">size</span></span>|<span data-ttu-id="ce3ee-195">Int64</span><span class="sxs-lookup"><span data-stu-id="ce3ee-195">Int64</span></span>|<span data-ttu-id="ce3ee-196">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="ce3ee-197">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce3ee-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="ce3ee-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="ce3ee-198">bundleId</span></span>|<span data-ttu-id="ce3ee-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-199">String</span></span>|<span data-ttu-id="ce3ee-200">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-200">The Identity Name.</span></span>|
|<span data-ttu-id="ce3ee-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ce3ee-201">applicableDeviceType</span></span>|[<span data-ttu-id="ce3ee-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ce3ee-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="ce3ee-203">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="ce3ee-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ce3ee-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ce3ee-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ce3ee-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="ce3ee-206">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ce3ee-207">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ce3ee-207">expirationDateTime</span></span>|<span data-ttu-id="ce3ee-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce3ee-208">DateTimeOffset</span></span>|<span data-ttu-id="ce3ee-209">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-209">The expiration time.</span></span>|
|<span data-ttu-id="ce3ee-210">versionNumber</span><span class="sxs-lookup"><span data-stu-id="ce3ee-210">versionNumber</span></span>|<span data-ttu-id="ce3ee-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-211">String</span></span>|<span data-ttu-id="ce3ee-212">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-212">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ce3ee-213">buildNumber</span><span class="sxs-lookup"><span data-stu-id="ce3ee-213">buildNumber</span></span>|<span data-ttu-id="ce3ee-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce3ee-214">String</span></span>|<span data-ttu-id="ce3ee-215">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-215">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="ce3ee-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce3ee-216">Response</span></span>
<span data-ttu-id="ce3ee-217">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosLobApp](../resources/intune_apps_ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-217">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce3ee-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce3ee-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce3ee-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce3ee-219">Request</span></span>
<span data-ttu-id="ce3ee-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1253

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="ce3ee-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce3ee-221">Response</span></span>
<span data-ttu-id="ce3ee-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce3ee-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



