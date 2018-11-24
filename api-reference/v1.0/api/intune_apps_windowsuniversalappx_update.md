# <a name="update-windowsuniversalappx"></a><span data-ttu-id="6031a-101">Atualizar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="6031a-101">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="6031a-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6031a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6031a-103">Atualiza as propriedades de um objeto [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="6031a-103">Update the properties of a [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6031a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6031a-104">Prerequisites</span></span>
<span data-ttu-id="6031a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6031a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6031a-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6031a-107">Permission type</span></span>|<span data-ttu-id="6031a-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6031a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6031a-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6031a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6031a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6031a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6031a-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6031a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6031a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6031a-112">Not supported.</span></span>|
|<span data-ttu-id="6031a-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6031a-113">Application</span></span>|<span data-ttu-id="6031a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6031a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6031a-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6031a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="6031a-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6031a-116">Request headers</span></span>
|<span data-ttu-id="6031a-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6031a-117">Header</span></span>|<span data-ttu-id="6031a-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6031a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6031a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6031a-119">Authorization</span></span>|<span data-ttu-id="6031a-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6031a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6031a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6031a-121">Accept</span></span>|<span data-ttu-id="6031a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6031a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6031a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6031a-123">Request body</span></span>
<span data-ttu-id="6031a-124">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="6031a-124">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="6031a-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="6031a-125">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span></span>

