# <a name="update-ioslobapp"></a><span data-ttu-id="9a2e0-101">Atualizar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="9a2e0-101">Update iosLobApp</span></span>

> <span data-ttu-id="9a2e0-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a2e0-103">Atualiza as propriedades de um objeto [iosLobApp](../resources/intune_apps_ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2e0-103">Update the properties of a [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9a2e0-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a2e0-104">Prerequisites</span></span>
<span data-ttu-id="9a2e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a2e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a2e0-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a2e0-107">Permission type</span></span>|<span data-ttu-id="9a2e0-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a2e0-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9a2e0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a2e0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9a2e0-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a2e0-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-112">Not supported.</span></span>|
|<span data-ttu-id="9a2e0-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a2e0-113">Application</span></span>|<span data-ttu-id="9a2e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a2e0-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a2e0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="9a2e0-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a2e0-116">Request headers</span></span>
|<span data-ttu-id="9a2e0-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a2e0-117">Header</span></span>|<span data-ttu-id="9a2e0-118">Valor</span><span class="sxs-lookup"><span data-stu-id="9a2e0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a2e0-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a2e0-119">Authorization</span></span>|<span data-ttu-id="9a2e0-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="9a2e0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a2e0-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a2e0-121">Accept</span></span>|<span data-ttu-id="9a2e0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9a2e0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a2e0-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a2e0-123">Request body</span></span>
<span data-ttu-id="9a2e0-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobApp](../resources/intune_apps_ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2e0-124">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune_apps_ioslobapp.md) object.</span></span>

<span data-ttu-id="9a2e0-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosLobApp.](../resources/intune_apps_ioslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-125">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune_apps_ioslobapp.md).</span></span>

