# <a name="create-managedioslobapp"></a><span data-ttu-id="58b46-101">Criar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="58b46-101">Create managedIOSLobApp</span></span>

> <span data-ttu-id="58b46-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="58b46-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58b46-103">Cria um novo objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="58b46-103">Create a new [plannerBucket](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58b46-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58b46-104">Prerequisites</span></span>
<span data-ttu-id="58b46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="58b46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58b46-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58b46-107">Permission type</span></span>|<span data-ttu-id="58b46-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58b46-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58b46-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58b46-109">Delegated (work or school account)</span></span>|<span data-ttu-id="58b46-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58b46-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="58b46-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58b46-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58b46-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58b46-112">Not supported.</span></span>|
|<span data-ttu-id="58b46-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58b46-113">Application</span></span>|<span data-ttu-id="58b46-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58b46-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58b46-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58b46-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="58b46-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58b46-116">Request headers</span></span>
|<span data-ttu-id="58b46-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58b46-117">Header</span></span>|<span data-ttu-id="58b46-118">Valor</span><span class="sxs-lookup"><span data-stu-id="58b46-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58b46-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="58b46-119">Authorization</span></span>|<span data-ttu-id="58b46-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58b46-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="58b46-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58b46-121">Accept</span></span>|<span data-ttu-id="58b46-122">application/json</span><span class="sxs-lookup"><span data-stu-id="58b46-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58b46-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58b46-123">Request body</span></span>
<span data-ttu-id="58b46-124">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="58b46-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="58b46-125">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="58b46-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="58b46-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58b46-126">Property</span></span>|<span data-ttu-id="58b46-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="58b46-127">Type</span></span>|<span data-ttu-id="58b46-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="58b46-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58b46-129">id</span><span class="sxs-lookup"><span data-stu-id="58b46-129">id</span></span>|<span data-ttu-id="58b46-130">String</span><span class="sxs-lookup"><span data-stu-id="58b46-130">String</span></span>|<span data-ttu-id="58b46-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="58b46-131">Key of the setting.</span></span> <span data-ttu-id="58b46-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-133">displayName</span><span class="sxs-lookup"><span data-stu-id="58b46-133">displayName</span></span>|<span data-ttu-id="58b46-134">String</span><span class="sxs-lookup"><span data-stu-id="58b46-134">String</span></span>|<span data-ttu-id="58b46-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="58b46-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="58b46-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-137">descrição</span><span class="sxs-lookup"><span data-stu-id="58b46-137">description</span></span>|<span data-ttu-id="58b46-138">String</span><span class="sxs-lookup"><span data-stu-id="58b46-138">String</span></span>|<span data-ttu-id="58b46-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58b46-139">The description of the app.</span></span> <span data-ttu-id="58b46-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-141">publicador</span><span class="sxs-lookup"><span data-stu-id="58b46-141">Publisher</span></span>|<span data-ttu-id="58b46-142">String</span><span class="sxs-lookup"><span data-stu-id="58b46-142">String</span></span>|<span data-ttu-id="58b46-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58b46-143">The publisher of the app.</span></span> <span data-ttu-id="58b46-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="58b46-145">largeIcon</span></span>|[<span data-ttu-id="58b46-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="58b46-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="58b46-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="58b46-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="58b46-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58b46-149">createdDateTime</span></span>|<span data-ttu-id="58b46-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58b46-150">DateTimeOffset</span></span>|<span data-ttu-id="58b46-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58b46-151">The date and time the group was created.</span></span> <span data-ttu-id="58b46-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58b46-153">lastModifiedDateTime</span></span>|<span data-ttu-id="58b46-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58b46-154">DateTimeOffset</span></span>|<span data-ttu-id="58b46-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="58b46-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="58b46-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="58b46-157">isFeatured</span></span>|<span data-ttu-id="58b46-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="58b46-158">Boolean</span></span>|<span data-ttu-id="58b46-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="58b46-160">privacyInformationUrl</span></span>|<span data-ttu-id="58b46-161">String</span><span class="sxs-lookup"><span data-stu-id="58b46-161">String</span></span>|<span data-ttu-id="58b46-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="58b46-162">The privacy statement Url.</span></span> <span data-ttu-id="58b46-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="58b46-164">informationUrl</span></span>|<span data-ttu-id="58b46-165">String</span><span class="sxs-lookup"><span data-stu-id="58b46-165">String</span></span>|<span data-ttu-id="58b46-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="58b46-166">The more information Url.</span></span> <span data-ttu-id="58b46-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-168">owner</span><span class="sxs-lookup"><span data-stu-id="58b46-168">owner</span></span>|<span data-ttu-id="58b46-169">String</span><span class="sxs-lookup"><span data-stu-id="58b46-169">String</span></span>|<span data-ttu-id="58b46-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="58b46-170">The owner of the app.</span></span> <span data-ttu-id="58b46-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-172">developer</span><span class="sxs-lookup"><span data-stu-id="58b46-172">"developer"</span></span>|<span data-ttu-id="58b46-173">String</span><span class="sxs-lookup"><span data-stu-id="58b46-173">String</span></span>|<span data-ttu-id="58b46-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58b46-174">The developer of the app.</span></span> <span data-ttu-id="58b46-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-176">Observações</span><span class="sxs-lookup"><span data-stu-id="58b46-176">Notes</span></span>|<span data-ttu-id="58b46-177">String</span><span class="sxs-lookup"><span data-stu-id="58b46-177">String</span></span>|<span data-ttu-id="58b46-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58b46-178">Notes for the app.</span></span> <span data-ttu-id="58b46-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="58b46-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="58b46-180">publishingState</span></span>|<span data-ttu-id="58b46-181">String</span><span class="sxs-lookup"><span data-stu-id="58b46-181">String</span></span>|<span data-ttu-id="58b46-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58b46-182">The publishing state for the app.</span></span> <span data-ttu-id="58b46-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="58b46-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="58b46-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="58b46-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="58b46-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="58b46-185">appAvailability</span></span>|<span data-ttu-id="58b46-186">String</span><span class="sxs-lookup"><span data-stu-id="58b46-186">String</span></span>|<span data-ttu-id="58b46-187">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58b46-187">The Application's availability.</span></span> <span data-ttu-id="58b46-188">Herdado de [managedApp](../resources/intune_apps_managedapp.md). Os possíveis valores são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="58b46-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="58b46-189">version</span><span class="sxs-lookup"><span data-stu-id="58b46-189">version</span></span>|<span data-ttu-id="58b46-190">String</span><span class="sxs-lookup"><span data-stu-id="58b46-190">String</span></span>|<span data-ttu-id="58b46-191">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58b46-191">The Application's version.</span></span> <span data-ttu-id="58b46-192">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="58b46-193">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="58b46-193">committedContentVersion</span></span>|<span data-ttu-id="58b46-194">String</span><span class="sxs-lookup"><span data-stu-id="58b46-194">String</span></span>|<span data-ttu-id="58b46-195">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="58b46-195">The internal committed content version.</span></span> <span data-ttu-id="58b46-196">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-196">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="58b46-197">fileName</span><span class="sxs-lookup"><span data-stu-id="58b46-197">fileName</span></span>|<span data-ttu-id="58b46-198">String</span><span class="sxs-lookup"><span data-stu-id="58b46-198">String</span></span>|<span data-ttu-id="58b46-199">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="58b46-199">The name of the main Lob application file.</span></span> <span data-ttu-id="58b46-200">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-200">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="58b46-201">size</span><span class="sxs-lookup"><span data-stu-id="58b46-201">size</span></span>|<span data-ttu-id="58b46-202">Int64</span><span class="sxs-lookup"><span data-stu-id="58b46-202">Int64</span></span>|<span data-ttu-id="58b46-203">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="58b46-203">The total size, including all uploaded files.</span></span> <span data-ttu-id="58b46-204">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="58b46-204">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="58b46-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="58b46-205">bundleId</span></span>|<span data-ttu-id="58b46-206">String</span><span class="sxs-lookup"><span data-stu-id="58b46-206">String</span></span>|<span data-ttu-id="58b46-207">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="58b46-207">The Identity Name.</span></span>|
|<span data-ttu-id="58b46-208">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="58b46-208">applicableDeviceType</span></span>|[<span data-ttu-id="58b46-209">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="58b46-209">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="58b46-210">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="58b46-210">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="58b46-211">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="58b46-211">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="58b46-212">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="58b46-212">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="58b46-213">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="58b46-213">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="58b46-214">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="58b46-214">expirationDateTime</span></span>|<span data-ttu-id="58b46-215">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58b46-215">DateTimeOffset</span></span>|<span data-ttu-id="58b46-216">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="58b46-216">: The expiration time for the subscription.</span></span>|
|<span data-ttu-id="58b46-217">versionNumber</span><span class="sxs-lookup"><span data-stu-id="58b46-217">versionNumber</span></span>|<span data-ttu-id="58b46-218">String</span><span class="sxs-lookup"><span data-stu-id="58b46-218">String</span></span>|<span data-ttu-id="58b46-219">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="58b46-219">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="58b46-220">buildNumber</span><span class="sxs-lookup"><span data-stu-id="58b46-220">buildNumber</span></span>|<span data-ttu-id="58b46-221">String</span><span class="sxs-lookup"><span data-stu-id="58b46-221">String</span></span>|<span data-ttu-id="58b46-222">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="58b46-222">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="58b46-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="58b46-223">Response</span></span>
<span data-ttu-id="58b46-224">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58b46-224">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58b46-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58b46-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="58b46-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58b46-226">Request</span></span>
<span data-ttu-id="58b46-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58b46-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58b46-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="58b46-228">Response</span></span>
<span data-ttu-id="58b46-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58b46-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



