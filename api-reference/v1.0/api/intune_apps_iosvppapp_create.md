# <a name="create-iosvppapp"></a><span data-ttu-id="b855c-101">Criar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="b855c-101">Create iosVppApp</span></span>

> <span data-ttu-id="b855c-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b855c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b855c-103">Cria um novo objeto [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="b855c-103">Create a new [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b855c-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b855c-104">Prerequisites</span></span>
<span data-ttu-id="b855c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b855c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b855c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b855c-107">Permission type</span></span>|<span data-ttu-id="b855c-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b855c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b855c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b855c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b855c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b855c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b855c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b855c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b855c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b855c-112">Not supported.</span></span>|
|<span data-ttu-id="b855c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b855c-113">Application</span></span>|<span data-ttu-id="b855c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b855c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b855c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b855c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b855c-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b855c-116">Request headers</span></span>
|<span data-ttu-id="b855c-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b855c-117">Header</span></span>|<span data-ttu-id="b855c-118">Valor</span><span class="sxs-lookup"><span data-stu-id="b855c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b855c-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="b855c-119">Authorization</span></span>|<span data-ttu-id="b855c-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="b855c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b855c-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b855c-121">Accept</span></span>|<span data-ttu-id="b855c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b855c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b855c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b855c-123">Request body</span></span>
<span data-ttu-id="b855c-124">No corpo da solicitação, forneça uma representação JSON do objeto iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="b855c-124">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="b855c-125">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="b855c-125">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="b855c-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b855c-126">Property</span></span>|<span data-ttu-id="b855c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b855c-127">Type</span></span>|<span data-ttu-id="b855c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b855c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b855c-129">id</span><span class="sxs-lookup"><span data-stu-id="b855c-129">id</span></span>|<span data-ttu-id="b855c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-130">String</span></span>|<span data-ttu-id="b855c-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b855c-131">Key of the entity.</span></span> <span data-ttu-id="b855c-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b855c-133">displayName</span></span>|<span data-ttu-id="b855c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-134">String</span></span>|<span data-ttu-id="b855c-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b855c-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b855c-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-137">description</span><span class="sxs-lookup"><span data-stu-id="b855c-137">description</span></span>|<span data-ttu-id="b855c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-138">String</span></span>|<span data-ttu-id="b855c-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b855c-139">The description of the app.</span></span> <span data-ttu-id="b855c-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-141">publisher</span><span class="sxs-lookup"><span data-stu-id="b855c-141">publisher</span></span>|<span data-ttu-id="b855c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-142">String</span></span>|<span data-ttu-id="b855c-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b855c-143">The publisher of the app.</span></span> <span data-ttu-id="b855c-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b855c-145">largeIcon</span></span>|[<span data-ttu-id="b855c-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b855c-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="b855c-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b855c-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b855c-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b855c-149">createdDateTime</span></span>|<span data-ttu-id="b855c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b855c-150">DateTimeOffset</span></span>|<span data-ttu-id="b855c-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b855c-151">The date and time the app was created.</span></span> <span data-ttu-id="b855c-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b855c-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b855c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b855c-154">DateTimeOffset</span></span>|<span data-ttu-id="b855c-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b855c-155">The date and time the app was last modified.</span></span> <span data-ttu-id="b855c-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b855c-157">isFeatured</span></span>|<span data-ttu-id="b855c-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="b855c-158">Boolean</span></span>|<span data-ttu-id="b855c-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b855c-160">privacyInformationUrl</span></span>|<span data-ttu-id="b855c-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-161">String</span></span>|<span data-ttu-id="b855c-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b855c-162">The privacy statement Url.</span></span> <span data-ttu-id="b855c-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b855c-164">informationUrl</span></span>|<span data-ttu-id="b855c-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-165">String</span></span>|<span data-ttu-id="b855c-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b855c-166">The more information Url.</span></span> <span data-ttu-id="b855c-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-168">owner</span><span class="sxs-lookup"><span data-stu-id="b855c-168">owner</span></span>|<span data-ttu-id="b855c-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-169">String</span></span>|<span data-ttu-id="b855c-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b855c-170">The owner of the app.</span></span> <span data-ttu-id="b855c-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-172">developer</span><span class="sxs-lookup"><span data-stu-id="b855c-172">developer</span></span>|<span data-ttu-id="b855c-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-173">String</span></span>|<span data-ttu-id="b855c-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b855c-174">The developer of the app.</span></span> <span data-ttu-id="b855c-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-176">Observações</span><span class="sxs-lookup"><span data-stu-id="b855c-176">notes</span></span>|<span data-ttu-id="b855c-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-177">String</span></span>|<span data-ttu-id="b855c-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b855c-178">Notes for the app.</span></span> <span data-ttu-id="b855c-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b855c-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b855c-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="b855c-180">publishingState</span></span>|[<span data-ttu-id="b855c-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b855c-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="b855c-p114">O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos que esteja publicado. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b855c-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b855c-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b855c-186">usedLicenseCount</span></span>|<span data-ttu-id="b855c-187">Int32</span><span class="sxs-lookup"><span data-stu-id="b855c-187">Int32</span></span>|<span data-ttu-id="b855c-188">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="b855c-188">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="b855c-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b855c-189">totalLicenseCount</span></span>|<span data-ttu-id="b855c-190">Int32</span><span class="sxs-lookup"><span data-stu-id="b855c-190">Int32</span></span>|<span data-ttu-id="b855c-191">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="b855c-191">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="b855c-192">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="b855c-192">releaseDateTime</span></span>|<span data-ttu-id="b855c-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b855c-193">DateTimeOffset</span></span>|<span data-ttu-id="b855c-194">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="b855c-194">The VPP application release date and time.</span></span>|
|<span data-ttu-id="b855c-195">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b855c-195">appStoreUrl</span></span>|<span data-ttu-id="b855c-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-196">String</span></span>|<span data-ttu-id="b855c-197">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="b855c-197">The store URL.</span></span>|
|<span data-ttu-id="b855c-198">licensingType</span><span class="sxs-lookup"><span data-stu-id="b855c-198">licensingType</span></span>|[<span data-ttu-id="b855c-199">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="b855c-199">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="b855c-200">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="b855c-200">The supported License Type.</span></span>|
|<span data-ttu-id="b855c-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="b855c-201">applicableDeviceType</span></span>|[<span data-ttu-id="b855c-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b855c-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="b855c-203">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="b855c-203">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="b855c-204">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="b855c-204">vppTokenOrganizationName</span></span>|<span data-ttu-id="b855c-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-205">String</span></span>|<span data-ttu-id="b855c-206">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="b855c-206">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="b855c-207">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b855c-207">vppTokenAccountType</span></span>|[<span data-ttu-id="b855c-208">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b855c-208">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="b855c-p115">O tipo de programa de compra de volume ao qual o Token do Programa de Compra de Volume da Apple está associado. Os valores possíveis são: `business` `education`. Os valores possíveis são: `business` `education`.</span><span class="sxs-lookup"><span data-stu-id="b855c-p115">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. The possible values are: `business`, `education`. The possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="b855c-212">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="b855c-212">vppTokenAppleId</span></span>|<span data-ttu-id="b855c-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-213">String</span></span>|<span data-ttu-id="b855c-214">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="b855c-214">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b855c-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="b855c-215">bundleId</span></span>|<span data-ttu-id="b855c-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b855c-216">String</span></span>|<span data-ttu-id="b855c-217">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b855c-217">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="b855c-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="b855c-218">Response</span></span>
<span data-ttu-id="b855c-219">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosVppApp](../resources/intune_apps_iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b855c-219">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b855c-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b855c-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="b855c-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b855c-221">Request</span></span>
<span data-ttu-id="b855c-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b855c-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1286

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="b855c-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="b855c-223">Response</span></span>
<span data-ttu-id="b855c-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b855c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```








