# <a name="create-androidstoreapp"></a><span data-ttu-id="1b1bc-101">Criar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="1b1bc-101">Create androidStoreApp</span></span>

> <span data-ttu-id="1b1bc-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b1bc-103">Criar um novo objeto [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b1bc-103">Create a new [plannerBucket](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b1bc-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b1bc-104">Prerequisites</span></span>
<span data-ttu-id="1b1bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b1bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1b1bc-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b1bc-107">Permission type</span></span>|<span data-ttu-id="1b1bc-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b1bc-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1b1bc-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b1bc-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b1bc-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b1bc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-112">Not supported.</span></span>|
|<span data-ttu-id="1b1bc-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b1bc-113">Application</span></span>|<span data-ttu-id="1b1bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b1bc-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b1bc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1b1bc-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b1bc-116">Request headers</span></span>
|<span data-ttu-id="1b1bc-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b1bc-117">Header</span></span>|<span data-ttu-id="1b1bc-118">Valor</span><span class="sxs-lookup"><span data-stu-id="1b1bc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b1bc-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b1bc-119">Authorization</span></span>|<span data-ttu-id="1b1bc-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1b1bc-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1b1bc-121">Accept</span></span>|<span data-ttu-id="1b1bc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1b1bc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b1bc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b1bc-123">Request body</span></span>
<span data-ttu-id="1b1bc-124">No corpo da solicitação, forneça uma representação JSON do objeto androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="1b1bc-125">A tabela a seguir mostra as propriedades que são necessárias ao criar androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="1b1bc-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b1bc-126">Property</span></span>|<span data-ttu-id="1b1bc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b1bc-127">Type</span></span>|<span data-ttu-id="1b1bc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b1bc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b1bc-129">id</span><span class="sxs-lookup"><span data-stu-id="1b1bc-129">id</span></span>|<span data-ttu-id="1b1bc-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-130">String</span></span>|<span data-ttu-id="1b1bc-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-131">Key of the setting.</span></span> <span data-ttu-id="1b1bc-132">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1b1bc-133">displayName</span></span>|<span data-ttu-id="1b1bc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-134">String</span></span>|<span data-ttu-id="1b1bc-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1b1bc-136">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-137">descrição</span><span class="sxs-lookup"><span data-stu-id="1b1bc-137">description</span></span>|<span data-ttu-id="1b1bc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-138">String</span></span>|<span data-ttu-id="1b1bc-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-139">The description of the app.</span></span> <span data-ttu-id="1b1bc-140">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-141">publicador</span><span class="sxs-lookup"><span data-stu-id="1b1bc-141">Publisher</span></span>|<span data-ttu-id="1b1bc-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-142">String</span></span>|<span data-ttu-id="1b1bc-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-143">The publisher of the app.</span></span> <span data-ttu-id="1b1bc-144">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1b1bc-145">largeIcon</span></span>|[<span data-ttu-id="1b1bc-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1b1bc-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="1b1bc-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1b1bc-148">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b1bc-149">createdDateTime</span></span>|<span data-ttu-id="1b1bc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b1bc-150">DateTimeOffset</span></span>|<span data-ttu-id="1b1bc-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-151">The date and time the group was created.</span></span> <span data-ttu-id="1b1bc-152">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b1bc-153">lastModifiedDateTime</span></span>|<span data-ttu-id="1b1bc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b1bc-154">DateTimeOffset</span></span>|<span data-ttu-id="1b1bc-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="1b1bc-156">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1b1bc-157">isFeatured</span></span>|<span data-ttu-id="1b1bc-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b1bc-158">Boolean</span></span>|<span data-ttu-id="1b1bc-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1b1bc-160">privacyInformationUrl</span></span>|<span data-ttu-id="1b1bc-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-161">String</span></span>|<span data-ttu-id="1b1bc-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-162">The privacy statement Url.</span></span> <span data-ttu-id="1b1bc-163">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1b1bc-164">informationUrl</span></span>|<span data-ttu-id="1b1bc-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-165">String</span></span>|<span data-ttu-id="1b1bc-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-166">The more information Url.</span></span> <span data-ttu-id="1b1bc-167">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-168">owner</span><span class="sxs-lookup"><span data-stu-id="1b1bc-168">owner</span></span>|<span data-ttu-id="1b1bc-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-169">String</span></span>|<span data-ttu-id="1b1bc-170">O proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-170">The owner of the app.</span></span> <span data-ttu-id="1b1bc-171">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-172">developer</span><span class="sxs-lookup"><span data-stu-id="1b1bc-172">"developer"</span></span>|<span data-ttu-id="1b1bc-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-173">String</span></span>|<span data-ttu-id="1b1bc-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-174">The developer of the app.</span></span> <span data-ttu-id="1b1bc-175">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-176">Observações</span><span class="sxs-lookup"><span data-stu-id="1b1bc-176">Notes</span></span>|<span data-ttu-id="1b1bc-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-177">String</span></span>|<span data-ttu-id="1b1bc-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-178">Notes for the app.</span></span> <span data-ttu-id="1b1bc-179">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b1bc-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="1b1bc-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="1b1bc-180">publishingState</span></span>|<span data-ttu-id="1b1bc-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-181">String</span></span>|<span data-ttu-id="1b1bc-182">O estado da publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-182">The publishing state for the app.</span></span> <span data-ttu-id="1b1bc-183">O aplicativo não pode ser atribuído, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1b1bc-184">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1b1bc-185">packageId</span><span class="sxs-lookup"><span data-stu-id="1b1bc-185">packageId</span></span>|<span data-ttu-id="1b1bc-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-186">String</span></span>|<span data-ttu-id="1b1bc-187">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-187">The package identifier.</span></span>|
|<span data-ttu-id="1b1bc-188">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1b1bc-188">appStoreUrl</span></span>|<span data-ttu-id="1b1bc-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1bc-189">String</span></span>|<span data-ttu-id="1b1bc-190">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-190">The Android app store URL.</span></span>|
|<span data-ttu-id="1b1bc-191">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1b1bc-191">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1b1bc-192">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1b1bc-192">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="1b1bc-193">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-193">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="1b1bc-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b1bc-194">Response</span></span>
<span data-ttu-id="1b1bc-195">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidStoreApp](../resources/intune_apps_androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-195">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b1bc-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b1bc-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b1bc-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b1bc-197">Request</span></span>
<span data-ttu-id="1b1bc-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1002

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

### <a name="response"></a><span data-ttu-id="1b1bc-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b1bc-199">Response</span></span>
<span data-ttu-id="1b1bc-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b1bc-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



