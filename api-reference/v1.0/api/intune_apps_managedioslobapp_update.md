# <a name="update-managedioslobapp"></a><span data-ttu-id="990df-101">Atualizar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="990df-101">Update managedIOSLobApp</span></span>

> <span data-ttu-id="990df-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="990df-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="990df-103">Atualiza as propriedades de um objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="990df-103">Update the properties of a [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="990df-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="990df-104">Prerequisites</span></span>
<span data-ttu-id="990df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="990df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="990df-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="990df-107">Permission type</span></span>|<span data-ttu-id="990df-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="990df-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="990df-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="990df-109">Delegated (work or school account)</span></span>|<span data-ttu-id="990df-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="990df-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="990df-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="990df-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="990df-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="990df-112">Not supported.</span></span>|
|<span data-ttu-id="990df-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="990df-113">Application</span></span>|<span data-ttu-id="990df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="990df-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="990df-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="990df-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="990df-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="990df-116">Request headers</span></span>
|<span data-ttu-id="990df-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="990df-117">Header</span></span>|<span data-ttu-id="990df-118">Valor</span><span class="sxs-lookup"><span data-stu-id="990df-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="990df-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="990df-119">Authorization</span></span>|<span data-ttu-id="990df-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="990df-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="990df-121">Accept</span><span class="sxs-lookup"><span data-stu-id="990df-121">Accept</span></span>|<span data-ttu-id="990df-122">application/json</span><span class="sxs-lookup"><span data-stu-id="990df-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="990df-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="990df-123">Request body</span></span>
<span data-ttu-id="990df-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="990df-124">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>

<span data-ttu-id="990df-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="990df-125">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span></span>

|<span data-ttu-id="990df-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="990df-126">Property</span></span>|<span data-ttu-id="990df-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="990df-127">Type</span></span>|<span data-ttu-id="990df-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="990df-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="990df-129">id</span><span class="sxs-lookup"><span data-stu-id="990df-129">id</span></span>|<span data-ttu-id="990df-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="990df-130">String</span></span>|<span data-ttu-id="990df-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="990df-131">Key of the entity.</span></span> <span data-ttu-id="990df-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-133">displayName</span><span class="sxs-lookup"><span data-stu-id="990df-133">displayName</span></span>|<span data-ttu-id="990df-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="990df-134">String</span></span>|<span data-ttu-id="990df-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="990df-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="990df-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-137">description</span><span class="sxs-lookup"><span data-stu-id="990df-137">description</span></span>|<span data-ttu-id="990df-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="990df-138">String</span></span>|<span data-ttu-id="990df-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="990df-139">The description of the app.</span></span> <span data-ttu-id="990df-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-141">publisher</span><span class="sxs-lookup"><span data-stu-id="990df-141">publisher</span></span>|<span data-ttu-id="990df-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="990df-142">String</span></span>|<span data-ttu-id="990df-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="990df-143">The publisher of the app.</span></span> <span data-ttu-id="990df-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="990df-145">largeIcon</span></span>|[<span data-ttu-id="990df-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="990df-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="990df-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="990df-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="990df-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="990df-149">createdDateTime</span></span>|<span data-ttu-id="990df-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="990df-150">DateTimeOffset</span></span>|<span data-ttu-id="990df-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="990df-151">The date and time the app was created.</span></span> <span data-ttu-id="990df-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="990df-153">lastModifiedDateTime</span></span>|<span data-ttu-id="990df-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="990df-154">DateTimeOffset</span></span>|<span data-ttu-id="990df-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="990df-155">The date and time the app was last modified.</span></span> <span data-ttu-id="990df-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="990df-157">isFeatured</span></span>|<span data-ttu-id="990df-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="990df-158">Boolean</span></span>|<span data-ttu-id="990df-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="990df-160">privacyInformationUrl</span></span>|<span data-ttu-id="990df-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="990df-161">String</span></span>|<span data-ttu-id="990df-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="990df-162">The privacy statement Url.</span></span> <span data-ttu-id="990df-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="990df-164">informationUrl</span></span>|<span data-ttu-id="990df-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="990df-165">String</span></span>|<span data-ttu-id="990df-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="990df-166">The more information Url.</span></span> <span data-ttu-id="990df-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-168">owner</span><span class="sxs-lookup"><span data-stu-id="990df-168">owner</span></span>|<span data-ttu-id="990df-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="990df-169">String</span></span>|<span data-ttu-id="990df-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="990df-170">The owner of the app.</span></span> <span data-ttu-id="990df-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-172">developer</span><span class="sxs-lookup"><span data-stu-id="990df-172">developer</span></span>|<span data-ttu-id="990df-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="990df-173">String</span></span>|<span data-ttu-id="990df-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="990df-174">The developer of the app.</span></span> <span data-ttu-id="990df-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-176">notes</span><span class="sxs-lookup"><span data-stu-id="990df-176">notes</span></span>|<span data-ttu-id="990df-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="990df-177">String</span></span>|<span data-ttu-id="990df-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="990df-178">Notes for the app.</span></span> <span data-ttu-id="990df-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="990df-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="990df-180">publishingState</span></span>|[<span data-ttu-id="990df-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="990df-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="990df-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="990df-182">The publishing state for the app.</span></span> <span data-ttu-id="990df-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="990df-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="990df-184">Herdada do [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="990df-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="990df-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="990df-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="990df-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="990df-186">appAvailability</span></span>|[<span data-ttu-id="990df-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="990df-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="990df-188">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="990df-188">The Application's availability.</span></span> <span data-ttu-id="990df-189">Herdada do [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="990df-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md).</span></span> <span data-ttu-id="990df-190">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="990df-190">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="990df-191">version</span><span class="sxs-lookup"><span data-stu-id="990df-191">version</span></span>|<span data-ttu-id="990df-192">String</span><span class="sxs-lookup"><span data-stu-id="990df-192">String</span></span>|<span data-ttu-id="990df-193">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="990df-193">The Application's version.</span></span> <span data-ttu-id="990df-194">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="990df-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="990df-195">committedContentVersion</span></span>|<span data-ttu-id="990df-196">String</span><span class="sxs-lookup"><span data-stu-id="990df-196">String</span></span>|<span data-ttu-id="990df-197">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="990df-197">The internal committed content version.</span></span> <span data-ttu-id="990df-198">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="990df-199">fileName</span><span class="sxs-lookup"><span data-stu-id="990df-199">fileName</span></span>|<span data-ttu-id="990df-200">String</span><span class="sxs-lookup"><span data-stu-id="990df-200">String</span></span>|<span data-ttu-id="990df-201">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="990df-201">The name of the main Lob application file.</span></span> <span data-ttu-id="990df-202">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="990df-203">size</span><span class="sxs-lookup"><span data-stu-id="990df-203">size</span></span>|<span data-ttu-id="990df-204">Int64</span><span class="sxs-lookup"><span data-stu-id="990df-204">Int64</span></span>|<span data-ttu-id="990df-205">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="990df-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="990df-206">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="990df-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="990df-207">bundleId</span><span class="sxs-lookup"><span data-stu-id="990df-207">bundleId</span></span>|<span data-ttu-id="990df-208">String</span><span class="sxs-lookup"><span data-stu-id="990df-208">String</span></span>|<span data-ttu-id="990df-209">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="990df-209">The Identity Name.</span></span>|
|<span data-ttu-id="990df-210">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="990df-210">applicableDeviceType</span></span>|[<span data-ttu-id="990df-211">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="990df-211">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="990df-212">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="990df-212">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="990df-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="990df-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="990df-214">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="990df-214">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="990df-215">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="990df-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="990df-216">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="990df-216">expirationDateTime</span></span>|<span data-ttu-id="990df-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="990df-217">DateTimeOffset</span></span>|<span data-ttu-id="990df-218">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="990df-218">The expiration time.</span></span>|
|<span data-ttu-id="990df-219">versionNumber</span><span class="sxs-lookup"><span data-stu-id="990df-219">versionNumber</span></span>|<span data-ttu-id="990df-220">String</span><span class="sxs-lookup"><span data-stu-id="990df-220">String</span></span>|<span data-ttu-id="990df-221">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="990df-221">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="990df-222">buildNumber</span><span class="sxs-lookup"><span data-stu-id="990df-222">buildNumber</span></span>|<span data-ttu-id="990df-223">String</span><span class="sxs-lookup"><span data-stu-id="990df-223">String</span></span>|<span data-ttu-id="990df-224">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="990df-224">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="990df-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="990df-225">Response</span></span>
<span data-ttu-id="990df-226">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="990df-226">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="990df-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="990df-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="990df-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="990df-228">Request</span></span>
<span data-ttu-id="990df-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="990df-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="990df-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="990df-230">Response</span></span>
<span data-ttu-id="990df-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="990df-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



