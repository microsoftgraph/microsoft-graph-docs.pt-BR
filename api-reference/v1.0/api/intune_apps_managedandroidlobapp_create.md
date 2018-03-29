# <a name="create-managedandroidlobapp"></a><span data-ttu-id="6840b-101">Criar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="6840b-101">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="6840b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6840b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6840b-103">Cria um novo objeto [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6840b-103">Create a new [plannerBucket](../resources/intune_apps_managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6840b-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6840b-104">Prerequisites</span></span>
<span data-ttu-id="6840b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6840b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6840b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6840b-107">Permission type</span></span>|<span data-ttu-id="6840b-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6840b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6840b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6840b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6840b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6840b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6840b-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6840b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6840b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6840b-112">Not supported.</span></span>|
|<span data-ttu-id="6840b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6840b-113">Application</span></span>|<span data-ttu-id="6840b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6840b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6840b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6840b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6840b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6840b-116">Request headers</span></span>
|<span data-ttu-id="6840b-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6840b-117">Header</span></span>|<span data-ttu-id="6840b-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6840b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6840b-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6840b-119">Authorization</span></span>|<span data-ttu-id="6840b-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6840b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6840b-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6840b-121">Accept</span></span>|<span data-ttu-id="6840b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6840b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6840b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6840b-123">Request body</span></span>
<span data-ttu-id="6840b-124">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="6840b-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="6840b-125">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="6840b-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="6840b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6840b-126">Property</span></span>|<span data-ttu-id="6840b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6840b-127">Type</span></span>|<span data-ttu-id="6840b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6840b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6840b-129">id</span><span class="sxs-lookup"><span data-stu-id="6840b-129">id</span></span>|<span data-ttu-id="6840b-130">String</span><span class="sxs-lookup"><span data-stu-id="6840b-130">String</span></span>|<span data-ttu-id="6840b-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6840b-131">Key of the setting.</span></span> <span data-ttu-id="6840b-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6840b-133">displayName</span></span>|<span data-ttu-id="6840b-134">String</span><span class="sxs-lookup"><span data-stu-id="6840b-134">String</span></span>|<span data-ttu-id="6840b-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6840b-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6840b-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-137">descrição</span><span class="sxs-lookup"><span data-stu-id="6840b-137">description</span></span>|<span data-ttu-id="6840b-138">String</span><span class="sxs-lookup"><span data-stu-id="6840b-138">String</span></span>|<span data-ttu-id="6840b-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6840b-139">The description of the app.</span></span> <span data-ttu-id="6840b-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-141">publicador</span><span class="sxs-lookup"><span data-stu-id="6840b-141">Publisher</span></span>|<span data-ttu-id="6840b-142">String</span><span class="sxs-lookup"><span data-stu-id="6840b-142">String</span></span>|<span data-ttu-id="6840b-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6840b-143">The publisher of the app.</span></span> <span data-ttu-id="6840b-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6840b-145">largeIcon</span></span>|[<span data-ttu-id="6840b-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6840b-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="6840b-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6840b-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6840b-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6840b-149">createdDateTime</span></span>|<span data-ttu-id="6840b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6840b-150">DateTimeOffset</span></span>|<span data-ttu-id="6840b-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6840b-151">The date and time the group was created.</span></span> <span data-ttu-id="6840b-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6840b-153">lastModifiedDateTime</span></span>|<span data-ttu-id="6840b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6840b-154">DateTimeOffset</span></span>|<span data-ttu-id="6840b-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6840b-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="6840b-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6840b-157">isFeatured</span></span>|<span data-ttu-id="6840b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="6840b-158">Boolean</span></span>|<span data-ttu-id="6840b-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6840b-160">privacyInformationUrl</span></span>|<span data-ttu-id="6840b-161">String</span><span class="sxs-lookup"><span data-stu-id="6840b-161">String</span></span>|<span data-ttu-id="6840b-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6840b-162">The privacy statement Url.</span></span> <span data-ttu-id="6840b-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6840b-164">informationUrl</span></span>|<span data-ttu-id="6840b-165">String</span><span class="sxs-lookup"><span data-stu-id="6840b-165">String</span></span>|<span data-ttu-id="6840b-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6840b-166">The more information Url.</span></span> <span data-ttu-id="6840b-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-168">owner</span><span class="sxs-lookup"><span data-stu-id="6840b-168">owner</span></span>|<span data-ttu-id="6840b-169">String</span><span class="sxs-lookup"><span data-stu-id="6840b-169">String</span></span>|<span data-ttu-id="6840b-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6840b-170">The owner of the app.</span></span> <span data-ttu-id="6840b-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-172">developer</span><span class="sxs-lookup"><span data-stu-id="6840b-172">"developer"</span></span>|<span data-ttu-id="6840b-173">String</span><span class="sxs-lookup"><span data-stu-id="6840b-173">String</span></span>|<span data-ttu-id="6840b-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6840b-174">The developer of the app.</span></span> <span data-ttu-id="6840b-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-176">Observações</span><span class="sxs-lookup"><span data-stu-id="6840b-176">Notes</span></span>|<span data-ttu-id="6840b-177">String</span><span class="sxs-lookup"><span data-stu-id="6840b-177">String</span></span>|<span data-ttu-id="6840b-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6840b-178">Notes for the app.</span></span> <span data-ttu-id="6840b-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="6840b-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="6840b-180">publishingState</span></span>|<span data-ttu-id="6840b-181">String</span><span class="sxs-lookup"><span data-stu-id="6840b-181">String</span></span>|<span data-ttu-id="6840b-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6840b-182">The publishing state for the app.</span></span> <span data-ttu-id="6840b-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6840b-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6840b-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6840b-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6840b-185">appAvailability</span><span class="sxs-lookup"><span data-stu-id="6840b-185">appAvailability</span></span>|<span data-ttu-id="6840b-186">String</span><span class="sxs-lookup"><span data-stu-id="6840b-186">String</span></span>|<span data-ttu-id="6840b-187">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6840b-187">The Application's availability.</span></span> <span data-ttu-id="6840b-188">Herdado de [managedApp](../resources/intune_apps_managedapp.md). Os possíveis valores são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="6840b-188">Inherited from [managedApp](../resources/intune_apps_managedapp.md) Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="6840b-189">version</span><span class="sxs-lookup"><span data-stu-id="6840b-189">version</span></span>|<span data-ttu-id="6840b-190">String</span><span class="sxs-lookup"><span data-stu-id="6840b-190">String</span></span>|<span data-ttu-id="6840b-191">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6840b-191">The Application's version.</span></span> <span data-ttu-id="6840b-192">Herdado de [managedApp](../resources/intune_apps_managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-192">Inherited from [managedApp](../resources/intune_apps_managedapp.md)</span></span>|
|<span data-ttu-id="6840b-193">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="6840b-193">committedContentVersion</span></span>|<span data-ttu-id="6840b-194">String</span><span class="sxs-lookup"><span data-stu-id="6840b-194">String</span></span>|<span data-ttu-id="6840b-195">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="6840b-195">The internal committed content version.</span></span> <span data-ttu-id="6840b-196">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-196">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="6840b-197">fileName</span><span class="sxs-lookup"><span data-stu-id="6840b-197">fileName</span></span>|<span data-ttu-id="6840b-198">String</span><span class="sxs-lookup"><span data-stu-id="6840b-198">String</span></span>|<span data-ttu-id="6840b-199">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="6840b-199">The name of the main Lob application file.</span></span> <span data-ttu-id="6840b-200">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-200">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="6840b-201">size</span><span class="sxs-lookup"><span data-stu-id="6840b-201">size</span></span>|<span data-ttu-id="6840b-202">Int64</span><span class="sxs-lookup"><span data-stu-id="6840b-202">Int64</span></span>|<span data-ttu-id="6840b-203">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="6840b-203">The total size, including all uploaded files.</span></span> <span data-ttu-id="6840b-204">Herdado de [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6840b-204">Inherited from [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="6840b-205">packageId</span><span class="sxs-lookup"><span data-stu-id="6840b-205">packageId</span></span>|<span data-ttu-id="6840b-206">String</span><span class="sxs-lookup"><span data-stu-id="6840b-206">String</span></span>|<span data-ttu-id="6840b-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="6840b-207">The package identifier.</span></span>|
|<span data-ttu-id="6840b-208">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6840b-208">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6840b-209">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6840b-209">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="6840b-210">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="6840b-210">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="6840b-211">versionName</span><span class="sxs-lookup"><span data-stu-id="6840b-211">versionName</span></span>|<span data-ttu-id="6840b-212">String</span><span class="sxs-lookup"><span data-stu-id="6840b-212">String</span></span>|<span data-ttu-id="6840b-213">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6840b-213">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="6840b-214">versionCode</span><span class="sxs-lookup"><span data-stu-id="6840b-214">versionCode</span></span>|<span data-ttu-id="6840b-215">String</span><span class="sxs-lookup"><span data-stu-id="6840b-215">String</span></span>|<span data-ttu-id="6840b-216">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6840b-216">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="6840b-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="6840b-217">Response</span></span>
<span data-ttu-id="6840b-218">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedAndroidLobApp](../resources/intune_apps_managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6840b-218">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6840b-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6840b-219">Example</span></span>
### <a name="request"></a><span data-ttu-id="6840b-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6840b-220">Request</span></span>
<span data-ttu-id="6840b-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6840b-221">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6840b-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="6840b-222">Response</span></span>
<span data-ttu-id="6840b-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6840b-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



