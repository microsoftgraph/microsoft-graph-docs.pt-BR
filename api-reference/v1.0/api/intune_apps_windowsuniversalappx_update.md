# <a name="update-windowsuniversalappx"></a><span data-ttu-id="658dc-101">Atualizar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="658dc-101">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="658dc-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="658dc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="658dc-103">Atualiza as propriedades de um objeto [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="658dc-103">Update the properties of a [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="658dc-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="658dc-104">Prerequisites</span></span>
<span data-ttu-id="658dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="658dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="658dc-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="658dc-107">Permission type</span></span>|<span data-ttu-id="658dc-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="658dc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="658dc-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="658dc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="658dc-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="658dc-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="658dc-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="658dc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="658dc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="658dc-112">Not supported.</span></span>|
|<span data-ttu-id="658dc-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="658dc-113">Application</span></span>|<span data-ttu-id="658dc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="658dc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="658dc-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="658dc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="658dc-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="658dc-116">Request headers</span></span>
|<span data-ttu-id="658dc-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="658dc-117">Header</span></span>|<span data-ttu-id="658dc-118">Valor</span><span class="sxs-lookup"><span data-stu-id="658dc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="658dc-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="658dc-119">Authorization</span></span>|<span data-ttu-id="658dc-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="658dc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="658dc-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="658dc-121">Accept</span></span>|<span data-ttu-id="658dc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="658dc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="658dc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="658dc-123">Request body</span></span>
<span data-ttu-id="658dc-124">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="658dc-124">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="658dc-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="658dc-125">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span></span>

