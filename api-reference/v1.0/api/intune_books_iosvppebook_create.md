# <a name="create-iosvppebook"></a><span data-ttu-id="cf6e9-101">Criar iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="cf6e9-101">Create iosVppEBook</span></span>

> <span data-ttu-id="cf6e9-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf6e9-103">Cria um novo objeto [iosVppEBook](../resources/intune_books_iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="cf6e9-103">Create a new [iosVppEBook](../resources/intune_books_iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf6e9-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf6e9-104">Prerequisites</span></span>
<span data-ttu-id="cf6e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf6e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf6e9-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf6e9-107">Permission type</span></span>|<span data-ttu-id="cf6e9-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf6e9-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cf6e9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf6e9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cf6e9-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf6e9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-112">Not supported.</span></span>|
|<span data-ttu-id="cf6e9-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf6e9-113">Application</span></span>|<span data-ttu-id="cf6e9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf6e9-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf6e9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="cf6e9-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf6e9-116">Request headers</span></span>
|<span data-ttu-id="cf6e9-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf6e9-117">Header</span></span>|<span data-ttu-id="cf6e9-118">Valor</span><span class="sxs-lookup"><span data-stu-id="cf6e9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf6e9-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf6e9-119">Authorization</span></span>|<span data-ttu-id="cf6e9-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf6e9-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf6e9-121">Accept</span></span>|<span data-ttu-id="cf6e9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cf6e9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf6e9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf6e9-123">Request body</span></span>
<span data-ttu-id="cf6e9-124">No corpo da solicitação, forneça uma representação JSON do objeto iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-124">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="cf6e9-125">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-125">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="cf6e9-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf6e9-126">Property</span></span>|<span data-ttu-id="cf6e9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf6e9-127">Type</span></span>|<span data-ttu-id="cf6e9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf6e9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf6e9-129">id</span><span class="sxs-lookup"><span data-stu-id="cf6e9-129">id</span></span>|<span data-ttu-id="cf6e9-130">String</span><span class="sxs-lookup"><span data-stu-id="cf6e9-130">String</span></span>|<span data-ttu-id="cf6e9-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-131">Key of the entity.</span></span> <span data-ttu-id="cf6e9-132">Herdada de [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-132">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="cf6e9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cf6e9-133">displayName</span></span>|<span data-ttu-id="cf6e9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6e9-134">String</span></span>|<span data-ttu-id="cf6e9-135">Nome do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-135">Name of the eBook.</span></span> <span data-ttu-id="cf6e9-136">Herdada de [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-136">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="cf6e9-137">description</span><span class="sxs-lookup"><span data-stu-id="cf6e9-137">description</span></span>|<span data-ttu-id="cf6e9-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6e9-138">String</span></span>|<span data-ttu-id="cf6e9-139">Descrição.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-139">Description.</span></span> <span data-ttu-id="cf6e9-140">Herdada de [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-140">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="cf6e9-141">publisher</span><span class="sxs-lookup"><span data-stu-id="cf6e9-141">publisher</span></span>|<span data-ttu-id="cf6e9-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6e9-142">String</span></span>|<span data-ttu-id="cf6e9-143">Publicador.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-143">Publisher.</span></span> <span data-ttu-id="cf6e9-144">Herdada de [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-144">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="cf6e9-145">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf6e9-145">publishedDateTime</span></span>|<span data-ttu-id="cf6e9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf6e9-146">DateTimeOffset</span></span>|<span data-ttu-id="cf6e9-147">A data e hora em que o livro eletrônico foi publicado.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-147">The date and time when the eBook was published.</span></span> <span data-ttu-id="cf6e9-148">Herdada de [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-148">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="cf6e9-149">largeCover</span><span class="sxs-lookup"><span data-stu-id="cf6e9-149">largeCover</span></span>|[<span data-ttu-id="cf6e9-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cf6e9-150">mimeContent</span></span>](../resources/intune_books_mimecontent.md)|<span data-ttu-id="cf6e9-151">Capa do livro.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-151">Book cover.</span></span> <span data-ttu-id="cf6e9-152">Herdada de [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-152">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="cf6e9-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf6e9-153">createdDateTime</span></span>|<span data-ttu-id="cf6e9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf6e9-154">DateTimeOffset</span></span>|<span data-ttu-id="cf6e9-155">A data e hora em que o livro eletrônico foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-155">The date and time when the eBook file was created.</span></span> <span data-ttu-id="cf6e9-156">Herdada de [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-156">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="cf6e9-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf6e9-157">lastModifiedDateTime</span></span>|<span data-ttu-id="cf6e9-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf6e9-158">DateTimeOffset</span></span>|<span data-ttu-id="cf6e9-159">A data e hora da última modificação do livro eletrônico.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-159">The date and time when teh eBook was last modified.</span></span> <span data-ttu-id="cf6e9-160">Herdada de [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-160">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="cf6e9-161">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cf6e9-161">informationUrl</span></span>|<span data-ttu-id="cf6e9-162">String</span><span class="sxs-lookup"><span data-stu-id="cf6e9-162">String</span></span>|<span data-ttu-id="cf6e9-163">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-163">The more information Url.</span></span> <span data-ttu-id="cf6e9-164">Herdada de [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-164">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="cf6e9-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cf6e9-165">privacyInformationUrl</span></span>|<span data-ttu-id="cf6e9-166">String</span><span class="sxs-lookup"><span data-stu-id="cf6e9-166">String</span></span>|<span data-ttu-id="cf6e9-167">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-167">The privacy statement Url.</span></span> <span data-ttu-id="cf6e9-168">Herdada de [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cf6e9-168">Inherited from [managedEBook](../resources/intune_books_managedebook.md)</span></span>|
|<span data-ttu-id="cf6e9-169">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="cf6e9-169">vppTokenId</span></span>|<span data-ttu-id="cf6e9-170">Guid</span><span class="sxs-lookup"><span data-stu-id="cf6e9-170">Guid</span></span>|<span data-ttu-id="cf6e9-171">A ID de token Vpp.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-171">The Vpp token ID.</span></span>|
|<span data-ttu-id="cf6e9-172">appleId</span><span class="sxs-lookup"><span data-stu-id="cf6e9-172">appleId</span></span>|<span data-ttu-id="cf6e9-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6e9-173">String</span></span>|<span data-ttu-id="cf6e9-174">O Apple ID associado ao token Vpp.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-174">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="cf6e9-175">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="cf6e9-175">vppOrganizationName</span></span>|<span data-ttu-id="cf6e9-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6e9-176">String</span></span>|<span data-ttu-id="cf6e9-177">O nome da organização do token Vpp.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-177">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="cf6e9-178">genres</span><span class="sxs-lookup"><span data-stu-id="cf6e9-178">genres</span></span>|<span data-ttu-id="cf6e9-179">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6e9-179">String collection</span></span>|<span data-ttu-id="cf6e9-180">Gêneros.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-180">Genres.</span></span>|
|<span data-ttu-id="cf6e9-181">idioma</span><span class="sxs-lookup"><span data-stu-id="cf6e9-181">language</span></span>|<span data-ttu-id="cf6e9-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6e9-182">String</span></span>|<span data-ttu-id="cf6e9-183">Idioma.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-183">Language.</span></span>|
|<span data-ttu-id="cf6e9-184">seller</span><span class="sxs-lookup"><span data-stu-id="cf6e9-184">seller</span></span>|<span data-ttu-id="cf6e9-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf6e9-185">String</span></span>|<span data-ttu-id="cf6e9-186">Vendedor.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-186">Seller.</span></span>|
|<span data-ttu-id="cf6e9-187">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cf6e9-187">totalLicenseCount</span></span>|<span data-ttu-id="cf6e9-188">Int32</span><span class="sxs-lookup"><span data-stu-id="cf6e9-188">Int32</span></span>|<span data-ttu-id="cf6e9-189">Contagem total de licenças.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-189">Total license count.</span></span>|
|<span data-ttu-id="cf6e9-190">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cf6e9-190">usedLicenseCount</span></span>|<span data-ttu-id="cf6e9-191">Int32</span><span class="sxs-lookup"><span data-stu-id="cf6e9-191">Int32</span></span>|<span data-ttu-id="cf6e9-192">Contagem de licenças usadas.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-192">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="cf6e9-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf6e9-193">Response</span></span>
<span data-ttu-id="cf6e9-194">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosVppEBook](../resources/intune_books_iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-194">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune_books_iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf6e9-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf6e9-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf6e9-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf6e9-196">Request</span></span>
<span data-ttu-id="cf6e9-197">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 853

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```

### <a name="response"></a><span data-ttu-id="cf6e9-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf6e9-198">Response</span></span>
<span data-ttu-id="cf6e9-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf6e9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 961

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```



