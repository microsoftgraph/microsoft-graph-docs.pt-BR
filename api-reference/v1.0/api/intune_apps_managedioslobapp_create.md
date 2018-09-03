# <a name="create-managedioslobapp"></a><span data-ttu-id="b6e42-101">Criar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="b6e42-101">Create managedIOSLobApp</span></span>

> <span data-ttu-id="b6e42-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b6e42-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6e42-103">Cria um novo objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6e42-103">Create a new [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6e42-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6e42-104">Prerequisites</span></span>
<span data-ttu-id="b6e42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b6e42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b6e42-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6e42-107">Permission type</span></span>|<span data-ttu-id="b6e42-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6e42-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6e42-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6e42-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b6e42-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6e42-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b6e42-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6e42-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6e42-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6e42-112">Not supported.</span></span>|
|<span data-ttu-id="b6e42-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6e42-113">Application</span></span>|<span data-ttu-id="b6e42-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6e42-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6e42-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6e42-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b6e42-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e42-116">Request headers</span></span>
|<span data-ttu-id="b6e42-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6e42-117">Header</span></span>|<span data-ttu-id="b6e42-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b6e42-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6e42-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6e42-119">Authorization</span></span>|<span data-ttu-id="b6e42-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="b6e42-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6e42-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6e42-121">Accept</span></span>|<span data-ttu-id="b6e42-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b6e42-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6e42-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e42-123">Request body</span></span>
<span data-ttu-id="b6e42-124">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="b6e42-124">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="b6e42-125">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="b6e42-125">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="b6e42-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6e42-126">Property</span></span>|<span data-ttu-id="b6e42-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6e42-127">Type</span></span>|<span data-ttu-id="b6e42-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6e42-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6e42-129">id</span><span class="sxs-lookup"><span data-stu-id="b6e42-129">id</span></span>|<span data-ttu-id="b6e42-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-130">String</span></span>|<span data-ttu-id="b6e42-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b6e42-131">Key of the entity.</span></span> <span data-ttu-id="b6e42-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b6e42-133">displayName</span></span>|<span data-ttu-id="b6e42-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-134">String</span></span>|<span data-ttu-id="b6e42-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b6e42-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b6e42-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-137">description</span><span class="sxs-lookup"><span data-stu-id="b6e42-137">description</span></span>|<span data-ttu-id="b6e42-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-138">String</span></span>|<span data-ttu-id="b6e42-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6e42-139">The description of the app.</span></span> <span data-ttu-id="b6e42-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-141">publisher</span><span class="sxs-lookup"><span data-stu-id="b6e42-141">publisher</span></span>|<span data-ttu-id="b6e42-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-142">String</span></span>|<span data-ttu-id="b6e42-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6e42-143">The publisher of the app.</span></span> <span data-ttu-id="b6e42-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b6e42-145">largeIcon</span></span>|[<span data-ttu-id="b6e42-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b6e42-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="b6e42-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b6e42-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b6e42-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6e42-149">createdDateTime</span></span>|<span data-ttu-id="b6e42-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6e42-150">DateTimeOffset</span></span>|<span data-ttu-id="b6e42-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6e42-151">The date and time the app was created.</span></span> <span data-ttu-id="b6e42-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6e42-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b6e42-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6e42-154">DateTimeOffset</span></span>|<span data-ttu-id="b6e42-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b6e42-155">The date and time the app was last modified.</span></span> <span data-ttu-id="b6e42-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b6e42-157">isFeatured</span></span>|<span data-ttu-id="b6e42-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="b6e42-158">Boolean</span></span>|<span data-ttu-id="b6e42-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b6e42-160">privacyInformationUrl</span></span>|<span data-ttu-id="b6e42-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-161">String</span></span>|<span data-ttu-id="b6e42-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b6e42-162">The privacy statement Url.</span></span> <span data-ttu-id="b6e42-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b6e42-164">informationUrl</span></span>|<span data-ttu-id="b6e42-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-165">String</span></span>|<span data-ttu-id="b6e42-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b6e42-166">The more information Url.</span></span> <span data-ttu-id="b6e42-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-168">owner</span><span class="sxs-lookup"><span data-stu-id="b6e42-168">owner</span></span>|<span data-ttu-id="b6e42-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-169">String</span></span>|<span data-ttu-id="b6e42-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b6e42-170">The owner of the app.</span></span> <span data-ttu-id="b6e42-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-172">developer</span><span class="sxs-lookup"><span data-stu-id="b6e42-172">developer</span></span>|<span data-ttu-id="b6e42-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-173">String</span></span>|<span data-ttu-id="b6e42-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6e42-174">The developer of the app.</span></span> <span data-ttu-id="b6e42-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-176">Observações</span><span class="sxs-lookup"><span data-stu-id="b6e42-176">notes</span></span>|<span data-ttu-id="b6e42-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-177">String</span></span>|<span data-ttu-id="b6e42-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6e42-178">Notes for the app.</span></span> <span data-ttu-id="b6e42-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b6e42-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="b6e42-180">publishingState</span></span>|[<span data-ttu-id="b6e42-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b6e42-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="b6e42-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6e42-182">The publishing state for the app.</span></span> <span data-ttu-id="b6e42-183">O aplicativo não pode ser atribuído, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b6e42-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b6e42-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6e42-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="b6e42-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b6e42-185">The possible values are:</span></span>|
|<span data-ttu-id="b6e42-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="b6e42-186">appAvailability</span></span>|[<span data-ttu-id="b6e42-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="b6e42-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="b6e42-188">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6e42-188">The Application's availability.</span></span> <span data-ttu-id="b6e42-189">Herdado de [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6e42-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="b6e42-190">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="b6e42-190">The possible values are:</span></span>|
|<span data-ttu-id="b6e42-191">version</span><span class="sxs-lookup"><span data-stu-id="b6e42-191">version</span></span>|<span data-ttu-id="b6e42-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-192">String</span></span>|<span data-ttu-id="b6e42-193">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6e42-193">The Application's version.</span></span> <span data-ttu-id="b6e42-194">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="b6e42-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b6e42-195">committedContentVersion</span></span>|<span data-ttu-id="b6e42-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-196">String</span></span>|<span data-ttu-id="b6e42-197">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="b6e42-197">The internal committed content version.</span></span> <span data-ttu-id="b6e42-198">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="b6e42-199">fileName</span><span class="sxs-lookup"><span data-stu-id="b6e42-199">fileName</span></span>|<span data-ttu-id="b6e42-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-200">String</span></span>|<span data-ttu-id="b6e42-201">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="b6e42-201">The name of the main Lob application file.</span></span> <span data-ttu-id="b6e42-202">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="b6e42-203">size</span><span class="sxs-lookup"><span data-stu-id="b6e42-203">size</span></span>|<span data-ttu-id="b6e42-204">Int64</span><span class="sxs-lookup"><span data-stu-id="b6e42-204">Int64</span></span>|<span data-ttu-id="b6e42-205">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="b6e42-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="b6e42-206">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6e42-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="b6e42-207">bundleId</span><span class="sxs-lookup"><span data-stu-id="b6e42-207">bundleId</span></span>|<span data-ttu-id="b6e42-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-208">String</span></span>|<span data-ttu-id="b6e42-209">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b6e42-209">The Identity Name.</span></span>|
|<span data-ttu-id="b6e42-210">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="b6e42-210">applicableDeviceType</span></span>|[<span data-ttu-id="b6e42-211">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b6e42-211">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="b6e42-212">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="b6e42-212">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="b6e42-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b6e42-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b6e42-214">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b6e42-214">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="b6e42-215">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="b6e42-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b6e42-216">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b6e42-216">expirationDateTime</span></span>|<span data-ttu-id="b6e42-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6e42-217">DateTimeOffset</span></span>|<span data-ttu-id="b6e42-218">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="b6e42-218">The expiration time.</span></span>|
|<span data-ttu-id="b6e42-219">versionNumber</span><span class="sxs-lookup"><span data-stu-id="b6e42-219">versionNumber</span></span>|<span data-ttu-id="b6e42-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-220">String</span></span>|<span data-ttu-id="b6e42-221">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b6e42-221">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b6e42-222">buildNumber</span><span class="sxs-lookup"><span data-stu-id="b6e42-222">buildNumber</span></span>|<span data-ttu-id="b6e42-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6e42-223">String</span></span>|<span data-ttu-id="b6e42-224">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b6e42-224">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="b6e42-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6e42-225">Response</span></span>
<span data-ttu-id="b6e42-226">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6e42-226">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6e42-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6e42-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6e42-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6e42-228">Request</span></span>
<span data-ttu-id="b6e42-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6e42-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1331

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
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="b6e42-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6e42-230">Response</span></span>
<span data-ttu-id="b6e42-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6e42-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1439

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
    "v11_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