|<span data-ttu-id="6031a-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6031a-126">Property</span></span>|<span data-ttu-id="6031a-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6031a-127">Type</span></span>|<span data-ttu-id="6031a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6031a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6031a-129">id</span><span class="sxs-lookup"><span data-stu-id="6031a-129">id</span></span>|<span data-ttu-id="6031a-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6031a-130">String</span></span>|<span data-ttu-id="6031a-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6031a-131">Key of the entity.</span></span> <span data-ttu-id="6031a-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6031a-133">displayName</span></span>|<span data-ttu-id="6031a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6031a-134">String</span></span>|<span data-ttu-id="6031a-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6031a-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6031a-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-137">description</span><span class="sxs-lookup"><span data-stu-id="6031a-137">description</span></span>|<span data-ttu-id="6031a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6031a-138">String</span></span>|<span data-ttu-id="6031a-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6031a-139">The description of the app.</span></span> <span data-ttu-id="6031a-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-141">publisher</span><span class="sxs-lookup"><span data-stu-id="6031a-141">publisher</span></span>|<span data-ttu-id="6031a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6031a-142">String</span></span>|<span data-ttu-id="6031a-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6031a-143">The publisher of the app.</span></span> <span data-ttu-id="6031a-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6031a-145">largeIcon</span></span>|[<span data-ttu-id="6031a-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6031a-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="6031a-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6031a-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6031a-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6031a-149">createdDateTime</span></span>|<span data-ttu-id="6031a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6031a-150">DateTimeOffset</span></span>|<span data-ttu-id="6031a-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6031a-151">The date and time the app was created.</span></span> <span data-ttu-id="6031a-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6031a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="6031a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6031a-154">DateTimeOffset</span></span>|<span data-ttu-id="6031a-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6031a-155">The date and time the app was last modified.</span></span> <span data-ttu-id="6031a-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6031a-157">isFeatured</span></span>|<span data-ttu-id="6031a-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="6031a-158">Boolean</span></span>|<span data-ttu-id="6031a-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6031a-160">privacyInformationUrl</span></span>|<span data-ttu-id="6031a-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6031a-161">String</span></span>|<span data-ttu-id="6031a-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6031a-162">The privacy statement Url.</span></span> <span data-ttu-id="6031a-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6031a-164">informationUrl</span></span>|<span data-ttu-id="6031a-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6031a-165">String</span></span>|<span data-ttu-id="6031a-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6031a-166">The more information Url.</span></span> <span data-ttu-id="6031a-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-168">owner</span><span class="sxs-lookup"><span data-stu-id="6031a-168">owner</span></span>|<span data-ttu-id="6031a-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6031a-169">String</span></span>|<span data-ttu-id="6031a-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6031a-170">The owner of the app.</span></span> <span data-ttu-id="6031a-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-172">developer</span><span class="sxs-lookup"><span data-stu-id="6031a-172">developer</span></span>|<span data-ttu-id="6031a-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6031a-173">String</span></span>|<span data-ttu-id="6031a-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6031a-174">The developer of the app.</span></span> <span data-ttu-id="6031a-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-176">notes</span><span class="sxs-lookup"><span data-stu-id="6031a-176">notes</span></span>|<span data-ttu-id="6031a-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6031a-177">String</span></span>|<span data-ttu-id="6031a-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6031a-178">Notes for the app.</span></span> <span data-ttu-id="6031a-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6031a-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="6031a-180">publishingState</span></span>|[<span data-ttu-id="6031a-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6031a-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="6031a-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6031a-182">The publishing state for the app.</span></span> <span data-ttu-id="6031a-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6031a-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6031a-184">Herdada do [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6031a-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="6031a-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6031a-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6031a-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="6031a-186">committedContentVersion</span></span>|<span data-ttu-id="6031a-187">String</span><span class="sxs-lookup"><span data-stu-id="6031a-187">String</span></span>|<span data-ttu-id="6031a-188">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="6031a-188">The internal committed content version.</span></span> <span data-ttu-id="6031a-189">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="6031a-190">fileName</span><span class="sxs-lookup"><span data-stu-id="6031a-190">fileName</span></span>|<span data-ttu-id="6031a-191">String</span><span class="sxs-lookup"><span data-stu-id="6031a-191">String</span></span>|<span data-ttu-id="6031a-192">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="6031a-192">The name of the main Lob application file.</span></span> <span data-ttu-id="6031a-193">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="6031a-194">size</span><span class="sxs-lookup"><span data-stu-id="6031a-194">size</span></span>|<span data-ttu-id="6031a-195">Int64</span><span class="sxs-lookup"><span data-stu-id="6031a-195">Int64</span></span>|<span data-ttu-id="6031a-196">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="6031a-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="6031a-197">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6031a-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="6031a-198">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="6031a-198">applicableArchitectures</span></span>|[<span data-ttu-id="6031a-199">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="6031a-199">windowsArchitecture</span></span>](../resources/intune_apps_windowsarchitecture.md)|<span data-ttu-id="6031a-200">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="6031a-200">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="6031a-201">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="6031a-201">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="6031a-202">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="6031a-202">applicableDeviceTypes</span></span>|[<span data-ttu-id="6031a-203">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="6031a-203">windowsDeviceType</span></span>](../resources/intune_apps_windowsdevicetype.md)|<span data-ttu-id="6031a-204">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="6031a-204">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="6031a-205">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="6031a-205">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="6031a-206">identityName</span><span class="sxs-lookup"><span data-stu-id="6031a-206">identityName</span></span>|<span data-ttu-id="6031a-207">String</span><span class="sxs-lookup"><span data-stu-id="6031a-207">String</span></span>|<span data-ttu-id="6031a-208">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6031a-208">The Identity Name.</span></span>|
|<span data-ttu-id="6031a-209">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="6031a-209">identityPublisherHash</span></span>|<span data-ttu-id="6031a-210">String</span><span class="sxs-lookup"><span data-stu-id="6031a-210">String</span></span>|<span data-ttu-id="6031a-211">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="6031a-211">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="6031a-212">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6031a-212">identityResourceIdentifier</span></span>|<span data-ttu-id="6031a-213">String</span><span class="sxs-lookup"><span data-stu-id="6031a-213">String</span></span>|<span data-ttu-id="6031a-214">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6031a-214">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="6031a-215">isBundle</span><span class="sxs-lookup"><span data-stu-id="6031a-215">isBundle</span></span>|<span data-ttu-id="6031a-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="6031a-216">Boolean</span></span>|<span data-ttu-id="6031a-217">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="6031a-217">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="6031a-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6031a-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6031a-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6031a-219">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="6031a-220">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="6031a-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="6031a-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="6031a-221">identityVersion</span></span>|<span data-ttu-id="6031a-222">String</span><span class="sxs-lookup"><span data-stu-id="6031a-222">String</span></span>|<span data-ttu-id="6031a-223">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="6031a-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="6031a-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="6031a-224">Response</span></span>
<span data-ttu-id="6031a-225">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6031a-225">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6031a-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6031a-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="6031a-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6031a-227">Request</span></span>
<span data-ttu-id="6031a-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6031a-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="6031a-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="6031a-229">Response</span></span>
<span data-ttu-id="6031a-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6031a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```



