# <a name="create-windowsuniversalappx"></a><span data-ttu-id="c07a2-101">Criar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="c07a2-101">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="c07a2-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c07a2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c07a2-103">Cria um novo objeto [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="c07a2-103">Create a new [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c07a2-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c07a2-104">Prerequisites</span></span>
<span data-ttu-id="c07a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c07a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c07a2-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c07a2-107">Permission type</span></span>|<span data-ttu-id="c07a2-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c07a2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c07a2-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c07a2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c07a2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c07a2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c07a2-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c07a2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c07a2-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c07a2-112">Not supported.</span></span>|
|<span data-ttu-id="c07a2-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c07a2-113">Application</span></span>|<span data-ttu-id="c07a2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c07a2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c07a2-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c07a2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c07a2-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c07a2-116">Request headers</span></span>
|<span data-ttu-id="c07a2-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c07a2-117">Header</span></span>|<span data-ttu-id="c07a2-118">Valor</span><span class="sxs-lookup"><span data-stu-id="c07a2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c07a2-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="c07a2-119">Authorization</span></span>|<span data-ttu-id="c07a2-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="c07a2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c07a2-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c07a2-121">Accept</span></span>|<span data-ttu-id="c07a2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c07a2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c07a2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c07a2-123">Request body</span></span>
<span data-ttu-id="c07a2-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="c07a2-124">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="c07a2-125">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="c07a2-125">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="c07a2-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c07a2-126">Property</span></span>|<span data-ttu-id="c07a2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c07a2-127">Type</span></span>|<span data-ttu-id="c07a2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c07a2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c07a2-129">id</span><span class="sxs-lookup"><span data-stu-id="c07a2-129">id</span></span>|<span data-ttu-id="c07a2-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-130">String</span></span>|<span data-ttu-id="c07a2-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c07a2-131">Key of the entity.</span></span> <span data-ttu-id="c07a2-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c07a2-133">displayName</span></span>|<span data-ttu-id="c07a2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-134">String</span></span>|<span data-ttu-id="c07a2-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c07a2-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c07a2-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-137">description</span><span class="sxs-lookup"><span data-stu-id="c07a2-137">description</span></span>|<span data-ttu-id="c07a2-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-138">String</span></span>|<span data-ttu-id="c07a2-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c07a2-139">The description of the app.</span></span> <span data-ttu-id="c07a2-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-141">publisher</span><span class="sxs-lookup"><span data-stu-id="c07a2-141">publisher</span></span>|<span data-ttu-id="c07a2-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-142">String</span></span>|<span data-ttu-id="c07a2-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c07a2-143">The publisher of the app.</span></span> <span data-ttu-id="c07a2-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c07a2-145">largeIcon</span></span>|[<span data-ttu-id="c07a2-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c07a2-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="c07a2-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="c07a2-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c07a2-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c07a2-149">createdDateTime</span></span>|<span data-ttu-id="c07a2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c07a2-150">DateTimeOffset</span></span>|<span data-ttu-id="c07a2-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c07a2-151">The date and time the app was created.</span></span> <span data-ttu-id="c07a2-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c07a2-153">lastModifiedDateTime</span></span>|<span data-ttu-id="c07a2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c07a2-154">DateTimeOffset</span></span>|<span data-ttu-id="c07a2-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c07a2-155">The date and time the app was last modified.</span></span> <span data-ttu-id="c07a2-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c07a2-157">isFeatured</span></span>|<span data-ttu-id="c07a2-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="c07a2-158">Boolean</span></span>|<span data-ttu-id="c07a2-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c07a2-160">privacyInformationUrl</span></span>|<span data-ttu-id="c07a2-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-161">String</span></span>|<span data-ttu-id="c07a2-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c07a2-162">The privacy statement Url.</span></span> <span data-ttu-id="c07a2-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c07a2-164">informationUrl</span></span>|<span data-ttu-id="c07a2-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-165">String</span></span>|<span data-ttu-id="c07a2-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c07a2-166">The more information Url.</span></span> <span data-ttu-id="c07a2-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-168">owner</span><span class="sxs-lookup"><span data-stu-id="c07a2-168">owner</span></span>|<span data-ttu-id="c07a2-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-169">String</span></span>|<span data-ttu-id="c07a2-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c07a2-170">The owner of the app.</span></span> <span data-ttu-id="c07a2-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-172">developer</span><span class="sxs-lookup"><span data-stu-id="c07a2-172">developer</span></span>|<span data-ttu-id="c07a2-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-173">String</span></span>|<span data-ttu-id="c07a2-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c07a2-174">The developer of the app.</span></span> <span data-ttu-id="c07a2-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-176">Observações</span><span class="sxs-lookup"><span data-stu-id="c07a2-176">notes</span></span>|<span data-ttu-id="c07a2-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-177">String</span></span>|<span data-ttu-id="c07a2-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c07a2-178">Notes for the app.</span></span> <span data-ttu-id="c07a2-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="c07a2-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="c07a2-180">publishingState</span></span>|[<span data-ttu-id="c07a2-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c07a2-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="c07a2-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c07a2-182">The publishing state for the app.</span></span> <span data-ttu-id="c07a2-183">O aplicativo não pode ser atribuído, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="c07a2-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c07a2-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c07a2-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="c07a2-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c07a2-185">The possible values are:</span></span>|
|<span data-ttu-id="c07a2-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c07a2-186">committedContentVersion</span></span>|<span data-ttu-id="c07a2-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-187">String</span></span>|<span data-ttu-id="c07a2-188">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="c07a2-188">The internal committed content version.</span></span> <span data-ttu-id="c07a2-189">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="c07a2-190">fileName</span><span class="sxs-lookup"><span data-stu-id="c07a2-190">fileName</span></span>|<span data-ttu-id="c07a2-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-191">String</span></span>|<span data-ttu-id="c07a2-192">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="c07a2-192">The name of the main Lob application file.</span></span> <span data-ttu-id="c07a2-193">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="c07a2-194">size</span><span class="sxs-lookup"><span data-stu-id="c07a2-194">size</span></span>|<span data-ttu-id="c07a2-195">Int64</span><span class="sxs-lookup"><span data-stu-id="c07a2-195">Int64</span></span>|<span data-ttu-id="c07a2-196">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="c07a2-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="c07a2-197">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c07a2-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="c07a2-198">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="c07a2-198">applicableArchitectures</span></span>|[<span data-ttu-id="c07a2-199">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="c07a2-199">windowsArchitecture</span></span>](../resources/intune_apps_windowsarchitecture.md)|<span data-ttu-id="c07a2-200">A(s) arquitetura(s) do Windows na(s) qual(is) este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="c07a2-200">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="c07a2-201">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="c07a2-201">The possible values are `none`, `x86`, `x64`, `arm`, `neutral`, , , , , , , or .</span></span>|
|<span data-ttu-id="c07a2-202">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="c07a2-202">applicableDeviceTypes</span></span>|[<span data-ttu-id="c07a2-203">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="c07a2-203">windowsDeviceType</span></span>](../resources/intune_apps_windowsdevicetype.md)|<span data-ttu-id="c07a2-204">O(s) tipo(s) de dispositivo(s) Windows no(s) qual(is) este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="c07a2-204">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="c07a2-205">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="c07a2-205">The possible values are `none`, `desktop`, `mobile`, `holographic`, `team`, , , , , , , or .</span></span>|
|<span data-ttu-id="c07a2-206">identityName</span><span class="sxs-lookup"><span data-stu-id="c07a2-206">identityName</span></span>|<span data-ttu-id="c07a2-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-207">String</span></span>|<span data-ttu-id="c07a2-208">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="c07a2-208">The Identity Name.</span></span>|
|<span data-ttu-id="c07a2-209">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="c07a2-209">identityPublisherHash</span></span>|<span data-ttu-id="c07a2-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-210">String</span></span>|<span data-ttu-id="c07a2-211">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="c07a2-211">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="c07a2-212">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c07a2-212">identityResourceIdentifier</span></span>|<span data-ttu-id="c07a2-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-213">String</span></span>|<span data-ttu-id="c07a2-214">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="c07a2-214">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="c07a2-215">isBundle</span><span class="sxs-lookup"><span data-stu-id="c07a2-215">isBundle</span></span>|<span data-ttu-id="c07a2-216">Booleano</span><span class="sxs-lookup"><span data-stu-id="c07a2-216">Boolean</span></span>|<span data-ttu-id="c07a2-217">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="c07a2-217">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="c07a2-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c07a2-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c07a2-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c07a2-219">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="c07a2-220">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="c07a2-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c07a2-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="c07a2-221">identityVersion</span></span>|<span data-ttu-id="c07a2-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07a2-222">String</span></span>|<span data-ttu-id="c07a2-223">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="c07a2-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="c07a2-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="c07a2-224">Response</span></span>
<span data-ttu-id="c07a2-225">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c07a2-225">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c07a2-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c07a2-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="c07a2-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c07a2-227">Request</span></span>
<span data-ttu-id="c07a2-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c07a2-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1253

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

### <a name="response"></a><span data-ttu-id="c07a2-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="c07a2-229">Response</span></span>
<span data-ttu-id="c07a2-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c07a2-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