|<span data-ttu-id="658dc-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="658dc-126">Property</span></span>|<span data-ttu-id="658dc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="658dc-127">Type</span></span>|<span data-ttu-id="658dc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="658dc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="658dc-129">id</span><span class="sxs-lookup"><span data-stu-id="658dc-129">id</span></span>|<span data-ttu-id="658dc-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-130">String</span></span>|<span data-ttu-id="658dc-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="658dc-131">Key of the entity.</span></span> <span data-ttu-id="658dc-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-133">displayName</span><span class="sxs-lookup"><span data-stu-id="658dc-133">displayName</span></span>|<span data-ttu-id="658dc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-134">String</span></span>|<span data-ttu-id="658dc-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="658dc-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="658dc-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-137">description</span><span class="sxs-lookup"><span data-stu-id="658dc-137">description</span></span>|<span data-ttu-id="658dc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-138">String</span></span>|<span data-ttu-id="658dc-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="658dc-139">The description of the app.</span></span> <span data-ttu-id="658dc-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-141">publisher</span><span class="sxs-lookup"><span data-stu-id="658dc-141">publisher</span></span>|<span data-ttu-id="658dc-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-142">String</span></span>|<span data-ttu-id="658dc-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="658dc-143">The publisher of the app.</span></span> <span data-ttu-id="658dc-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="658dc-145">largeIcon</span></span>|[<span data-ttu-id="658dc-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="658dc-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="658dc-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="658dc-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="658dc-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="658dc-149">createdDateTime</span></span>|<span data-ttu-id="658dc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="658dc-150">DateTimeOffset</span></span>|<span data-ttu-id="658dc-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="658dc-151">The date and time the app was created.</span></span> <span data-ttu-id="658dc-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="658dc-153">lastModifiedDateTime</span></span>|<span data-ttu-id="658dc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="658dc-154">DateTimeOffset</span></span>|<span data-ttu-id="658dc-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="658dc-155">The date and time the app was last modified.</span></span> <span data-ttu-id="658dc-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="658dc-157">isFeatured</span></span>|<span data-ttu-id="658dc-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="658dc-158">Boolean</span></span>|<span data-ttu-id="658dc-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="658dc-160">privacyInformationUrl</span></span>|<span data-ttu-id="658dc-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-161">String</span></span>|<span data-ttu-id="658dc-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="658dc-162">The privacy statement Url.</span></span> <span data-ttu-id="658dc-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="658dc-164">informationUrl</span></span>|<span data-ttu-id="658dc-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-165">String</span></span>|<span data-ttu-id="658dc-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="658dc-166">The more information Url.</span></span> <span data-ttu-id="658dc-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-168">owner</span><span class="sxs-lookup"><span data-stu-id="658dc-168">owner</span></span>|<span data-ttu-id="658dc-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-169">String</span></span>|<span data-ttu-id="658dc-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="658dc-170">The owner of the app.</span></span> <span data-ttu-id="658dc-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-172">developer</span><span class="sxs-lookup"><span data-stu-id="658dc-172">developer</span></span>|<span data-ttu-id="658dc-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-173">String</span></span>|<span data-ttu-id="658dc-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="658dc-174">The developer of the app.</span></span> <span data-ttu-id="658dc-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-176">Observações</span><span class="sxs-lookup"><span data-stu-id="658dc-176">notes</span></span>|<span data-ttu-id="658dc-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-177">String</span></span>|<span data-ttu-id="658dc-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="658dc-178">Notes for the app.</span></span> <span data-ttu-id="658dc-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="658dc-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="658dc-180">publishingState</span></span>|[<span data-ttu-id="658dc-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="658dc-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="658dc-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="658dc-182">The publishing state for the app.</span></span> <span data-ttu-id="658dc-183">O aplicativo não pode ser atribuído, a menos que seja publicado.</span><span class="sxs-lookup"><span data-stu-id="658dc-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="658dc-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658dc-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="658dc-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="658dc-185">The possible values are:</span></span>|
|<span data-ttu-id="658dc-186">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="658dc-186">committedContentVersion</span></span>|<span data-ttu-id="658dc-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-187">String</span></span>|<span data-ttu-id="658dc-188">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="658dc-188">The internal committed content version.</span></span> <span data-ttu-id="658dc-189">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-189">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="658dc-190">fileName</span><span class="sxs-lookup"><span data-stu-id="658dc-190">fileName</span></span>|<span data-ttu-id="658dc-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-191">String</span></span>|<span data-ttu-id="658dc-192">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="658dc-192">The name of the main Lob application file.</span></span> <span data-ttu-id="658dc-193">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-193">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="658dc-194">size</span><span class="sxs-lookup"><span data-stu-id="658dc-194">size</span></span>|<span data-ttu-id="658dc-195">Int64</span><span class="sxs-lookup"><span data-stu-id="658dc-195">Int64</span></span>|<span data-ttu-id="658dc-196">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="658dc-196">The total size, including all uploaded files.</span></span> <span data-ttu-id="658dc-197">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="658dc-197">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="658dc-198">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="658dc-198">applicableArchitectures</span></span>|[<span data-ttu-id="658dc-199">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="658dc-199">windowsArchitecture</span></span>](../resources/intune_apps_windowsarchitecture.md)|<span data-ttu-id="658dc-200">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="658dc-200">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="658dc-201">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="658dc-201">The possible values are `none`, `x86`, `x64`, `arm`, `neutral`, , , , , , , or .</span></span>|
|<span data-ttu-id="658dc-202">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="658dc-202">applicableDeviceTypes</span></span>|[<span data-ttu-id="658dc-203">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="658dc-203">windowsDeviceType</span></span>](../resources/intune_apps_windowsdevicetype.md)|<span data-ttu-id="658dc-204">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="658dc-204">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="658dc-205">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="658dc-205">The possible values are `none`, `desktop`, `mobile`, `holographic`, `team`, , , , , , , or .</span></span>|
|<span data-ttu-id="658dc-206">identityName</span><span class="sxs-lookup"><span data-stu-id="658dc-206">identityName</span></span>|<span data-ttu-id="658dc-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-207">String</span></span>|<span data-ttu-id="658dc-208">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="658dc-208">The Identity Name.</span></span>|
|<span data-ttu-id="658dc-209">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="658dc-209">identityPublisherHash</span></span>|<span data-ttu-id="658dc-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-210">String</span></span>|<span data-ttu-id="658dc-211">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="658dc-211">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="658dc-212">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="658dc-212">identityResourceIdentifier</span></span>|<span data-ttu-id="658dc-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-213">String</span></span>|<span data-ttu-id="658dc-214">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="658dc-214">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="658dc-215">isBundle</span><span class="sxs-lookup"><span data-stu-id="658dc-215">isBundle</span></span>|<span data-ttu-id="658dc-216">Booleano</span><span class="sxs-lookup"><span data-stu-id="658dc-216">Boolean</span></span>|<span data-ttu-id="658dc-217">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="658dc-217">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="658dc-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="658dc-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="658dc-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="658dc-219">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="658dc-220">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="658dc-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="658dc-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="658dc-221">identityVersion</span></span>|<span data-ttu-id="658dc-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="658dc-222">String</span></span>|<span data-ttu-id="658dc-223">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="658dc-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="658dc-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="658dc-224">Response</span></span>
<span data-ttu-id="658dc-225">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="658dc-225">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="658dc-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="658dc-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="658dc-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="658dc-227">Request</span></span>
<span data-ttu-id="658dc-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="658dc-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1194

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

### <a name="response"></a><span data-ttu-id="658dc-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="658dc-229">Response</span></span>
<span data-ttu-id="658dc-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="658dc-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



