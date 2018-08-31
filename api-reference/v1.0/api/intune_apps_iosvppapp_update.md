# <a name="update-iosvppapp"></a><span data-ttu-id="12c27-101">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="12c27-101">Update iosVppApp</span></span>

> <span data-ttu-id="12c27-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="12c27-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12c27-103">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="12c27-103">Update the properties of a [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12c27-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12c27-104">Prerequisites</span></span>
<span data-ttu-id="12c27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="12c27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12c27-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12c27-107">Permission type</span></span>|<span data-ttu-id="12c27-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12c27-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12c27-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12c27-109">Delegated (work or school account)</span></span>|<span data-ttu-id="12c27-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c27-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12c27-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12c27-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12c27-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12c27-112">Not supported.</span></span>|
|<span data-ttu-id="12c27-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12c27-113">Application</span></span>|<span data-ttu-id="12c27-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12c27-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12c27-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12c27-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="12c27-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12c27-116">Request headers</span></span>
|<span data-ttu-id="12c27-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12c27-117">Header</span></span>|<span data-ttu-id="12c27-118">Valor</span><span class="sxs-lookup"><span data-stu-id="12c27-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12c27-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="12c27-119">Authorization</span></span>|<span data-ttu-id="12c27-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="12c27-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12c27-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12c27-121">Accept</span></span>|<span data-ttu-id="12c27-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="12c27-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12c27-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12c27-123">Request body</span></span>
<span data-ttu-id="12c27-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="12c27-124">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune_apps_iosvppapp.md) object.</span></span>

<span data-ttu-id="12c27-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune_apps_iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="12c27-125">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune_apps_iosvppapp.md).</span></span>

