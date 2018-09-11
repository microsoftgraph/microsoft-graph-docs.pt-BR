# <a name="update-iosvppapp"></a><span data-ttu-id="3c308-101">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="3c308-101">Update iosVppApp</span></span>

> <span data-ttu-id="3c308-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3c308-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c308-103">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c308-103">Update the properties of a [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c308-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c308-104">Prerequisites</span></span>
<span data-ttu-id="3c308-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3c308-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3c308-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c308-107">Permission type</span></span>|<span data-ttu-id="3c308-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c308-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c308-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c308-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3c308-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c308-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c308-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c308-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c308-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c308-112">Not supported.</span></span>|
|<span data-ttu-id="3c308-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c308-113">Application</span></span>|<span data-ttu-id="3c308-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c308-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c308-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c308-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="3c308-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c308-116">Request headers</span></span>
|<span data-ttu-id="3c308-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c308-117">Header</span></span>|<span data-ttu-id="3c308-118">Valor</span><span class="sxs-lookup"><span data-stu-id="3c308-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c308-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c308-119">Authorization</span></span>|<span data-ttu-id="3c308-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="3c308-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c308-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c308-121">Accept</span></span>|<span data-ttu-id="3c308-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="3c308-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c308-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c308-123">Request body</span></span>
<span data-ttu-id="3c308-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c308-124">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>

<span data-ttu-id="3c308-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c308-125">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune_apps_iosvppapp.md).</span></span>

