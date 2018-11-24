# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="40367-101">Atualizar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="40367-101">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="40367-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="40367-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40367-103">Atualizar as propriedades de um objeto [ macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="40367-103">Update the properties of a [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40367-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40367-104">Prerequisites</span></span>
<span data-ttu-id="40367-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="40367-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="40367-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40367-107">Permission type</span></span>|<span data-ttu-id="40367-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40367-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40367-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40367-109">Delegated (work or school account)</span></span>|<span data-ttu-id="40367-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40367-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40367-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40367-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40367-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40367-112">Not supported.</span></span>|
|<span data-ttu-id="40367-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40367-113">Application</span></span>|<span data-ttu-id="40367-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40367-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40367-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40367-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="40367-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40367-116">Request headers</span></span>
|<span data-ttu-id="40367-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40367-117">Header</span></span>|<span data-ttu-id="40367-118">Valor</span><span class="sxs-lookup"><span data-stu-id="40367-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40367-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="40367-119">Authorization</span></span>|<span data-ttu-id="40367-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40367-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40367-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40367-121">Accept</span></span>|<span data-ttu-id="40367-122">application/json</span><span class="sxs-lookup"><span data-stu-id="40367-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40367-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40367-123">Request body</span></span>
<span data-ttu-id="40367-124">No corpo da solicitação, forneça uma representação JSON do objeto [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="40367-124">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="40367-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="40367-125">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="40367-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40367-126">Property</span></span>|<span data-ttu-id="40367-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="40367-127">Type</span></span>|<span data-ttu-id="40367-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="40367-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40367-129">id</span><span class="sxs-lookup"><span data-stu-id="40367-129">id</span></span>|<span data-ttu-id="40367-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40367-130">String</span></span>|<span data-ttu-id="40367-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="40367-131">Key of the entity.</span></span> <span data-ttu-id="40367-132">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-133">displayName</span><span class="sxs-lookup"><span data-stu-id="40367-133">displayName</span></span>|<span data-ttu-id="40367-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40367-134">String</span></span>|<span data-ttu-id="40367-135">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="40367-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="40367-136">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-137">descrição</span><span class="sxs-lookup"><span data-stu-id="40367-137">description</span></span>|<span data-ttu-id="40367-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40367-138">String</span></span>|<span data-ttu-id="40367-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40367-139">The description of the app.</span></span> <span data-ttu-id="40367-140">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-141">publicador</span><span class="sxs-lookup"><span data-stu-id="40367-141">publisher</span></span>|<span data-ttu-id="40367-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40367-142">String</span></span>|<span data-ttu-id="40367-143">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40367-143">The publisher of the app.</span></span> <span data-ttu-id="40367-144">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="40367-145">largeIcon</span></span>|[<span data-ttu-id="40367-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="40367-146">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="40367-147">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="40367-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="40367-148">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40367-149">createdDateTime</span></span>|<span data-ttu-id="40367-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40367-150">DateTimeOffset</span></span>|<span data-ttu-id="40367-151">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40367-151">The date and time the app was created.</span></span> <span data-ttu-id="40367-152">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40367-153">lastModifiedDateTime</span></span>|<span data-ttu-id="40367-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40367-154">DateTimeOffset</span></span>|<span data-ttu-id="40367-155">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="40367-155">The date and time the app was last modified.</span></span> <span data-ttu-id="40367-156">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="40367-157">isFeatured</span></span>|<span data-ttu-id="40367-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="40367-158">Boolean</span></span>|<span data-ttu-id="40367-159">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="40367-160">privacyInformationUrl</span></span>|<span data-ttu-id="40367-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40367-161">String</span></span>|<span data-ttu-id="40367-162">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="40367-162">The privacy statement Url.</span></span> <span data-ttu-id="40367-163">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="40367-164">informationUrl</span></span>|<span data-ttu-id="40367-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40367-165">String</span></span>|<span data-ttu-id="40367-166">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="40367-166">The more information Url.</span></span> <span data-ttu-id="40367-167">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-168">owner</span><span class="sxs-lookup"><span data-stu-id="40367-168">owner</span></span>|<span data-ttu-id="40367-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40367-169">String</span></span>|<span data-ttu-id="40367-170">O proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40367-170">The owner of the app.</span></span> <span data-ttu-id="40367-171">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-172">developer</span><span class="sxs-lookup"><span data-stu-id="40367-172">developer</span></span>|<span data-ttu-id="40367-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40367-173">String</span></span>|<span data-ttu-id="40367-174">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40367-174">The developer of the app.</span></span> <span data-ttu-id="40367-175">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-176">Observações</span><span class="sxs-lookup"><span data-stu-id="40367-176">notes</span></span>|<span data-ttu-id="40367-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40367-177">String</span></span>|<span data-ttu-id="40367-178">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40367-178">Notes for the app.</span></span> <span data-ttu-id="40367-179">Herdada de [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="40367-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="40367-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="40367-180">publishingState</span></span>|[<span data-ttu-id="40367-181">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="40367-181">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="40367-182">O estado da publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40367-182">The publishing state for the app.</span></span> <span data-ttu-id="40367-183">O aplicativo não pode ser atribuído, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="40367-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="40367-184">Herdada do [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40367-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md).</span></span> <span data-ttu-id="40367-185">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="40367-185">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="40367-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="40367-186">Response</span></span>
<span data-ttu-id="40367-187">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40367-187">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune_apps_macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40367-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40367-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="40367-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40367-189">Request</span></span>
<span data-ttu-id="40367-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40367-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 584

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="40367-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="40367-191">Response</span></span>
<span data-ttu-id="40367-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40367-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "publishingState": "processing"
}
```



