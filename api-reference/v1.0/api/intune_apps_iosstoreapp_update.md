# <a name="update-iosstoreapp"></a><span data-ttu-id="e3c82-101">Atualizar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="e3c82-101">Update iosStoreApp</span></span>

> <span data-ttu-id="e3c82-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e3c82-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3c82-103">Atualiza as propriedades de um objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3c82-103">Update the properties of a [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3c82-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3c82-104">Prerequisites</span></span>
<span data-ttu-id="e3c82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3c82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e3c82-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3c82-107">Permission type</span></span>|<span data-ttu-id="e3c82-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3c82-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3c82-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3c82-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e3c82-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3c82-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3c82-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3c82-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3c82-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3c82-112">Not supported.</span></span>|
|<span data-ttu-id="e3c82-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3c82-113">Application</span></span>|<span data-ttu-id="e3c82-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3c82-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3c82-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3c82-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="e3c82-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c82-116">Request headers</span></span>
|<span data-ttu-id="e3c82-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3c82-117">Header</span></span>|<span data-ttu-id="e3c82-118">Valor</span><span class="sxs-lookup"><span data-stu-id="e3c82-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3c82-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3c82-119">Authorization</span></span>|<span data-ttu-id="e3c82-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="e3c82-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3c82-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3c82-121">Accept</span></span>|<span data-ttu-id="e3c82-122">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="e3c82-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3c82-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c82-123">Request body</span></span>
<span data-ttu-id="e3c82-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3c82-124">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object.</span></span>

<span data-ttu-id="e3c82-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3c82-125">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span></span>

|<span data-ttu-id="e3c82-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3c82-126">Property</span></span>|<span data-ttu-id="e3c82-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3c82-127">Type</span></span>|<span data-ttu-id="e3c82-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3c82-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3c82-129">id</span><span class="sxs-lookup"><span data-stu-id="e3c82-129">id</span></span>|<span data-ttu-id="e3c82-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-130">String</span></span>|<span data-ttu-id="e3c82-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e3c82-131">Key of the entity.</span></span> <span data-ttu-id="e3c82-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e3c82-133">displayName</span></span>|<span data-ttu-id="e3c82-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-134">String</span></span>|<span data-ttu-id="e3c82-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e3c82-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e3c82-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-137">description</span><span class="sxs-lookup"><span data-stu-id="e3c82-137">description</span></span>|<span data-ttu-id="e3c82-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-138">String</span></span>|<span data-ttu-id="e3c82-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3c82-139">The description of the app.</span></span> <span data-ttu-id="e3c82-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-141">publisher</span><span class="sxs-lookup"><span data-stu-id="e3c82-141">publisher</span></span>|<span data-ttu-id="e3c82-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-142">String</span></span>|<span data-ttu-id="e3c82-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3c82-143">The publisher of the app.</span></span> <span data-ttu-id="e3c82-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e3c82-145">largeIcon</span></span>|[<span data-ttu-id="e3c82-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3c82-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="e3c82-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e3c82-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e3c82-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3c82-149">createdDateTime</span></span>|<span data-ttu-id="e3c82-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c82-150">DateTimeOffset</span></span>|<span data-ttu-id="e3c82-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3c82-151">The date and time the app was created.</span></span> <span data-ttu-id="e3c82-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3c82-153">lastModifiedDateTime</span></span>|<span data-ttu-id="e3c82-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c82-154">DateTimeOffset</span></span>|<span data-ttu-id="e3c82-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e3c82-155">The date and time the app was last modified.</span></span> <span data-ttu-id="e3c82-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e3c82-157">isFeatured</span></span>|<span data-ttu-id="e3c82-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="e3c82-158">Boolean</span></span>|<span data-ttu-id="e3c82-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e3c82-160">privacyInformationUrl</span></span>|<span data-ttu-id="e3c82-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-161">String</span></span>|<span data-ttu-id="e3c82-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e3c82-162">The privacy statement Url.</span></span> <span data-ttu-id="e3c82-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e3c82-164">informationUrl</span></span>|<span data-ttu-id="e3c82-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-165">String</span></span>|<span data-ttu-id="e3c82-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e3c82-166">The more information Url.</span></span> <span data-ttu-id="e3c82-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-168">owner</span><span class="sxs-lookup"><span data-stu-id="e3c82-168">owner</span></span>|<span data-ttu-id="e3c82-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-169">String</span></span>|<span data-ttu-id="e3c82-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e3c82-170">The owner of the app.</span></span> <span data-ttu-id="e3c82-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-172">developer</span><span class="sxs-lookup"><span data-stu-id="e3c82-172">developer</span></span>|<span data-ttu-id="e3c82-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-173">String</span></span>|<span data-ttu-id="e3c82-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3c82-174">The developer of the app.</span></span> <span data-ttu-id="e3c82-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-176">Observações</span><span class="sxs-lookup"><span data-stu-id="e3c82-176">notes</span></span>|<span data-ttu-id="e3c82-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-177">String</span></span>|<span data-ttu-id="e3c82-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3c82-178">Notes for the app.</span></span> <span data-ttu-id="e3c82-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3c82-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="e3c82-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="e3c82-180">publishingState</span></span>|[<span data-ttu-id="e3c82-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e3c82-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="e3c82-p114">O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos que esteja publicado. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e3c82-p114">The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md). The possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e3c82-186">bundleId</span><span class="sxs-lookup"><span data-stu-id="e3c82-186">bundleId</span></span>|<span data-ttu-id="e3c82-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-187">String</span></span>|<span data-ttu-id="e3c82-188">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e3c82-188">The Identity Name.</span></span>|
|<span data-ttu-id="e3c82-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e3c82-189">appStoreUrl</span></span>|<span data-ttu-id="e3c82-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3c82-190">String</span></span>|<span data-ttu-id="e3c82-191">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="e3c82-191">The Apple App Store URL</span></span>|
|<span data-ttu-id="e3c82-192">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="e3c82-192">applicableDeviceType</span></span>|[<span data-ttu-id="e3c82-193">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e3c82-193">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="e3c82-194">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="e3c82-194">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="e3c82-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e3c82-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e3c82-196">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e3c82-196">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="e3c82-197">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="e3c82-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="e3c82-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3c82-198">Response</span></span>
<span data-ttu-id="e3c82-199">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3c82-199">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune_apps_iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3c82-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3c82-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3c82-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c82-201">Request</span></span>
<span data-ttu-id="e3c82-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3c82-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1000

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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="e3c82-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3c82-203">Response</span></span>
<span data-ttu-id="e3c82-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3c82-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1158

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```








