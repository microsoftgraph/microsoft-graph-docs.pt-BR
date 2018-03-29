# <a name="update-iosstoreapp"></a><span data-ttu-id="7e9f5-101">Atualizar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="7e9f5-101">Update iosStoreApp</span></span>

> <span data-ttu-id="7e9f5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e9f5-103">Atualiza as propriedades de um objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e9f5-103">Update the properties of a [calendar](../resources/intune_apps_iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e9f5-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7e9f5-104">Prerequisites</span></span>
<span data-ttu-id="7e9f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e9f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7e9f5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e9f5-107">Permission type</span></span>|<span data-ttu-id="7e9f5-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e9f5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7e9f5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e9f5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e9f5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e9f5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-112">Not supported.</span></span>|
|<span data-ttu-id="7e9f5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e9f5-113">Application</span></span>|<span data-ttu-id="7e9f5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e9f5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e9f5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="7e9f5-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9f5-116">Request headers</span></span>
|<span data-ttu-id="7e9f5-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e9f5-117">Header</span></span>|<span data-ttu-id="7e9f5-118">Valor</span><span class="sxs-lookup"><span data-stu-id="7e9f5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e9f5-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e9f5-119">Authorization</span></span>|<span data-ttu-id="7e9f5-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7e9f5-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e9f5-121">Accept</span></span>|<span data-ttu-id="7e9f5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7e9f5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e9f5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9f5-123">Request body</span></span>
<span data-ttu-id="7e9f5-124">No corpo da solicitação, forneça uma representação JSON do objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e9f5-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_iosstoreapp.md) object.</span></span>

<span data-ttu-id="7e9f5-125">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e9f5-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="7e9f5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e9f5-126">Property</span></span>|<span data-ttu-id="7e9f5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e9f5-127">Type</span></span>|<span data-ttu-id="7e9f5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e9f5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e9f5-129">id</span><span class="sxs-lookup"><span data-stu-id="7e9f5-129">id</span></span>|<span data-ttu-id="7e9f5-130">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-130">String</span></span>|<span data-ttu-id="7e9f5-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-131">Key of the setting.</span></span> <span data-ttu-id="7e9f5-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7e9f5-133">displayName</span></span>|<span data-ttu-id="7e9f5-134">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-134">String</span></span>|<span data-ttu-id="7e9f5-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7e9f5-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-137">descrição</span><span class="sxs-lookup"><span data-stu-id="7e9f5-137">description</span></span>|<span data-ttu-id="7e9f5-138">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-138">String</span></span>|<span data-ttu-id="7e9f5-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-139">The description of the app.</span></span> <span data-ttu-id="7e9f5-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-141">publicador</span><span class="sxs-lookup"><span data-stu-id="7e9f5-141">Publisher</span></span>|<span data-ttu-id="7e9f5-142">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-142">String</span></span>|<span data-ttu-id="7e9f5-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-143">The publisher of the app.</span></span> <span data-ttu-id="7e9f5-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7e9f5-145">largeIcon</span></span>|[<span data-ttu-id="7e9f5-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7e9f5-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="7e9f5-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7e9f5-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e9f5-149">createdDateTime</span></span>|<span data-ttu-id="7e9f5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e9f5-150">DateTimeOffset</span></span>|<span data-ttu-id="7e9f5-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-151">The date and time the group was created.</span></span> <span data-ttu-id="7e9f5-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e9f5-153">lastModifiedDateTime</span></span>|<span data-ttu-id="7e9f5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e9f5-154">DateTimeOffset</span></span>|<span data-ttu-id="7e9f5-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="7e9f5-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7e9f5-157">isFeatured</span></span>|<span data-ttu-id="7e9f5-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e9f5-158">Boolean</span></span>|<span data-ttu-id="7e9f5-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7e9f5-160">privacyInformationUrl</span></span>|<span data-ttu-id="7e9f5-161">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-161">String</span></span>|<span data-ttu-id="7e9f5-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-162">The privacy statement Url.</span></span> <span data-ttu-id="7e9f5-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7e9f5-164">informationUrl</span></span>|<span data-ttu-id="7e9f5-165">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-165">String</span></span>|<span data-ttu-id="7e9f5-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-166">The more information Url.</span></span> <span data-ttu-id="7e9f5-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-168">owner</span><span class="sxs-lookup"><span data-stu-id="7e9f5-168">owner</span></span>|<span data-ttu-id="7e9f5-169">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-169">String</span></span>|<span data-ttu-id="7e9f5-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-170">The owner of the app.</span></span> <span data-ttu-id="7e9f5-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-172">developer</span><span class="sxs-lookup"><span data-stu-id="7e9f5-172">"developer"</span></span>|<span data-ttu-id="7e9f5-173">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-173">String</span></span>|<span data-ttu-id="7e9f5-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-174">The developer of the app.</span></span> <span data-ttu-id="7e9f5-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-176">Observações</span><span class="sxs-lookup"><span data-stu-id="7e9f5-176">Notes</span></span>|<span data-ttu-id="7e9f5-177">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-177">String</span></span>|<span data-ttu-id="7e9f5-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-178">Notes for the app.</span></span> <span data-ttu-id="7e9f5-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7e9f5-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="7e9f5-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="7e9f5-180">publishingState</span></span>|<span data-ttu-id="7e9f5-181">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-181">String</span></span>|<span data-ttu-id="7e9f5-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-182">The publishing state for the app.</span></span> <span data-ttu-id="7e9f5-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7e9f5-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7e9f5-185">bundleId</span><span class="sxs-lookup"><span data-stu-id="7e9f5-185">bundleId</span></span>|<span data-ttu-id="7e9f5-186">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-186">String</span></span>|<span data-ttu-id="7e9f5-187">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-187">The Identity Name.</span></span>|
|<span data-ttu-id="7e9f5-188">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7e9f5-188">appStoreUrl</span></span>|<span data-ttu-id="7e9f5-189">String</span><span class="sxs-lookup"><span data-stu-id="7e9f5-189">String</span></span>|<span data-ttu-id="7e9f5-190">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="7e9f5-190">The Apple App Store URL</span></span>|
|<span data-ttu-id="7e9f5-191">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="7e9f5-191">applicableDeviceType</span></span>|[<span data-ttu-id="7e9f5-192">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="7e9f5-192">iosDeviceType</span></span>](../resources/intune_apps_iosdevicetype.md)|<span data-ttu-id="7e9f5-193">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-193">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="7e9f5-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7e9f5-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7e9f5-195">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7e9f5-195">iosMinimumOperatingSystem</span></span>](../resources/intune_apps_iosminimumoperatingsystem.md)|<span data-ttu-id="7e9f5-196">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="7e9f5-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e9f5-197">Response</span></span>
<span data-ttu-id="7e9f5-198">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosStoreApp](../resources/intune_apps_iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-198">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e9f5-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e9f5-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e9f5-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9f5-200">Request</span></span>
<span data-ttu-id="7e9f5-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7e9f5-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e9f5-202">Response</span></span>
<span data-ttu-id="7e9f5-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e9f5-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



