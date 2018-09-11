# <a name="update-webapp"></a><span data-ttu-id="91ddf-101">Atualizar webApp</span><span class="sxs-lookup"><span data-stu-id="91ddf-101">Update webApp</span></span>

> <span data-ttu-id="91ddf-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="91ddf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91ddf-103">Atualiza as propriedades de um objeto [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="91ddf-103">Update the properties of a [webApp](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91ddf-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91ddf-104">Prerequisites</span></span>
<span data-ttu-id="91ddf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="91ddf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="91ddf-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91ddf-107">Permission type</span></span>|<span data-ttu-id="91ddf-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91ddf-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91ddf-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91ddf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="91ddf-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91ddf-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="91ddf-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91ddf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91ddf-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91ddf-112">Not supported.</span></span>|
|<span data-ttu-id="91ddf-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91ddf-113">Application</span></span>|<span data-ttu-id="91ddf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91ddf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91ddf-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91ddf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="91ddf-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91ddf-116">Request headers</span></span>
|<span data-ttu-id="91ddf-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91ddf-117">Header</span></span>|<span data-ttu-id="91ddf-118">Valor</span><span class="sxs-lookup"><span data-stu-id="91ddf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91ddf-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="91ddf-119">Authorization</span></span>|<span data-ttu-id="91ddf-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="91ddf-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91ddf-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91ddf-121">Accept</span></span>|<span data-ttu-id="91ddf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="91ddf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91ddf-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91ddf-123">Request body</span></span>
<span data-ttu-id="91ddf-124">No corpo da solicitação, forneça uma representação JSON do objeto [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="91ddf-124">In the request body, supply a JSON representation for the [webApp](../resources/intune_apps_webapp.md) object.</span></span>

<span data-ttu-id="91ddf-125">A tabela a seguir mostra as propriedades obrigatórias ao criar o [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="91ddf-125">The following table shows the properties that are required when you create the [webApp](../resources/intune_apps_webapp.md).</span></span>

|<span data-ttu-id="91ddf-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91ddf-126">Property</span></span>|<span data-ttu-id="91ddf-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="91ddf-127">Type</span></span>|<span data-ttu-id="91ddf-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="91ddf-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91ddf-129">id</span><span class="sxs-lookup"><span data-stu-id="91ddf-129">id</span></span>|<span data-ttu-id="91ddf-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ddf-130">String</span></span>|<span data-ttu-id="91ddf-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="91ddf-131">Key of the entity.</span></span> <span data-ttu-id="91ddf-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-133">displayName</span><span class="sxs-lookup"><span data-stu-id="91ddf-133">displayName</span></span>|<span data-ttu-id="91ddf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ddf-134">String</span></span>|<span data-ttu-id="91ddf-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="91ddf-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="91ddf-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-137">descrição</span><span class="sxs-lookup"><span data-stu-id="91ddf-137">description</span></span>|<span data-ttu-id="91ddf-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ddf-138">String</span></span>|<span data-ttu-id="91ddf-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91ddf-139">The description of the app.</span></span> <span data-ttu-id="91ddf-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-141">publisher</span><span class="sxs-lookup"><span data-stu-id="91ddf-141">publisher</span></span>|<span data-ttu-id="91ddf-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ddf-142">String</span></span>|<span data-ttu-id="91ddf-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91ddf-143">The publisher of the app.</span></span> <span data-ttu-id="91ddf-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="91ddf-145">largeIcon</span></span>|[<span data-ttu-id="91ddf-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="91ddf-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="91ddf-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="91ddf-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="91ddf-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91ddf-149">createdDateTime</span></span>|<span data-ttu-id="91ddf-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91ddf-150">DateTimeOffset</span></span>|<span data-ttu-id="91ddf-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91ddf-151">The date and time the app was created.</span></span> <span data-ttu-id="91ddf-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91ddf-153">lastModifiedDateTime</span></span>|<span data-ttu-id="91ddf-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91ddf-154">DateTimeOffset</span></span>|<span data-ttu-id="91ddf-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="91ddf-155">The date and time the app was last modified.</span></span> <span data-ttu-id="91ddf-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="91ddf-157">isFeatured</span></span>|<span data-ttu-id="91ddf-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="91ddf-158">Boolean</span></span>|<span data-ttu-id="91ddf-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="91ddf-160">privacyInformationUrl</span></span>|<span data-ttu-id="91ddf-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ddf-161">String</span></span>|<span data-ttu-id="91ddf-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="91ddf-162">The privacy statement Url.</span></span> <span data-ttu-id="91ddf-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="91ddf-164">informationUrl</span></span>|<span data-ttu-id="91ddf-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ddf-165">String</span></span>|<span data-ttu-id="91ddf-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="91ddf-166">The more information Url.</span></span> <span data-ttu-id="91ddf-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-168">owner</span><span class="sxs-lookup"><span data-stu-id="91ddf-168">owner</span></span>|<span data-ttu-id="91ddf-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ddf-169">String</span></span>|<span data-ttu-id="91ddf-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="91ddf-170">The owner of the app.</span></span> <span data-ttu-id="91ddf-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-172">developer</span><span class="sxs-lookup"><span data-stu-id="91ddf-172">developer</span></span>|<span data-ttu-id="91ddf-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ddf-173">String</span></span>|<span data-ttu-id="91ddf-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91ddf-174">The developer of the app.</span></span> <span data-ttu-id="91ddf-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-176">Observações</span><span class="sxs-lookup"><span data-stu-id="91ddf-176">notes</span></span>|<span data-ttu-id="91ddf-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ddf-177">String</span></span>|<span data-ttu-id="91ddf-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91ddf-178">Notes for the app.</span></span> <span data-ttu-id="91ddf-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="91ddf-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="91ddf-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="91ddf-180">publishingState</span></span>|[<span data-ttu-id="91ddf-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="91ddf-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="91ddf-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91ddf-182">The publishing state for the app.</span></span> <span data-ttu-id="91ddf-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="91ddf-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="91ddf-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="91ddf-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span> <span data-ttu-id="91ddf-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="91ddf-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="91ddf-186">appUrl</span><span class="sxs-lookup"><span data-stu-id="91ddf-186">appUrl</span></span>|<span data-ttu-id="91ddf-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91ddf-187">String</span></span>|<span data-ttu-id="91ddf-188">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="91ddf-188">The web app URL.</span></span>|
|<span data-ttu-id="91ddf-189">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="91ddf-189">useManagedBrowser</span></span>|<span data-ttu-id="91ddf-190">Booleano</span><span class="sxs-lookup"><span data-stu-id="91ddf-190">Boolean</span></span>|<span data-ttu-id="91ddf-191">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="91ddf-191">Whether or not to use managed browser.</span></span> <span data-ttu-id="91ddf-192">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="91ddf-192">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="91ddf-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="91ddf-193">Response</span></span>
<span data-ttu-id="91ddf-194">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [webApp](../resources/intune_apps_webapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91ddf-194">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91ddf-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91ddf-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="91ddf-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91ddf-196">Request</span></span>
<span data-ttu-id="91ddf-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91ddf-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 664

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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="91ddf-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="91ddf-198">Response</span></span>
<span data-ttu-id="91ddf-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91ddf-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 817

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```








