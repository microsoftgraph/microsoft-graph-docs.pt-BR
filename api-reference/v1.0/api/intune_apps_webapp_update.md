# <a name="update-webapp"></a><span data-ttu-id="04d90-101">Atualizar webApp</span><span class="sxs-lookup"><span data-stu-id="04d90-101">Update webApp</span></span>

> <span data-ttu-id="04d90-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="04d90-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04d90-103">Atualiza as propriedades de um objeto [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="04d90-103">Update the properties of a [calendar](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04d90-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04d90-104">Prerequisites</span></span>
<span data-ttu-id="04d90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="04d90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04d90-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04d90-107">Permission type</span></span>|<span data-ttu-id="04d90-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04d90-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04d90-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04d90-109">Delegated (work or school account)</span></span>|<span data-ttu-id="04d90-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04d90-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04d90-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04d90-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04d90-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04d90-112">Not supported.</span></span>|
|<span data-ttu-id="04d90-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04d90-113">Application</span></span>|<span data-ttu-id="04d90-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04d90-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04d90-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04d90-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="04d90-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04d90-116">Request headers</span></span>
|<span data-ttu-id="04d90-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04d90-117">Header</span></span>|<span data-ttu-id="04d90-118">Valor</span><span class="sxs-lookup"><span data-stu-id="04d90-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04d90-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="04d90-119">Authorization</span></span>|<span data-ttu-id="04d90-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04d90-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="04d90-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04d90-121">Accept</span></span>|<span data-ttu-id="04d90-122">application/json</span><span class="sxs-lookup"><span data-stu-id="04d90-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04d90-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04d90-123">Request body</span></span>
<span data-ttu-id="04d90-124">No corpo da solicitação, forneça uma representação JSON do objeto [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="04d90-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_webapp.md) object.</span></span>

<span data-ttu-id="04d90-125">A tabela a seguir mostra as propriedades obrigatórias ao criar o [webApp](../resources/intune_apps_webapp.md).</span><span class="sxs-lookup"><span data-stu-id="04d90-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="04d90-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04d90-126">Property</span></span>|<span data-ttu-id="04d90-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="04d90-127">Type</span></span>|<span data-ttu-id="04d90-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="04d90-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04d90-129">id</span><span class="sxs-lookup"><span data-stu-id="04d90-129">id</span></span>|<span data-ttu-id="04d90-130">String</span><span class="sxs-lookup"><span data-stu-id="04d90-130">String</span></span>|<span data-ttu-id="04d90-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="04d90-131">Key of the setting.</span></span> <span data-ttu-id="04d90-132">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-133">displayName</span><span class="sxs-lookup"><span data-stu-id="04d90-133">displayName</span></span>|<span data-ttu-id="04d90-134">String</span><span class="sxs-lookup"><span data-stu-id="04d90-134">String</span></span>|<span data-ttu-id="04d90-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="04d90-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="04d90-136">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-137">descrição</span><span class="sxs-lookup"><span data-stu-id="04d90-137">description</span></span>|<span data-ttu-id="04d90-138">String</span><span class="sxs-lookup"><span data-stu-id="04d90-138">String</span></span>|<span data-ttu-id="04d90-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04d90-139">The description of the app.</span></span> <span data-ttu-id="04d90-140">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-141">publicador</span><span class="sxs-lookup"><span data-stu-id="04d90-141">Publisher</span></span>|<span data-ttu-id="04d90-142">String</span><span class="sxs-lookup"><span data-stu-id="04d90-142">String</span></span>|<span data-ttu-id="04d90-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04d90-143">The publisher of the app.</span></span> <span data-ttu-id="04d90-144">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="04d90-145">largeIcon</span></span>|[<span data-ttu-id="04d90-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="04d90-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="04d90-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="04d90-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="04d90-148">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04d90-149">createdDateTime</span></span>|<span data-ttu-id="04d90-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04d90-150">DateTimeOffset</span></span>|<span data-ttu-id="04d90-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04d90-151">The date and time the group was created.</span></span> <span data-ttu-id="04d90-152">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04d90-153">lastModifiedDateTime</span></span>|<span data-ttu-id="04d90-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04d90-154">DateTimeOffset</span></span>|<span data-ttu-id="04d90-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="04d90-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="04d90-156">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="04d90-157">isFeatured</span></span>|<span data-ttu-id="04d90-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="04d90-158">Boolean</span></span>|<span data-ttu-id="04d90-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="04d90-160">privacyInformationUrl</span></span>|<span data-ttu-id="04d90-161">String</span><span class="sxs-lookup"><span data-stu-id="04d90-161">String</span></span>|<span data-ttu-id="04d90-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="04d90-162">The privacy statement Url.</span></span> <span data-ttu-id="04d90-163">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="04d90-164">informationUrl</span></span>|<span data-ttu-id="04d90-165">String</span><span class="sxs-lookup"><span data-stu-id="04d90-165">String</span></span>|<span data-ttu-id="04d90-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="04d90-166">The more information Url.</span></span> <span data-ttu-id="04d90-167">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-168">owner</span><span class="sxs-lookup"><span data-stu-id="04d90-168">owner</span></span>|<span data-ttu-id="04d90-169">String</span><span class="sxs-lookup"><span data-stu-id="04d90-169">String</span></span>|<span data-ttu-id="04d90-170">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="04d90-170">The owner of the app.</span></span> <span data-ttu-id="04d90-171">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-172">developer</span><span class="sxs-lookup"><span data-stu-id="04d90-172">"developer"</span></span>|<span data-ttu-id="04d90-173">String</span><span class="sxs-lookup"><span data-stu-id="04d90-173">String</span></span>|<span data-ttu-id="04d90-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04d90-174">The developer of the app.</span></span> <span data-ttu-id="04d90-175">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-176">Observações</span><span class="sxs-lookup"><span data-stu-id="04d90-176">Notes</span></span>|<span data-ttu-id="04d90-177">String</span><span class="sxs-lookup"><span data-stu-id="04d90-177">String</span></span>|<span data-ttu-id="04d90-178">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04d90-178">Notes for the app.</span></span> <span data-ttu-id="04d90-179">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04d90-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="04d90-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="04d90-180">publishingState</span></span>|<span data-ttu-id="04d90-181">String</span><span class="sxs-lookup"><span data-stu-id="04d90-181">String</span></span>|<span data-ttu-id="04d90-182">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04d90-182">The publishing state for the app.</span></span> <span data-ttu-id="04d90-183">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="04d90-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="04d90-184">Herdado de [mobileApp](../resources/intune_apps_mobileapp.md). Os possíveis valores são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="04d90-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="04d90-185">appUrl</span><span class="sxs-lookup"><span data-stu-id="04d90-185">appUrl</span></span>|<span data-ttu-id="04d90-186">String</span><span class="sxs-lookup"><span data-stu-id="04d90-186">String</span></span>|<span data-ttu-id="04d90-187">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="04d90-187">The web app URL.</span></span>|
|<span data-ttu-id="04d90-188">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="04d90-188">useManagedBrowser</span></span>|<span data-ttu-id="04d90-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="04d90-189">Boolean</span></span>|<span data-ttu-id="04d90-190">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="04d90-190">Whether or not to use managed browser.</span></span> <span data-ttu-id="04d90-191">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="04d90-191">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="04d90-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="04d90-192">Response</span></span>
<span data-ttu-id="04d90-193">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [webApp](../resources/intune_apps_webapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04d90-193">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04d90-194">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04d90-194">Example</span></span>
### <a name="request"></a><span data-ttu-id="04d90-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04d90-195">Request</span></span>
<span data-ttu-id="04d90-196">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04d90-196">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04d90-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="04d90-197">Response</span></span>
<span data-ttu-id="04d90-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04d90-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



