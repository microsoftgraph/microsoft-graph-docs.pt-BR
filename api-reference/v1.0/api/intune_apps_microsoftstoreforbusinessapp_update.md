# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="00d98-101">Atualizar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="00d98-101">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="00d98-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="00d98-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00d98-103">Atualiza as propriedades de um objeto [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="00d98-103">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00d98-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00d98-104">Prerequisites</span></span>
<span data-ttu-id="00d98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="00d98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00d98-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00d98-107">Permission type</span></span>|<span data-ttu-id="00d98-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00d98-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00d98-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00d98-109">Delegated (work or school account)</span></span>|<span data-ttu-id="00d98-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00d98-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="00d98-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00d98-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00d98-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00d98-112">Not supported.</span></span>|
|<span data-ttu-id="00d98-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00d98-113">Application</span></span>|<span data-ttu-id="00d98-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00d98-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00d98-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00d98-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="00d98-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00d98-116">Request headers</span></span>
|<span data-ttu-id="00d98-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00d98-117">Header</span></span>|<span data-ttu-id="00d98-118">Valor</span><span class="sxs-lookup"><span data-stu-id="00d98-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00d98-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="00d98-119">Authorization</span></span>|<span data-ttu-id="00d98-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="00d98-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00d98-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00d98-121">Accept</span></span>|<span data-ttu-id="00d98-122">application/json</span><span class="sxs-lookup"><span data-stu-id="00d98-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00d98-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00d98-123">Request body</span></span>
<span data-ttu-id="00d98-124">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="00d98-124">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="00d98-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="00d98-125">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="00d98-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00d98-126">Property</span></span>|<span data-ttu-id="00d98-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="00d98-127">Type</span></span>|<span data-ttu-id="00d98-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="00d98-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00d98-129">id</span><span class="sxs-lookup"><span data-stu-id="00d98-129">id</span></span>|<span data-ttu-id="00d98-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-130">String</span></span>|<span data-ttu-id="00d98-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="00d98-131">Key of the entity.</span></span> <span data-ttu-id="00d98-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-133">displayName</span><span class="sxs-lookup"><span data-stu-id="00d98-133">displayName</span></span>|<span data-ttu-id="00d98-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-134">String</span></span>|<span data-ttu-id="00d98-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="00d98-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="00d98-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-137">description</span><span class="sxs-lookup"><span data-stu-id="00d98-137">description</span></span>|<span data-ttu-id="00d98-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-138">String</span></span>|<span data-ttu-id="00d98-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00d98-139">The description of the app.</span></span> <span data-ttu-id="00d98-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-141">publisher</span><span class="sxs-lookup"><span data-stu-id="00d98-141">publisher</span></span>|<span data-ttu-id="00d98-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-142">String</span></span>|<span data-ttu-id="00d98-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00d98-143">The publisher of the app.</span></span> <span data-ttu-id="00d98-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="00d98-145">largeIcon</span></span>|[<span data-ttu-id="00d98-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="00d98-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="00d98-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="00d98-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="00d98-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00d98-149">createdDateTime</span></span>|<span data-ttu-id="00d98-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d98-150">DateTimeOffset</span></span>|<span data-ttu-id="00d98-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00d98-151">The date and time the app was created.</span></span> <span data-ttu-id="00d98-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00d98-153">lastModifiedDateTime</span></span>|<span data-ttu-id="00d98-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d98-154">DateTimeOffset</span></span>|<span data-ttu-id="00d98-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="00d98-155">The date and time the app was last modified.</span></span> <span data-ttu-id="00d98-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="00d98-157">isFeatured</span></span>|<span data-ttu-id="00d98-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="00d98-158">Boolean</span></span>|<span data-ttu-id="00d98-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="00d98-160">privacyInformationUrl</span></span>|<span data-ttu-id="00d98-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-161">String</span></span>|<span data-ttu-id="00d98-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="00d98-162">The privacy statement Url.</span></span> <span data-ttu-id="00d98-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="00d98-164">informationUrl</span></span>|<span data-ttu-id="00d98-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-165">String</span></span>|<span data-ttu-id="00d98-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="00d98-166">The more information Url.</span></span> <span data-ttu-id="00d98-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-168">owner</span><span class="sxs-lookup"><span data-stu-id="00d98-168">owner</span></span>|<span data-ttu-id="00d98-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-169">String</span></span>|<span data-ttu-id="00d98-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="00d98-170">The owner of the app.</span></span> <span data-ttu-id="00d98-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-172">developer</span><span class="sxs-lookup"><span data-stu-id="00d98-172">developer</span></span>|<span data-ttu-id="00d98-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-173">String</span></span>|<span data-ttu-id="00d98-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00d98-174">The developer of the app.</span></span> <span data-ttu-id="00d98-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-176">Observações</span><span class="sxs-lookup"><span data-stu-id="00d98-176">notes</span></span>|<span data-ttu-id="00d98-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-177">String</span></span>|<span data-ttu-id="00d98-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00d98-178">Notes for the app.</span></span> <span data-ttu-id="00d98-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="00d98-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="00d98-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="00d98-180">publishingState</span></span>|[<span data-ttu-id="00d98-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="00d98-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="00d98-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00d98-182">The publishing state for the app.</span></span> <span data-ttu-id="00d98-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="00d98-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="00d98-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00d98-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="00d98-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="00d98-185">The possible values are:</span></span>|
|<span data-ttu-id="00d98-186">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="00d98-186">usedLicenseCount</span></span>|<span data-ttu-id="00d98-187">Int32</span><span class="sxs-lookup"><span data-stu-id="00d98-187">Int32</span></span>|<span data-ttu-id="00d98-188">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="00d98-188">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="00d98-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="00d98-189">totalLicenseCount</span></span>|<span data-ttu-id="00d98-190">Int32</span><span class="sxs-lookup"><span data-stu-id="00d98-190">Int32</span></span>|<span data-ttu-id="00d98-191">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="00d98-191">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="00d98-192">productKey</span><span class="sxs-lookup"><span data-stu-id="00d98-192">productKey</span></span>|<span data-ttu-id="00d98-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-193">String</span></span>|<span data-ttu-id="00d98-194">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="00d98-194">The app product key</span></span>|
|<span data-ttu-id="00d98-195">licenseType</span><span class="sxs-lookup"><span data-stu-id="00d98-195">licenseType</span></span>|[<span data-ttu-id="00d98-196">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="00d98-196">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune_apps_microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="00d98-197">O tipo de licença de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="00d98-197">The app license type Possible values are: , .</span></span> <span data-ttu-id="00d98-198">Os valores possíveis são: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="00d98-198">The possible values are:</span></span>|
|<span data-ttu-id="00d98-199">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="00d98-199">packageIdentityName</span></span>|<span data-ttu-id="00d98-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00d98-200">String</span></span>|<span data-ttu-id="00d98-201">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="00d98-201">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="00d98-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="00d98-202">Response</span></span>
<span data-ttu-id="00d98-203">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00d98-203">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00d98-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00d98-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="00d98-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00d98-205">Request</span></span>
<span data-ttu-id="00d98-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="00d98-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 766

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
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="00d98-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="00d98-207">Response</span></span>
<span data-ttu-id="00d98-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00d98-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```