|<span data-ttu-id="12c27-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12c27-126">Property</span></span>|<span data-ttu-id="12c27-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="12c27-127">Type</span></span>|<span data-ttu-id="12c27-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="12c27-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12c27-129">id</span><span class="sxs-lookup"><span data-stu-id="12c27-129">id</span></span>|<span data-ttu-id="12c27-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-130">String</span></span>|<span data-ttu-id="12c27-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="12c27-131">Key of the entity.</span></span> <span data-ttu-id="12c27-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-133">displayName</span><span class="sxs-lookup"><span data-stu-id="12c27-133">displayName</span></span>|<span data-ttu-id="12c27-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-134">String</span></span>|<span data-ttu-id="12c27-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="12c27-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="12c27-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-137">description</span><span class="sxs-lookup"><span data-stu-id="12c27-137">description</span></span>|<span data-ttu-id="12c27-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-138">String</span></span>|<span data-ttu-id="12c27-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12c27-139">The description of the app.</span></span> <span data-ttu-id="12c27-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-141">publisher</span><span class="sxs-lookup"><span data-stu-id="12c27-141">publisher</span></span>|<span data-ttu-id="12c27-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-142">String</span></span>|<span data-ttu-id="12c27-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12c27-143">The publisher of the app.</span></span> <span data-ttu-id="12c27-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="12c27-145">largeIcon</span></span>|[<span data-ttu-id="12c27-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="12c27-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="12c27-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="12c27-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="12c27-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12c27-149">createdDateTime</span></span>|<span data-ttu-id="12c27-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12c27-150">DateTimeOffset</span></span>|<span data-ttu-id="12c27-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12c27-151">The date and time the app was created.</span></span> <span data-ttu-id="12c27-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12c27-153">lastModifiedDateTime</span></span>|<span data-ttu-id="12c27-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12c27-154">DateTimeOffset</span></span>|<span data-ttu-id="12c27-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="12c27-155">The date and time the app was last modified.</span></span> <span data-ttu-id="12c27-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="12c27-157">isFeatured</span></span>|<span data-ttu-id="12c27-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="12c27-158">Boolean</span></span>|<span data-ttu-id="12c27-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="12c27-160">privacyInformationUrl</span></span>|<span data-ttu-id="12c27-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-161">String</span></span>|<span data-ttu-id="12c27-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="12c27-162">The privacy statement Url.</span></span> <span data-ttu-id="12c27-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="12c27-164">informationUrl</span></span>|<span data-ttu-id="12c27-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-165">String</span></span>|<span data-ttu-id="12c27-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="12c27-166">The more information Url.</span></span> <span data-ttu-id="12c27-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-168">owner</span><span class="sxs-lookup"><span data-stu-id="12c27-168">owner</span></span>|<span data-ttu-id="12c27-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-169">String</span></span>|<span data-ttu-id="12c27-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="12c27-170">The owner of the app.</span></span> <span data-ttu-id="12c27-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-172">developer</span><span class="sxs-lookup"><span data-stu-id="12c27-172">developer</span></span>|<span data-ttu-id="12c27-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-173">String</span></span>|<span data-ttu-id="12c27-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12c27-174">The developer of the app.</span></span> <span data-ttu-id="12c27-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-176">Observações</span><span class="sxs-lookup"><span data-stu-id="12c27-176">notes</span></span>|<span data-ttu-id="12c27-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-177">String</span></span>|<span data-ttu-id="12c27-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12c27-178">Notes for the app.</span></span> <span data-ttu-id="12c27-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12c27-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="12c27-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="12c27-180">publishingState</span></span>|[<span data-ttu-id="12c27-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="12c27-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="12c27-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12c27-182">The publishing state for the app.</span></span> <span data-ttu-id="12c27-183">O aplicativo não pode ser atribuído, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="12c27-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="12c27-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="12c27-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="12c27-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="12c27-185">The possible values are:</span></span>|
|<span data-ttu-id="12c27-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="12c27-186">usedLicenseCount</span></span>|<span data-ttu-id="12c27-187">Int32</span><span class="sxs-lookup"><span data-stu-id="12c27-187">Int32</span></span>|<span data-ttu-id="12c27-188">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="12c27-188">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="12c27-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="12c27-189">totalLicenseCount</span></span>|<span data-ttu-id="12c27-190">Int32</span><span class="sxs-lookup"><span data-stu-id="12c27-190">Int32</span></span>|<span data-ttu-id="12c27-191">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="12c27-191">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="12c27-192">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="12c27-192">releaseDateTime</span></span>|<span data-ttu-id="12c27-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12c27-193">DateTimeOffset</span></span>|<span data-ttu-id="12c27-194">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="12c27-194">The VPP application release date and time.</span></span>|
|<span data-ttu-id="12c27-195">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="12c27-195">appStoreUrl</span></span>|<span data-ttu-id="12c27-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-196">String</span></span>|<span data-ttu-id="12c27-197">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="12c27-197">The store URL.</span></span>|
|<span data-ttu-id="12c27-198">licensingType</span><span class="sxs-lookup"><span data-stu-id="12c27-198">licensingType</span></span>|[<span data-ttu-id="12c27-199">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="12c27-199">vppLicensingType</span></span>](../resources/intune_apps_vpplicensingtype.md)|<span data-ttu-id="12c27-200">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="12c27-200">The supported License Type.</span></span>|
|<span data-ttu-id="12c27-201">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="12c27-201">applicableDeviceType</span></span>|[<span data-ttu-id="12c27-202">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="12c27-202">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="12c27-203">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="12c27-203">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="12c27-204">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="12c27-204">vppTokenOrganizationName</span></span>|<span data-ttu-id="12c27-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-205">String</span></span>|<span data-ttu-id="12c27-206">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="12c27-206">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="12c27-207">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="12c27-207">vppTokenAccountType</span></span>|[<span data-ttu-id="12c27-208">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="12c27-208">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="12c27-209">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="12c27-209">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="12c27-210">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="12c27-210">The possible values are:</span></span> <span data-ttu-id="12c27-211">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="12c27-211">The possible values are:</span></span>|
|<span data-ttu-id="12c27-212">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="12c27-212">vppTokenAppleId</span></span>|<span data-ttu-id="12c27-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-213">String</span></span>|<span data-ttu-id="12c27-214">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="12c27-214">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="12c27-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="12c27-215">bundleId</span></span>|<span data-ttu-id="12c27-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12c27-216">String</span></span>|<span data-ttu-id="12c27-217">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="12c27-217">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="12c27-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="12c27-218">Response</span></span>
<span data-ttu-id="12c27-219">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune_apps_iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12c27-219">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune_apps_iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c27-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12c27-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="12c27-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12c27-221">Request</span></span>
<span data-ttu-id="12c27-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12c27-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="12c27-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="12c27-223">Response</span></span>
<span data-ttu-id="12c27-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12c27-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



