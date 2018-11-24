# <a name="update-androidstoreapp"></a><span data-ttu-id="35025-101">Atualizar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="35025-101">Update androidStoreApp</span></span>

> <span data-ttu-id="35025-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="35025-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35025-103">Atualiza as propriedades de um objeto [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="35025-103">Update the properties of a [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35025-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35025-104">Prerequisites</span></span>
<span data-ttu-id="35025-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="35025-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="35025-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35025-107">Permission type</span></span>|<span data-ttu-id="35025-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35025-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35025-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35025-109">Delegated (work or school account)</span></span>|<span data-ttu-id="35025-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35025-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="35025-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35025-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35025-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35025-112">Not supported.</span></span>|
|<span data-ttu-id="35025-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35025-113">Application</span></span>|<span data-ttu-id="35025-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35025-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35025-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35025-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="35025-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35025-116">Request headers</span></span>
|<span data-ttu-id="35025-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35025-117">Header</span></span>|<span data-ttu-id="35025-118">Valor</span><span class="sxs-lookup"><span data-stu-id="35025-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35025-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="35025-119">Authorization</span></span>|<span data-ttu-id="35025-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35025-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35025-121">Accept</span><span class="sxs-lookup"><span data-stu-id="35025-121">Accept</span></span>|<span data-ttu-id="35025-122">application/json</span><span class="sxs-lookup"><span data-stu-id="35025-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35025-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35025-123">Request body</span></span>
<span data-ttu-id="35025-124">No corpo da solicitação, forneça uma representação JSON do objeto [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="35025-124">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>

<span data-ttu-id="35025-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="35025-125">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span></span>

|<span data-ttu-id="35025-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35025-126">Property</span></span>|<span data-ttu-id="35025-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="35025-127">Type</span></span>|<span data-ttu-id="35025-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="35025-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35025-129">id</span><span class="sxs-lookup"><span data-stu-id="35025-129">id</span></span>|<span data-ttu-id="35025-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35025-130">String</span></span>|<span data-ttu-id="35025-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="35025-131">Key of the entity.</span></span> <span data-ttu-id="35025-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-133">displayName</span><span class="sxs-lookup"><span data-stu-id="35025-133">displayName</span></span>|<span data-ttu-id="35025-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35025-134">String</span></span>|<span data-ttu-id="35025-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="35025-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="35025-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-137">description</span><span class="sxs-lookup"><span data-stu-id="35025-137">description</span></span>|<span data-ttu-id="35025-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35025-138">String</span></span>|<span data-ttu-id="35025-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="35025-139">The description of the app.</span></span> <span data-ttu-id="35025-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-141">publisher</span><span class="sxs-lookup"><span data-stu-id="35025-141">publisher</span></span>|<span data-ttu-id="35025-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35025-142">String</span></span>|<span data-ttu-id="35025-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="35025-143">The publisher of the app.</span></span> <span data-ttu-id="35025-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="35025-145">largeIcon</span></span>|[<span data-ttu-id="35025-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="35025-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="35025-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="35025-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="35025-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35025-149">createdDateTime</span></span>|<span data-ttu-id="35025-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35025-150">DateTimeOffset</span></span>|<span data-ttu-id="35025-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="35025-151">The date and time the app was created.</span></span> <span data-ttu-id="35025-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35025-153">lastModifiedDateTime</span></span>|<span data-ttu-id="35025-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35025-154">DateTimeOffset</span></span>|<span data-ttu-id="35025-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="35025-155">The date and time the app was last modified.</span></span> <span data-ttu-id="35025-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="35025-157">isFeatured</span></span>|<span data-ttu-id="35025-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="35025-158">Boolean</span></span>|<span data-ttu-id="35025-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="35025-160">privacyInformationUrl</span></span>|<span data-ttu-id="35025-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35025-161">String</span></span>|<span data-ttu-id="35025-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="35025-162">The privacy statement Url.</span></span> <span data-ttu-id="35025-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="35025-164">informationUrl</span></span>|<span data-ttu-id="35025-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35025-165">String</span></span>|<span data-ttu-id="35025-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="35025-166">The more information Url.</span></span> <span data-ttu-id="35025-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-168">owner</span><span class="sxs-lookup"><span data-stu-id="35025-168">owner</span></span>|<span data-ttu-id="35025-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35025-169">String</span></span>|<span data-ttu-id="35025-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="35025-170">The owner of the app.</span></span> <span data-ttu-id="35025-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-172">developer</span><span class="sxs-lookup"><span data-stu-id="35025-172">developer</span></span>|<span data-ttu-id="35025-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35025-173">String</span></span>|<span data-ttu-id="35025-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="35025-174">The developer of the app.</span></span> <span data-ttu-id="35025-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-176">notes</span><span class="sxs-lookup"><span data-stu-id="35025-176">notes</span></span>|<span data-ttu-id="35025-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35025-177">String</span></span>|<span data-ttu-id="35025-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="35025-178">Notes for the app.</span></span> <span data-ttu-id="35025-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35025-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="35025-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="35025-180">publishingState</span></span>|[<span data-ttu-id="35025-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="35025-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="35025-182">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="35025-182">The publishing state for the app.</span></span> <span data-ttu-id="35025-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="35025-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="35025-184">Herdada do [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35025-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="35025-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="35025-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="35025-186">packageId</span><span class="sxs-lookup"><span data-stu-id="35025-186">packageId</span></span>|<span data-ttu-id="35025-187">String</span><span class="sxs-lookup"><span data-stu-id="35025-187">String</span></span>|<span data-ttu-id="35025-188">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="35025-188">The package identifier.</span></span>|
|<span data-ttu-id="35025-189">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="35025-189">appStoreUrl</span></span>|<span data-ttu-id="35025-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35025-190">String</span></span>|<span data-ttu-id="35025-191">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="35025-191">The Android app store URL.</span></span>|
|<span data-ttu-id="35025-192">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="35025-192">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="35025-193">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="35025-193">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="35025-194">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="35025-194">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="35025-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="35025-195">Response</span></span>
<span data-ttu-id="35025-196">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune_apps_androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35025-196">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35025-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35025-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="35025-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35025-198">Request</span></span>
<span data-ttu-id="35025-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35025-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="35025-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="35025-200">Response</span></span>
<span data-ttu-id="35025-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35025-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```



