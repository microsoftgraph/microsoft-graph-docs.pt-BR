# <a name="create-managedioslobapp"></a><span data-ttu-id="0f8af-101">Criar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="0f8af-101">Create managedIOSLobApp</span></span>

> <span data-ttu-id="0f8af-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0f8af-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f8af-103">Cria um novo objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f8af-103">Create a new [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f8af-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f8af-104">Prerequisites</span></span>
<span data-ttu-id="0f8af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f8af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0f8af-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f8af-107">Permission type</span></span>|<span data-ttu-id="0f8af-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f8af-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f8af-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f8af-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0f8af-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f8af-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f8af-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f8af-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f8af-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f8af-112">Not supported.</span></span>|
|<span data-ttu-id="0f8af-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f8af-113">Application</span></span>|<span data-ttu-id="0f8af-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f8af-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f8af-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f8af-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0f8af-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f8af-116">Request headers</span></span>
|<span data-ttu-id="0f8af-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f8af-117">Header</span></span>|<span data-ttu-id="0f8af-118">Valor</span><span class="sxs-lookup"><span data-stu-id="0f8af-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f8af-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f8af-119">Authorization</span></span>|<span data-ttu-id="0f8af-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="0f8af-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f8af-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f8af-121">Accept</span></span>|<span data-ttu-id="0f8af-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0f8af-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f8af-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f8af-123">Request body</span></span>
<span data-ttu-id="0f8af-124">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="0f8af-124">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="0f8af-125">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="0f8af-125">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="0f8af-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f8af-126">Property</span></span>|<span data-ttu-id="0f8af-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f8af-127">Type</span></span>|<span data-ttu-id="0f8af-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f8af-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f8af-129">id</span><span class="sxs-lookup"><span data-stu-id="0f8af-129">id</span></span>|<span data-ttu-id="0f8af-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-130">String</span></span>|<span data-ttu-id="0f8af-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f8af-131">Key of the entity.</span></span> <span data-ttu-id="0f8af-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0f8af-133">displayName</span></span>|<span data-ttu-id="0f8af-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-134">String</span></span>|<span data-ttu-id="0f8af-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0f8af-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0f8af-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-137">description</span><span class="sxs-lookup"><span data-stu-id="0f8af-137">description</span></span>|<span data-ttu-id="0f8af-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-138">String</span></span>|<span data-ttu-id="0f8af-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f8af-139">The description of the app.</span></span> <span data-ttu-id="0f8af-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-141">publisher</span><span class="sxs-lookup"><span data-stu-id="0f8af-141">publisher</span></span>|<span data-ttu-id="0f8af-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-142">String</span></span>|<span data-ttu-id="0f8af-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f8af-143">The publisher of the app.</span></span> <span data-ttu-id="0f8af-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0f8af-145">largeIcon</span></span>|[<span data-ttu-id="0f8af-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f8af-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="0f8af-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0f8af-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0f8af-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f8af-149">createdDateTime</span></span>|<span data-ttu-id="0f8af-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f8af-150">DateTimeOffset</span></span>|<span data-ttu-id="0f8af-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f8af-151">The date and time the app was created.</span></span> <span data-ttu-id="0f8af-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f8af-153">lastModifiedDateTime</span></span>|<span data-ttu-id="0f8af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f8af-154">DateTimeOffset</span></span>|<span data-ttu-id="0f8af-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0f8af-155">The date and time the app was last modified.</span></span> <span data-ttu-id="0f8af-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0f8af-157">isFeatured</span></span>|<span data-ttu-id="0f8af-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="0f8af-158">Boolean</span></span>|<span data-ttu-id="0f8af-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0f8af-160">privacyInformationUrl</span></span>|<span data-ttu-id="0f8af-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-161">String</span></span>|<span data-ttu-id="0f8af-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0f8af-162">The privacy statement Url.</span></span> <span data-ttu-id="0f8af-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0f8af-164">informationUrl</span></span>|<span data-ttu-id="0f8af-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-165">String</span></span>|<span data-ttu-id="0f8af-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0f8af-166">The more information Url.</span></span> <span data-ttu-id="0f8af-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-168">owner</span><span class="sxs-lookup"><span data-stu-id="0f8af-168">owner</span></span>|<span data-ttu-id="0f8af-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-169">String</span></span>|<span data-ttu-id="0f8af-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0f8af-170">The owner of the app.</span></span> <span data-ttu-id="0f8af-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-172">developer</span><span class="sxs-lookup"><span data-stu-id="0f8af-172">developer</span></span>|<span data-ttu-id="0f8af-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-173">String</span></span>|<span data-ttu-id="0f8af-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f8af-174">The developer of the app.</span></span> <span data-ttu-id="0f8af-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-176">Observações</span><span class="sxs-lookup"><span data-stu-id="0f8af-176">notes</span></span>|<span data-ttu-id="0f8af-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-177">String</span></span>|<span data-ttu-id="0f8af-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f8af-178">Notes for the app.</span></span> <span data-ttu-id="0f8af-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="0f8af-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="0f8af-180">publishingState</span></span>|[<span data-ttu-id="0f8af-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0f8af-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="0f8af-p114">O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos que esteja publicado. Herdada de [mobileApp](../resources/intune_apps_mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0f8af-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0f8af-186">appAvailability</span><span class="sxs-lookup"><span data-stu-id="0f8af-186">appAvailability</span></span>|[<span data-ttu-id="0f8af-187">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="0f8af-187">managedAppAvailability</span></span>](../resources/intune_apps_managedappavailability.md)|<span data-ttu-id="0f8af-p115">A disponibilidade do aplicativo. Herdada de [managedApp](../resources/intune_apps_managedapp.md). Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="0f8af-p115">The Application's availability. Inherited from [managedApp](../resources/intune_apps_managedapp.md). The possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="0f8af-191">version</span><span class="sxs-lookup"><span data-stu-id="0f8af-191">version</span></span>|<span data-ttu-id="0f8af-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-192">String</span></span>|<span data-ttu-id="0f8af-193">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f8af-193">The Application's version.</span></span> <span data-ttu-id="0f8af-194">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-194">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="0f8af-195">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0f8af-195">committedContentVersion</span></span>|<span data-ttu-id="0f8af-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-196">String</span></span>|<span data-ttu-id="0f8af-197">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="0f8af-197">The internal committed content version.</span></span> <span data-ttu-id="0f8af-198">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-198">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="0f8af-199">fileName</span><span class="sxs-lookup"><span data-stu-id="0f8af-199">fileName</span></span>|<span data-ttu-id="0f8af-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-200">String</span></span>|<span data-ttu-id="0f8af-201">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="0f8af-201">The name of the main Lob application file.</span></span> <span data-ttu-id="0f8af-202">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-202">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="0f8af-203">size</span><span class="sxs-lookup"><span data-stu-id="0f8af-203">size</span></span>|<span data-ttu-id="0f8af-204">Int64</span><span class="sxs-lookup"><span data-stu-id="0f8af-204">Int64</span></span>|<span data-ttu-id="0f8af-205">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="0f8af-205">The total size, including all uploaded files.</span></span> <span data-ttu-id="0f8af-206">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f8af-206">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="0f8af-207">bundleId</span><span class="sxs-lookup"><span data-stu-id="0f8af-207">bundleId</span></span>|<span data-ttu-id="0f8af-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-208">String</span></span>|<span data-ttu-id="0f8af-209">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="0f8af-209">The Identity Name.</span></span>|
|<span data-ttu-id="0f8af-210">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="0f8af-210">applicableDeviceType</span></span>|[<span data-ttu-id="0f8af-211">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="0f8af-211">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="0f8af-212">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="0f8af-212">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="0f8af-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f8af-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0f8af-214">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f8af-214">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="0f8af-215">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="0f8af-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="0f8af-216">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0f8af-216">expirationDateTime</span></span>|<span data-ttu-id="0f8af-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f8af-217">DateTimeOffset</span></span>|<span data-ttu-id="0f8af-218">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="0f8af-218">The expiration time.</span></span>|
|<span data-ttu-id="0f8af-219">versionNumber</span><span class="sxs-lookup"><span data-stu-id="0f8af-219">versionNumber</span></span>|<span data-ttu-id="0f8af-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-220">String</span></span>|<span data-ttu-id="0f8af-221">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="0f8af-221">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0f8af-222">buildNumber</span><span class="sxs-lookup"><span data-stu-id="0f8af-222">buildNumber</span></span>|<span data-ttu-id="0f8af-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f8af-223">String</span></span>|<span data-ttu-id="0f8af-224">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="0f8af-224">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="0f8af-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f8af-225">Response</span></span>
<span data-ttu-id="0f8af-226">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f8af-226">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f8af-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f8af-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f8af-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f8af-228">Request</span></span>
<span data-ttu-id="0f8af-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f8af-229">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f8af-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f8af-230">Response</span></span>
<span data-ttu-id="0f8af-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f8af-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