|<span data-ttu-id="9a2e0-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a2e0-126">Property</span></span>|<span data-ttu-id="9a2e0-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a2e0-127">Type</span></span>|<span data-ttu-id="9a2e0-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a2e0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a2e0-129">id</span><span class="sxs-lookup"><span data-stu-id="9a2e0-129">id</span></span>|<span data-ttu-id="9a2e0-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-130">String</span></span>|<span data-ttu-id="9a2e0-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-131">Key of the entity.</span></span> <span data-ttu-id="9a2e0-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9a2e0-133">displayName</span></span>|<span data-ttu-id="9a2e0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-134">String</span></span>|<span data-ttu-id="9a2e0-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9a2e0-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-137">descrição</span><span class="sxs-lookup"><span data-stu-id="9a2e0-137">description</span></span>|<span data-ttu-id="9a2e0-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-138">String</span></span>|<span data-ttu-id="9a2e0-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-139">The description of the app.</span></span> <span data-ttu-id="9a2e0-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-141">publisher</span><span class="sxs-lookup"><span data-stu-id="9a2e0-141">publisher</span></span>|<span data-ttu-id="9a2e0-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-142">String</span></span>|<span data-ttu-id="9a2e0-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-143">The publisher of the app.</span></span> <span data-ttu-id="9a2e0-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9a2e0-145">largeIcon</span></span>|[<span data-ttu-id="9a2e0-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9a2e0-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="9a2e0-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9a2e0-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a2e0-149">createdDateTime</span></span>|<span data-ttu-id="9a2e0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a2e0-150">DateTimeOffset</span></span>|<span data-ttu-id="9a2e0-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-151">The date and time the app was created.</span></span> <span data-ttu-id="9a2e0-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a2e0-153">lastModifiedDateTime</span></span>|<span data-ttu-id="9a2e0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a2e0-154">DateTimeOffset</span></span>|<span data-ttu-id="9a2e0-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-155">The date and time the app was last modified.</span></span> <span data-ttu-id="9a2e0-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9a2e0-157">isFeatured</span></span>|<span data-ttu-id="9a2e0-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="9a2e0-158">Boolean</span></span>|<span data-ttu-id="9a2e0-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9a2e0-160">privacyInformationUrl</span></span>|<span data-ttu-id="9a2e0-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-161">String</span></span>|<span data-ttu-id="9a2e0-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-162">The privacy statement Url.</span></span> <span data-ttu-id="9a2e0-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9a2e0-164">informationUrl</span></span>|<span data-ttu-id="9a2e0-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-165">String</span></span>|<span data-ttu-id="9a2e0-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-166">The more information Url.</span></span> <span data-ttu-id="9a2e0-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-168">owner</span><span class="sxs-lookup"><span data-stu-id="9a2e0-168">owner</span></span>|<span data-ttu-id="9a2e0-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-169">String</span></span>|<span data-ttu-id="9a2e0-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-170">The owner of the app.</span></span> <span data-ttu-id="9a2e0-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-172">developer</span><span class="sxs-lookup"><span data-stu-id="9a2e0-172">developer</span></span>|<span data-ttu-id="9a2e0-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-173">String</span></span>|<span data-ttu-id="9a2e0-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-174">The developer of the app.</span></span> <span data-ttu-id="9a2e0-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-176">Observações</span><span class="sxs-lookup"><span data-stu-id="9a2e0-176">notes</span></span>|<span data-ttu-id="9a2e0-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-177">String</span></span>|<span data-ttu-id="9a2e0-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-178">Notes for the app.</span></span> <span data-ttu-id="9a2e0-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="9a2e0-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="9a2e0-180">publishingState</span></span>|[<span data-ttu-id="9a2e0-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9a2e0-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="9a2e0-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-182">The publishing state for the app.</span></span> <span data-ttu-id="9a2e0-183">O aplicativo não pode ser atribuído, a menos que seja publicado.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9a2e0-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a2e0-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="9a2e0-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9a2e0-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9a2e0-186">committedContentVersion</span></span>|<span data-ttu-id="9a2e0-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-187">String</span></span>|<span data-ttu-id="9a2e0-188">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-188">The internal committed content version.</span></span> <span data-ttu-id="9a2e0-189">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="9a2e0-190">fileName</span><span class="sxs-lookup"><span data-stu-id="9a2e0-190">fileName</span></span>|<span data-ttu-id="9a2e0-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-191">String</span></span>|<span data-ttu-id="9a2e0-192">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-192">The name of the main Lob application file.</span></span> <span data-ttu-id="9a2e0-193">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="9a2e0-194">size</span><span class="sxs-lookup"><span data-stu-id="9a2e0-194">size</span></span>|<span data-ttu-id="9a2e0-195">Int64</span><span class="sxs-lookup"><span data-stu-id="9a2e0-195">Int64</span></span>|<span data-ttu-id="9a2e0-196">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="9a2e0-197">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a2e0-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="9a2e0-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="9a2e0-198">bundleId</span></span>|<span data-ttu-id="9a2e0-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-199">String</span></span>|<span data-ttu-id="9a2e0-200">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-200">The Identity Name.</span></span>|
|<span data-ttu-id="9a2e0-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9a2e0-201">applicableDeviceType</span></span>|[<span data-ttu-id="9a2e0-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9a2e0-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="9a2e0-203">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-203">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9a2e0-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9a2e0-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9a2e0-205">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9a2e0-205">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="9a2e0-206">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9a2e0-207">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9a2e0-207">expirationDateTime</span></span>|<span data-ttu-id="9a2e0-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a2e0-208">DateTimeOffset</span></span>|<span data-ttu-id="9a2e0-209">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-209">The expiration time.</span></span>|
|<span data-ttu-id="9a2e0-210">versionNumber</span><span class="sxs-lookup"><span data-stu-id="9a2e0-210">versionNumber</span></span>|<span data-ttu-id="9a2e0-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-211">String</span></span>|<span data-ttu-id="9a2e0-212">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-212">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9a2e0-213">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9a2e0-213">buildNumber</span></span>|<span data-ttu-id="9a2e0-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2e0-214">String</span></span>|<span data-ttu-id="9a2e0-215">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-215">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="9a2e0-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a2e0-216">Response</span></span>
<span data-ttu-id="9a2e0-217">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosLobApp](../resources/intune_apps_ioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-217">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune_apps_ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a2e0-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a2e0-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a2e0-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a2e0-219">Request</span></span>
<span data-ttu-id="9a2e0-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a2e0-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a2e0-221">Response</span></span>
<span data-ttu-id="9a2e0-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a2e0-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








