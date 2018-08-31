# <a name="create-managedandroidlobapp"></a><span data-ttu-id="d82ac-101">Criar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="d82ac-101">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="d82ac-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d82ac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d82ac-103">Cria um novo objeto [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d82ac-103">Create a new [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d82ac-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d82ac-104">Prerequisites</span></span>
<span data-ttu-id="d82ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d82ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d82ac-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d82ac-107">Permission type</span></span>|<span data-ttu-id="d82ac-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d82ac-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d82ac-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d82ac-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d82ac-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d82ac-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d82ac-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d82ac-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d82ac-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d82ac-112">Not supported.</span></span>|
|<span data-ttu-id="d82ac-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d82ac-113">Application</span></span>|<span data-ttu-id="d82ac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d82ac-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d82ac-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d82ac-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d82ac-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d82ac-116">Request headers</span></span>
|<span data-ttu-id="d82ac-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d82ac-117">Header</span></span>|<span data-ttu-id="d82ac-118">Valor</span><span class="sxs-lookup"><span data-stu-id="d82ac-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d82ac-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="d82ac-119">Authorization</span></span>|<span data-ttu-id="d82ac-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="d82ac-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d82ac-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d82ac-121">Accept</span></span>|<span data-ttu-id="d82ac-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="d82ac-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d82ac-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d82ac-123">Request body</span></span>
<span data-ttu-id="d82ac-124">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="d82ac-124">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="d82ac-125">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="d82ac-125">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="d82ac-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d82ac-126">Property</span></span>|<span data-ttu-id="d82ac-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d82ac-127">Type</span></span>|<span data-ttu-id="d82ac-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d82ac-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d82ac-129">id</span><span class="sxs-lookup"><span data-stu-id="d82ac-129">id</span></span>|<span data-ttu-id="d82ac-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-130">String</span></span>|<span data-ttu-id="d82ac-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d82ac-131">Key of the entity.</span></span> <span data-ttu-id="d82ac-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d82ac-133">displayName</span></span>|<span data-ttu-id="d82ac-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-134">String</span></span>|<span data-ttu-id="d82ac-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d82ac-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d82ac-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-137">description</span><span class="sxs-lookup"><span data-stu-id="d82ac-137">description</span></span>|<span data-ttu-id="d82ac-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-138">String</span></span>|<span data-ttu-id="d82ac-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d82ac-139">The description of the app.</span></span> <span data-ttu-id="d82ac-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-141">publisher</span><span class="sxs-lookup"><span data-stu-id="d82ac-141">publisher</span></span>|<span data-ttu-id="d82ac-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-142">String</span></span>|<span data-ttu-id="d82ac-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d82ac-143">The publisher of the app.</span></span> <span data-ttu-id="d82ac-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d82ac-145">largeIcon</span></span>|[<span data-ttu-id="d82ac-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d82ac-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="d82ac-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d82ac-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d82ac-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d82ac-149">createdDateTime</span></span>|<span data-ttu-id="d82ac-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d82ac-150">DateTimeOffset</span></span>|<span data-ttu-id="d82ac-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d82ac-151">The date and time the app was created.</span></span> <span data-ttu-id="d82ac-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d82ac-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d82ac-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d82ac-154">DateTimeOffset</span></span>|<span data-ttu-id="d82ac-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d82ac-155">The date and time the app was last modified.</span></span> <span data-ttu-id="d82ac-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d82ac-157">isFeatured</span></span>|<span data-ttu-id="d82ac-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="d82ac-158">Boolean</span></span>|<span data-ttu-id="d82ac-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d82ac-160">privacyInformationUrl</span></span>|<span data-ttu-id="d82ac-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-161">String</span></span>|<span data-ttu-id="d82ac-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d82ac-162">The privacy statement Url.</span></span> <span data-ttu-id="d82ac-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d82ac-164">informationUrl</span></span>|<span data-ttu-id="d82ac-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-165">String</span></span>|<span data-ttu-id="d82ac-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d82ac-166">The more information Url.</span></span> <span data-ttu-id="d82ac-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-168">owner</span><span class="sxs-lookup"><span data-stu-id="d82ac-168">owner</span></span>|<span data-ttu-id="d82ac-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-169">String</span></span>|<span data-ttu-id="d82ac-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d82ac-170">The owner of the app.</span></span> <span data-ttu-id="d82ac-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-172">developer</span><span class="sxs-lookup"><span data-stu-id="d82ac-172">developer</span></span>|<span data-ttu-id="d82ac-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-173">String</span></span>|<span data-ttu-id="d82ac-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d82ac-174">The developer of the app.</span></span> <span data-ttu-id="d82ac-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-176">Observações</span><span class="sxs-lookup"><span data-stu-id="d82ac-176">notes</span></span>|<span data-ttu-id="d82ac-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-177">String</span></span>|<span data-ttu-id="d82ac-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d82ac-178">Notes for the app.</span></span> <span data-ttu-id="d82ac-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="d82ac-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="d82ac-180">publishingState</span></span>|[<span data-ttu-id="d82ac-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d82ac-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="d82ac-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d82ac-182">The publishing state for the app.</span></span> <span data-ttu-id="d82ac-183">O aplicativo não pode ser atribuído, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d82ac-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d82ac-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d82ac-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="d82ac-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d82ac-185">The possible values are:</span></span>|
|<span data-ttu-id="d82ac-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="d82ac-186">appAvailability</span></span>|[<span data-ttu-id="d82ac-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="d82ac-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="d82ac-188">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d82ac-188">The Application's availability.</span></span> <span data-ttu-id="d82ac-189">Herdado de [managedApp](../resources/intune_apps_managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d82ac-189">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span> <span data-ttu-id="d82ac-190">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="d82ac-190">The possible values are:</span></span>|
|<span data-ttu-id="d82ac-191">version</span><span class="sxs-lookup"><span data-stu-id="d82ac-191">version</span></span>|<span data-ttu-id="d82ac-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-192">String</span></span>|<span data-ttu-id="d82ac-193">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d82ac-193">The Application's version.</span></span> <span data-ttu-id="d82ac-194">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="d82ac-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d82ac-195">committedContentVersion</span></span>|<span data-ttu-id="d82ac-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-196">String</span></span>|<span data-ttu-id="d82ac-197">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="d82ac-197">The internal committed content version.</span></span> <span data-ttu-id="d82ac-198">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d82ac-199">fileName</span><span class="sxs-lookup"><span data-stu-id="d82ac-199">fileName</span></span>|<span data-ttu-id="d82ac-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-200">String</span></span>|<span data-ttu-id="d82ac-201">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="d82ac-201">The name of the main Lob application file.</span></span> <span data-ttu-id="d82ac-202">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d82ac-203">size</span><span class="sxs-lookup"><span data-stu-id="d82ac-203">size</span></span>|<span data-ttu-id="d82ac-204">Int64</span><span class="sxs-lookup"><span data-stu-id="d82ac-204">Int64</span></span>|<span data-ttu-id="d82ac-205">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="d82ac-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="d82ac-206">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d82ac-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d82ac-207">packageId</span><span class="sxs-lookup"><span data-stu-id="d82ac-207">packageId</span></span>|<span data-ttu-id="d82ac-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-208">String</span></span>|<span data-ttu-id="d82ac-209">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="d82ac-209">The package identifier.</span></span>|
|<span data-ttu-id="d82ac-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d82ac-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d82ac-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d82ac-211">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="d82ac-212">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="d82ac-212">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d82ac-213">versionName</span><span class="sxs-lookup"><span data-stu-id="d82ac-213">versionName</span></span>|<span data-ttu-id="d82ac-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-214">String</span></span>|<span data-ttu-id="d82ac-215">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d82ac-215">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d82ac-216">versionCode</span><span class="sxs-lookup"><span data-stu-id="d82ac-216">versionCode</span></span>|<span data-ttu-id="d82ac-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82ac-217">String</span></span>|<span data-ttu-id="d82ac-218">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d82ac-218">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="d82ac-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="d82ac-219">Response</span></span>
<span data-ttu-id="d82ac-220">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d82ac-220">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d82ac-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d82ac-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="d82ac-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d82ac-222">Request</span></span>
<span data-ttu-id="d82ac-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d82ac-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1217

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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

### <a name="response"></a><span data-ttu-id="d82ac-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="d82ac-224">Response</span></span>
<span data-ttu-id="d82ac-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d82ac-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1325

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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



