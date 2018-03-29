# <a name="create-windowsuniversalappx"></a><span data-ttu-id="1bb56-101">Criar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="1bb56-101">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="1bb56-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1bb56-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1bb56-103">Cria um novo objeto [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="1bb56-103">Create a new [plannerBucket](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1bb56-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bb56-104">Prerequisites</span></span>
<span data-ttu-id="1bb56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1bb56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1bb56-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bb56-107">Permission type</span></span>|<span data-ttu-id="1bb56-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1bb56-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bb56-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bb56-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1bb56-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb56-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1bb56-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bb56-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bb56-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bb56-112">Not supported.</span></span>|
|<span data-ttu-id="1bb56-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bb56-113">Application</span></span>|<span data-ttu-id="1bb56-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bb56-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bb56-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bb56-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1bb56-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb56-116">Request headers</span></span>
|<span data-ttu-id="1bb56-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bb56-117">Header</span></span>|<span data-ttu-id="1bb56-118">Valor</span><span class="sxs-lookup"><span data-stu-id="1bb56-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bb56-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bb56-119">Authorization</span></span>|<span data-ttu-id="1bb56-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bb56-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1bb56-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bb56-121">Accept</span></span>|<span data-ttu-id="1bb56-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1bb56-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bb56-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb56-123">Request body</span></span>
<span data-ttu-id="1bb56-124">No corpo da solicitação, forneça uma representação JSON do objeto windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="1bb56-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="1bb56-125">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="1bb56-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="1bb56-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bb56-126">Property</span></span>|<span data-ttu-id="1bb56-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bb56-127">Type</span></span>|<span data-ttu-id="1bb56-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bb56-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bb56-129">id</span><span class="sxs-lookup"><span data-stu-id="1bb56-129">id</span></span>|<span data-ttu-id="1bb56-130">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-130">String</span></span>|<span data-ttu-id="1bb56-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1bb56-131">Key of the setting.</span></span> <span data-ttu-id="1bb56-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1bb56-133">displayName</span></span>|<span data-ttu-id="1bb56-134">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-134">String</span></span>|<span data-ttu-id="1bb56-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1bb56-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1bb56-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-137">descrição</span><span class="sxs-lookup"><span data-stu-id="1bb56-137">description</span></span>|<span data-ttu-id="1bb56-138">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-138">String</span></span>|<span data-ttu-id="1bb56-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb56-139">The description of the app.</span></span> <span data-ttu-id="1bb56-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-141">publicador</span><span class="sxs-lookup"><span data-stu-id="1bb56-141">Publisher</span></span>|<span data-ttu-id="1bb56-142">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-142">String</span></span>|<span data-ttu-id="1bb56-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb56-143">The publisher of the app.</span></span> <span data-ttu-id="1bb56-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1bb56-145">largeIcon</span></span>|[<span data-ttu-id="1bb56-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1bb56-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="1bb56-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="1bb56-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1bb56-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1bb56-149">createdDateTime</span></span>|<span data-ttu-id="1bb56-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bb56-150">DateTimeOffset</span></span>|<span data-ttu-id="1bb56-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb56-151">The date and time the group was created.</span></span> <span data-ttu-id="1bb56-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1bb56-153">lastModifiedDateTime</span></span>|<span data-ttu-id="1bb56-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bb56-154">DateTimeOffset</span></span>|<span data-ttu-id="1bb56-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1bb56-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="1bb56-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1bb56-157">isFeatured</span></span>|<span data-ttu-id="1bb56-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bb56-158">Boolean</span></span>|<span data-ttu-id="1bb56-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1bb56-160">privacyInformationUrl</span></span>|<span data-ttu-id="1bb56-161">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-161">String</span></span>|<span data-ttu-id="1bb56-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="1bb56-162">The privacy statement Url.</span></span> <span data-ttu-id="1bb56-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1bb56-164">informationUrl</span></span>|<span data-ttu-id="1bb56-165">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-165">String</span></span>|<span data-ttu-id="1bb56-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="1bb56-166">The more information Url.</span></span> <span data-ttu-id="1bb56-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-168">owner</span><span class="sxs-lookup"><span data-stu-id="1bb56-168">owner</span></span>|<span data-ttu-id="1bb56-169">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-169">String</span></span>|<span data-ttu-id="1bb56-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1bb56-170">The owner of the app.</span></span> <span data-ttu-id="1bb56-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-172">developer</span><span class="sxs-lookup"><span data-stu-id="1bb56-172">"developer"</span></span>|<span data-ttu-id="1bb56-173">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-173">String</span></span>|<span data-ttu-id="1bb56-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb56-174">The developer of the app.</span></span> <span data-ttu-id="1bb56-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-176">Observações</span><span class="sxs-lookup"><span data-stu-id="1bb56-176">Notes</span></span>|<span data-ttu-id="1bb56-177">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-177">String</span></span>|<span data-ttu-id="1bb56-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb56-178">Notes for the app.</span></span> <span data-ttu-id="1bb56-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1bb56-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="1bb56-180">publishingState</span></span>|<span data-ttu-id="1bb56-181">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-181">String</span></span>|<span data-ttu-id="1bb56-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb56-182">The publishing state for the app.</span></span> <span data-ttu-id="1bb56-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="1bb56-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1bb56-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1bb56-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1bb56-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1bb56-185">committedContentVersion</span></span>|<span data-ttu-id="1bb56-186">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-186">String</span></span>|<span data-ttu-id="1bb56-187">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="1bb56-187">The internal committed content version.</span></span> <span data-ttu-id="1bb56-188">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="1bb56-189">fileName</span><span class="sxs-lookup"><span data-stu-id="1bb56-189">fileName</span></span>|<span data-ttu-id="1bb56-190">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-190">String</span></span>|<span data-ttu-id="1bb56-191">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="1bb56-191">The name of the main Lob application file.</span></span> <span data-ttu-id="1bb56-192">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="1bb56-193">size</span><span class="sxs-lookup"><span data-stu-id="1bb56-193">size</span></span>|<span data-ttu-id="1bb56-194">Int64</span><span class="sxs-lookup"><span data-stu-id="1bb56-194">Int64</span></span>|<span data-ttu-id="1bb56-195">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="1bb56-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="1bb56-196">Herdado de [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb56-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="1bb56-197">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="1bb56-197">applicableArchitectures</span></span>|<span data-ttu-id="1bb56-198">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-198">String</span></span>|<span data-ttu-id="1bb56-199">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="1bb56-199">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="1bb56-200">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="1bb56-200">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="1bb56-201">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="1bb56-201">applicableDeviceTypes</span></span>|<span data-ttu-id="1bb56-202">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-202">String</span></span>|<span data-ttu-id="1bb56-203">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="1bb56-203">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="1bb56-204">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="1bb56-204">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="1bb56-205">identityName</span><span class="sxs-lookup"><span data-stu-id="1bb56-205">identityName</span></span>|<span data-ttu-id="1bb56-206">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-206">String</span></span>|<span data-ttu-id="1bb56-207">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1bb56-207">The Identity Name.</span></span>|
|<span data-ttu-id="1bb56-208">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="1bb56-208">identityPublisherHash</span></span>|<span data-ttu-id="1bb56-209">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-209">String</span></span>|<span data-ttu-id="1bb56-210">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="1bb56-210">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="1bb56-211">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1bb56-211">identityResourceIdentifier</span></span>|<span data-ttu-id="1bb56-212">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-212">String</span></span>|<span data-ttu-id="1bb56-213">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1bb56-213">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="1bb56-214">isBundle</span><span class="sxs-lookup"><span data-stu-id="1bb56-214">isBundle</span></span>|<span data-ttu-id="1bb56-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bb56-215">Boolean</span></span>|<span data-ttu-id="1bb56-216">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="1bb56-216">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="1bb56-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1bb56-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1bb56-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1bb56-218">windowsMinimumOperatingSystem</span></span>](../resources/intune_apps_windowsminimumoperatingsystem.md)|<span data-ttu-id="1bb56-219">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="1bb56-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1bb56-220">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1bb56-220">identityVersion</span></span>|<span data-ttu-id="1bb56-221">String</span><span class="sxs-lookup"><span data-stu-id="1bb56-221">String</span></span>|<span data-ttu-id="1bb56-222">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="1bb56-222">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="1bb56-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bb56-223">Response</span></span>
<span data-ttu-id="1bb56-224">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bb56-224">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bb56-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bb56-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="1bb56-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb56-226">Request</span></span>
<span data-ttu-id="1bb56-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bb56-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1bb56-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bb56-228">Response</span></span>
<span data-ttu-id="1bb56-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bb56-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