|<span data-ttu-id="3c308-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c308-126">Property</span></span>|<span data-ttu-id="3c308-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c308-127">Type</span></span>|<span data-ttu-id="3c308-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c308-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c308-129">id</span><span class="sxs-lookup"><span data-stu-id="3c308-129">id</span></span>|<span data-ttu-id="3c308-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-130">String</span></span>|<span data-ttu-id="3c308-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3c308-131">Key of the entity.</span></span> <span data-ttu-id="3c308-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3c308-133">displayName</span></span>|<span data-ttu-id="3c308-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-134">String</span></span>|<span data-ttu-id="3c308-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3c308-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3c308-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-137">description</span><span class="sxs-lookup"><span data-stu-id="3c308-137">description</span></span>|<span data-ttu-id="3c308-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-138">String</span></span>|<span data-ttu-id="3c308-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3c308-139">The description of the app.</span></span> <span data-ttu-id="3c308-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-141">publisher</span><span class="sxs-lookup"><span data-stu-id="3c308-141">publisher</span></span>|<span data-ttu-id="3c308-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-142">String</span></span>|<span data-ttu-id="3c308-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3c308-143">The publisher of the app.</span></span> <span data-ttu-id="3c308-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3c308-145">largeIcon</span></span>|[<span data-ttu-id="3c308-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3c308-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="3c308-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="3c308-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3c308-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c308-149">createdDateTime</span></span>|<span data-ttu-id="3c308-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c308-150">DateTimeOffset</span></span>|<span data-ttu-id="3c308-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3c308-151">The date and time the app was created.</span></span> <span data-ttu-id="3c308-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c308-153">lastModifiedDateTime</span></span>|<span data-ttu-id="3c308-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c308-154">DateTimeOffset</span></span>|<span data-ttu-id="3c308-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3c308-155">The date and time the app was last modified.</span></span> <span data-ttu-id="3c308-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3c308-157">isFeatured</span></span>|<span data-ttu-id="3c308-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="3c308-158">Boolean</span></span>|<span data-ttu-id="3c308-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3c308-160">privacyInformationUrl</span></span>|<span data-ttu-id="3c308-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-161">String</span></span>|<span data-ttu-id="3c308-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3c308-162">The privacy statement Url.</span></span> <span data-ttu-id="3c308-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3c308-164">informationUrl</span></span>|<span data-ttu-id="3c308-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-165">String</span></span>|<span data-ttu-id="3c308-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3c308-166">The more information Url.</span></span> <span data-ttu-id="3c308-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-168">owner</span><span class="sxs-lookup"><span data-stu-id="3c308-168">owner</span></span>|<span data-ttu-id="3c308-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-169">String</span></span>|<span data-ttu-id="3c308-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3c308-170">The owner of the app.</span></span> <span data-ttu-id="3c308-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-172">developer</span><span class="sxs-lookup"><span data-stu-id="3c308-172">developer</span></span>|<span data-ttu-id="3c308-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-173">String</span></span>|<span data-ttu-id="3c308-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3c308-174">The developer of the app.</span></span> <span data-ttu-id="3c308-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-176">Observações</span><span class="sxs-lookup"><span data-stu-id="3c308-176">notes</span></span>|<span data-ttu-id="3c308-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-177">String</span></span>|<span data-ttu-id="3c308-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3c308-178">Notes for the app.</span></span> <span data-ttu-id="3c308-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3c308-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="3c308-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="3c308-180">publishingState</span></span>|[<span data-ttu-id="3c308-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3c308-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="3c308-p114">O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos que esteja publicado. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3c308-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3c308-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3c308-186">usedLicenseCount</span></span>|<span data-ttu-id="3c308-187">Int32</span><span class="sxs-lookup"><span data-stu-id="3c308-187">Int32</span></span>|<span data-ttu-id="3c308-188">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="3c308-188">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="3c308-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3c308-189">totalLicenseCount</span></span>|<span data-ttu-id="3c308-190">Int32</span><span class="sxs-lookup"><span data-stu-id="3c308-190">Int32</span></span>|<span data-ttu-id="3c308-191">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="3c308-191">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="3c308-192">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="3c308-192">releaseDateTime</span></span>|<span data-ttu-id="3c308-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c308-193">DateTimeOffset</span></span>|<span data-ttu-id="3c308-194">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="3c308-194">The VPP application release date and time.</span></span>|
|<span data-ttu-id="3c308-195">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3c308-195">appStoreUrl</span></span>|<span data-ttu-id="3c308-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-196">String</span></span>|<span data-ttu-id="3c308-197">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="3c308-197">The store URL.</span></span>|
|<span data-ttu-id="3c308-198">licensingType</span><span class="sxs-lookup"><span data-stu-id="3c308-198">licensingType</span></span>|[<span data-ttu-id="3c308-199">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="3c308-199">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="3c308-200">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="3c308-200">The supported License Type.</span></span>|
|<span data-ttu-id="3c308-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="3c308-201">applicableDeviceType</span></span>|[<span data-ttu-id="3c308-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3c308-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="3c308-203">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="3c308-203">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="3c308-204">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="3c308-204">vppTokenOrganizationName</span></span>|<span data-ttu-id="3c308-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-205">String</span></span>|<span data-ttu-id="3c308-206">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="3c308-206">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="3c308-207">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="3c308-207">vppTokenAccountType</span></span>|[<span data-ttu-id="3c308-208">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="3c308-208">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="3c308-p115">O tipo de programa de compra de volume ao qual o Token do Programa de Compra de Volume da Apple está associado. Os valores possíveis são: `business` `education`. Os valores possíveis são: `business` `education`.</span><span class="sxs-lookup"><span data-stu-id="3c308-p115">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. The possible values are: `business`, `education`. The possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="3c308-212">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="3c308-212">vppTokenAppleId</span></span>|<span data-ttu-id="3c308-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-213">String</span></span>|<span data-ttu-id="3c308-214">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="3c308-214">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3c308-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="3c308-215">bundleId</span></span>|<span data-ttu-id="3c308-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c308-216">String</span></span>|<span data-ttu-id="3c308-217">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="3c308-217">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="3c308-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c308-218">Response</span></span>
<span data-ttu-id="3c308-219">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune_apps_iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c308-219">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c308-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c308-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c308-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c308-221">Request</span></span>
<span data-ttu-id="3c308-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c308-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1238

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

### <a name="response"></a><span data-ttu-id="3c308-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c308-223">Response</span></span>
<span data-ttu-id="3c308-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c308-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








