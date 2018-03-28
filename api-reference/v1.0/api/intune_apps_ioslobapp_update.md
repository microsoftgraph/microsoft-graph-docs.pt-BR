# <a name="update-ioslobapp"></a><span data-ttu-id="8cc2d-101">Atualizar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="8cc2d-101">Update iosLobApp</span></span>

> <span data-ttu-id="8cc2d-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cc2d-103">Atualiza as propriedades de um objeto [iosLobApp](../resources/intune_apps_ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8cc2d-103">Update the properties of a [calendar](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8cc2d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cc2d-104">Prerequisites</span></span>
<span data-ttu-id="8cc2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8cc2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8cc2d-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc2d-107">Permission type</span></span>|<span data-ttu-id="8cc2d-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cc2d-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8cc2d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc2d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8cc2d-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc2d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-112">Not supported.</span></span>|
|<span data-ttu-id="8cc2d-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc2d-113">Application</span></span>|<span data-ttu-id="8cc2d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc2d-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc2d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="8cc2d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc2d-116">Request headers</span></span>
|<span data-ttu-id="8cc2d-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cc2d-117">Header</span></span>|<span data-ttu-id="8cc2d-118">Valor</span><span class="sxs-lookup"><span data-stu-id="8cc2d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cc2d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cc2d-119">Authorization</span></span>|<span data-ttu-id="8cc2d-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8cc2d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8cc2d-121">Accept</span></span>|<span data-ttu-id="8cc2d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8cc2d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc2d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc2d-123">Request body</span></span>
<span data-ttu-id="8cc2d-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobApp](../resources/intune_apps_ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8cc2d-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_ioslobapp.md) object.</span></span>

<span data-ttu-id="8cc2d-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosLobApp.](../resources/intune_apps_ioslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="8cc2d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cc2d-126">Property</span></span>|<span data-ttu-id="8cc2d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc2d-127">Type</span></span>|<span data-ttu-id="8cc2d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc2d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc2d-129">id</span><span class="sxs-lookup"><span data-stu-id="8cc2d-129">id</span></span>|<span data-ttu-id="8cc2d-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-130">String</span></span>|<span data-ttu-id="8cc2d-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-131">Key of the setting.</span></span> <span data-ttu-id="8cc2d-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8cc2d-133">displayName</span></span>|<span data-ttu-id="8cc2d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-134">String</span></span>|<span data-ttu-id="8cc2d-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8cc2d-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-137">description</span><span class="sxs-lookup"><span data-stu-id="8cc2d-137">description</span></span>|<span data-ttu-id="8cc2d-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-138">String</span></span>|<span data-ttu-id="8cc2d-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-139">The description of the app.</span></span> <span data-ttu-id="8cc2d-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-141">publisher</span><span class="sxs-lookup"><span data-stu-id="8cc2d-141">Publisher</span></span>|<span data-ttu-id="8cc2d-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-142">String</span></span>|<span data-ttu-id="8cc2d-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-143">The publisher of the app.</span></span> <span data-ttu-id="8cc2d-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8cc2d-145">largeIcon</span></span>|[<span data-ttu-id="8cc2d-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8cc2d-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="8cc2d-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8cc2d-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc2d-149">createdDateTime</span></span>|<span data-ttu-id="8cc2d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc2d-150">DateTimeOffset</span></span>|<span data-ttu-id="8cc2d-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-151">The date and time the group was created.</span></span> <span data-ttu-id="8cc2d-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc2d-153">lastModifiedDateTime</span></span>|<span data-ttu-id="8cc2d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc2d-154">DateTimeOffset</span></span>|<span data-ttu-id="8cc2d-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="8cc2d-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8cc2d-157">isFeatured</span></span>|<span data-ttu-id="8cc2d-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="8cc2d-158">Boolean</span></span>|<span data-ttu-id="8cc2d-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8cc2d-160">privacyInformationUrl</span></span>|<span data-ttu-id="8cc2d-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-161">String</span></span>|<span data-ttu-id="8cc2d-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-162">The privacy statement Url.</span></span> <span data-ttu-id="8cc2d-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8cc2d-164">informationUrl</span></span>|<span data-ttu-id="8cc2d-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-165">String</span></span>|<span data-ttu-id="8cc2d-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-166">The more information Url.</span></span> <span data-ttu-id="8cc2d-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-168">owner</span><span class="sxs-lookup"><span data-stu-id="8cc2d-168">owner</span></span>|<span data-ttu-id="8cc2d-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-169">String</span></span>|<span data-ttu-id="8cc2d-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-170">The owner of the app.</span></span> <span data-ttu-id="8cc2d-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-172">developer</span><span class="sxs-lookup"><span data-stu-id="8cc2d-172">"developer"</span></span>|<span data-ttu-id="8cc2d-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-173">String</span></span>|<span data-ttu-id="8cc2d-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-174">The developer of the app.</span></span> <span data-ttu-id="8cc2d-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-176">notes</span><span class="sxs-lookup"><span data-stu-id="8cc2d-176">Notes</span></span>|<span data-ttu-id="8cc2d-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-177">String</span></span>|<span data-ttu-id="8cc2d-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-178">Notes for the app.</span></span> <span data-ttu-id="8cc2d-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="8cc2d-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="8cc2d-180">publishingState</span></span>|<span data-ttu-id="8cc2d-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-181">String</span></span>|<span data-ttu-id="8cc2d-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-182">The publishing state for the app.</span></span> <span data-ttu-id="8cc2d-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8cc2d-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8cc2d-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8cc2d-185">committedContentVersion</span></span>|<span data-ttu-id="8cc2d-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-186">String</span></span>|<span data-ttu-id="8cc2d-187">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-187">The internal committed content version.</span></span> <span data-ttu-id="8cc2d-188">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="8cc2d-189">fileName</span><span class="sxs-lookup"><span data-stu-id="8cc2d-189">fileName</span></span>|<span data-ttu-id="8cc2d-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-190">String</span></span>|<span data-ttu-id="8cc2d-191">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-191">The name of the main Lob application file.</span></span> <span data-ttu-id="8cc2d-192">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="8cc2d-193">size</span><span class="sxs-lookup"><span data-stu-id="8cc2d-193">size</span></span>|<span data-ttu-id="8cc2d-194">Int64</span><span class="sxs-lookup"><span data-stu-id="8cc2d-194">Int64</span></span>|<span data-ttu-id="8cc2d-195">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="8cc2d-196">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc2d-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="8cc2d-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="8cc2d-197">bundleId</span></span>|<span data-ttu-id="8cc2d-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-198">String</span></span>|<span data-ttu-id="8cc2d-199">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-199">The Identity Name.</span></span>|
|<span data-ttu-id="8cc2d-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="8cc2d-200">applicableDeviceType</span></span>|[<span data-ttu-id="8cc2d-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="8cc2d-201">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="8cc2d-202">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-202">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="8cc2d-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8cc2d-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8cc2d-204">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8cc2d-204">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="8cc2d-205">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8cc2d-206">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc2d-206">expirationDateTime</span></span>|<span data-ttu-id="8cc2d-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc2d-207">DateTimeOffset</span></span>|<span data-ttu-id="8cc2d-208">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-208">: The expiration time for the subscription.</span></span>|
|<span data-ttu-id="8cc2d-209">versionNumber</span><span class="sxs-lookup"><span data-stu-id="8cc2d-209">versionNumber</span></span>|<span data-ttu-id="8cc2d-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-210">String</span></span>|<span data-ttu-id="8cc2d-211">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-211">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8cc2d-212">buildNumber</span><span class="sxs-lookup"><span data-stu-id="8cc2d-212">buildNumber</span></span>|<span data-ttu-id="8cc2d-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc2d-213">String</span></span>|<span data-ttu-id="8cc2d-214">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-214">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="8cc2d-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc2d-215">Response</span></span>
<span data-ttu-id="8cc2d-216">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosLobApp](../resources/intune_apps_ioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-216">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc2d-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc2d-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="8cc2d-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc2d-218">Request</span></span>
<span data-ttu-id="8cc2d-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1205

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

### <a name="response"></a><span data-ttu-id="8cc2d-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc2d-220">Response</span></span>
<span data-ttu-id="8cc2d-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc2d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



