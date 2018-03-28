# <a name="update-managedandroidlobapp"></a><span data-ttu-id="3b3bd-101">Atualizar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="3b3bd-101">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="3b3bd-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b3bd-103">Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b3bd-103">Update the properties of a [calendar](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b3bd-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b3bd-104">Prerequisites</span></span>
<span data-ttu-id="3b3bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3b3bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3b3bd-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b3bd-107">Permission type</span></span>|<span data-ttu-id="3b3bd-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b3bd-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3b3bd-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b3bd-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b3bd-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b3bd-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-112">Not supported.</span></span>|
|<span data-ttu-id="3b3bd-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b3bd-113">Application</span></span>|<span data-ttu-id="3b3bd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b3bd-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b3bd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="3b3bd-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3bd-116">Request headers</span></span>
|<span data-ttu-id="3b3bd-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b3bd-117">Header</span></span>|<span data-ttu-id="3b3bd-118">Valor</span><span class="sxs-lookup"><span data-stu-id="3b3bd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b3bd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b3bd-119">Authorization</span></span>|<span data-ttu-id="3b3bd-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3b3bd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3b3bd-121">Accept</span></span>|<span data-ttu-id="3b3bd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3b3bd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b3bd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3bd-123">Request body</span></span>
<span data-ttu-id="3b3bd-124">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b3bd-124">In the request body, supply a JSON representation of [message](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="3b3bd-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b3bd-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="3b3bd-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b3bd-126">Property</span></span>|<span data-ttu-id="3b3bd-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b3bd-127">Type</span></span>|<span data-ttu-id="3b3bd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b3bd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b3bd-129">id</span><span class="sxs-lookup"><span data-stu-id="3b3bd-129">id</span></span>|<span data-ttu-id="3b3bd-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-130">String</span></span>|<span data-ttu-id="3b3bd-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-131">Key of the setting.</span></span> <span data-ttu-id="3b3bd-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3b3bd-133">displayName</span></span>|<span data-ttu-id="3b3bd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-134">String</span></span>|<span data-ttu-id="3b3bd-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3b3bd-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-137">description</span><span class="sxs-lookup"><span data-stu-id="3b3bd-137">description</span></span>|<span data-ttu-id="3b3bd-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-138">String</span></span>|<span data-ttu-id="3b3bd-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-139">The description of the app.</span></span> <span data-ttu-id="3b3bd-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-141">publisher</span><span class="sxs-lookup"><span data-stu-id="3b3bd-141">Publisher</span></span>|<span data-ttu-id="3b3bd-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-142">String</span></span>|<span data-ttu-id="3b3bd-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-143">The publisher of the app.</span></span> <span data-ttu-id="3b3bd-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3b3bd-145">largeIcon</span></span>|[<span data-ttu-id="3b3bd-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3b3bd-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="3b3bd-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3b3bd-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b3bd-149">createdDateTime</span></span>|<span data-ttu-id="3b3bd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b3bd-150">DateTimeOffset</span></span>|<span data-ttu-id="3b3bd-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-151">The date and time the group was created.</span></span> <span data-ttu-id="3b3bd-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b3bd-153">lastModifiedDateTime</span></span>|<span data-ttu-id="3b3bd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b3bd-154">DateTimeOffset</span></span>|<span data-ttu-id="3b3bd-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="3b3bd-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3b3bd-157">isFeatured</span></span>|<span data-ttu-id="3b3bd-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b3bd-158">Boolean</span></span>|<span data-ttu-id="3b3bd-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3b3bd-160">privacyInformationUrl</span></span>|<span data-ttu-id="3b3bd-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-161">String</span></span>|<span data-ttu-id="3b3bd-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-162">The privacy statement Url.</span></span> <span data-ttu-id="3b3bd-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3b3bd-164">informationUrl</span></span>|<span data-ttu-id="3b3bd-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-165">String</span></span>|<span data-ttu-id="3b3bd-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-166">The more information Url.</span></span> <span data-ttu-id="3b3bd-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-168">owner</span><span class="sxs-lookup"><span data-stu-id="3b3bd-168">owner</span></span>|<span data-ttu-id="3b3bd-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-169">String</span></span>|<span data-ttu-id="3b3bd-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-170">The owner of the app.</span></span> <span data-ttu-id="3b3bd-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-172">developer</span><span class="sxs-lookup"><span data-stu-id="3b3bd-172">"developer"</span></span>|<span data-ttu-id="3b3bd-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-173">String</span></span>|<span data-ttu-id="3b3bd-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-174">The developer of the app.</span></span> <span data-ttu-id="3b3bd-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-176">notes</span><span class="sxs-lookup"><span data-stu-id="3b3bd-176">Notes</span></span>|<span data-ttu-id="3b3bd-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-177">String</span></span>|<span data-ttu-id="3b3bd-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-178">Notes for the app.</span></span> <span data-ttu-id="3b3bd-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3b3bd-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="3b3bd-180">publishingState</span></span>|<span data-ttu-id="3b3bd-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-181">String</span></span>|<span data-ttu-id="3b3bd-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-182">The publishing state for the app.</span></span> <span data-ttu-id="3b3bd-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3b3bd-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3b3bd-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="3b3bd-185">appAvailability</span></span>|<span data-ttu-id="3b3bd-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-186">String</span></span>|<span data-ttu-id="3b3bd-187">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-187">The Application's availability.</span></span> <span data-ttu-id="3b3bd-188">Herdado de [managedApp](../resources/intune_apps_managedapp.md). Os possíveis valores são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="3b3bd-189">version</span><span class="sxs-lookup"><span data-stu-id="3b3bd-189">version</span></span>|<span data-ttu-id="3b3bd-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-190">String</span></span>|<span data-ttu-id="3b3bd-191">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-191">The Application's version.</span></span> <span data-ttu-id="3b3bd-192">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="3b3bd-193">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3b3bd-193">committedContentVersion</span></span>|<span data-ttu-id="3b3bd-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-194">String</span></span>|<span data-ttu-id="3b3bd-195">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-195">The internal committed content version.</span></span> <span data-ttu-id="3b3bd-196">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-196">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="3b3bd-197">fileName</span><span class="sxs-lookup"><span data-stu-id="3b3bd-197">fileName</span></span>|<span data-ttu-id="3b3bd-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-198">String</span></span>|<span data-ttu-id="3b3bd-199">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-199">The name of the main Lob application file.</span></span> <span data-ttu-id="3b3bd-200">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-200">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="3b3bd-201">size</span><span class="sxs-lookup"><span data-stu-id="3b3bd-201">size</span></span>|<span data-ttu-id="3b3bd-202">Int64</span><span class="sxs-lookup"><span data-stu-id="3b3bd-202">Int64</span></span>|<span data-ttu-id="3b3bd-203">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-203">The total size, including all uploaded files.</span></span> <span data-ttu-id="3b3bd-204">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b3bd-204">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="3b3bd-205">packageId</span><span class="sxs-lookup"><span data-stu-id="3b3bd-205">packageId</span></span>|<span data-ttu-id="3b3bd-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-206">String</span></span>|<span data-ttu-id="3b3bd-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-207">The package identifier.</span></span>|
|<span data-ttu-id="3b3bd-208">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b3bd-208">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3b3bd-209">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b3bd-209">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="3b3bd-210">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-210">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3b3bd-211">versionName</span><span class="sxs-lookup"><span data-stu-id="3b3bd-211">versionName</span></span>|<span data-ttu-id="3b3bd-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-212">String</span></span>|<span data-ttu-id="3b3bd-213">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-213">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3b3bd-214">versionCode</span><span class="sxs-lookup"><span data-stu-id="3b3bd-214">versionCode</span></span>|<span data-ttu-id="3b3bd-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3bd-215">String</span></span>|<span data-ttu-id="3b3bd-216">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-216">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="3b3bd-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b3bd-217">Response</span></span>
<span data-ttu-id="3b3bd-218">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-218">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b3bd-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b3bd-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b3bd-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b3bd-220">Request</span></span>
<span data-ttu-id="3b3bd-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1158

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

### <a name="response"></a><span data-ttu-id="3b3bd-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b3bd-222">Response</span></span>
<span data-ttu-id="3b3bd-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b3bd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



