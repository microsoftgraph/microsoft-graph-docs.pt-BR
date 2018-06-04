# <a name="error-codes-for-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="feb5d-101">Códigos de erro para APIs do OneNote no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="feb5d-101">Error codes for OneNote APIs in Microsoft Graph</span></span>

<span data-ttu-id="feb5d-102">Este artigo descreve os códigos de erro que são retornados pelas APIs do OneNote no Microsoft Graph sempre que uma solicitação enviada pela API falha.</span><span class="sxs-lookup"><span data-stu-id="feb5d-102">This article describes error codes that are returned by the OneNote APIs in Microsoft Graph whenever a request sent through the API fails.</span></span>

## <a name="error-response-example"></a><span data-ttu-id="feb5d-103">Exemplo de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="feb5d-103">Error response example</span></span>
<span data-ttu-id="feb5d-104">Quando sua solicitação gera um erro, a API do OneNote para de executar a solicitação e retorna uma resposta de erro como um objeto JSON.</span><span class="sxs-lookup"><span data-stu-id="feb5d-104">When your request generates an error, the OneNote API stops performing the request and returns an error response as a JSON object.</span></span> <span data-ttu-id="feb5d-105">Uma resposta de erro contém o código de erro associado, uma mensagem e um link para a seção apropriada deste artigo.</span><span class="sxs-lookup"><span data-stu-id="feb5d-105">An error response contains the associated error code, a message, and a link to the appropriate section of this article.</span></span> <span data-ttu-id="feb5d-106">O exemplo a seguir mostra como é uma resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="feb5d-106">The following example shows how an error response looks.</span></span>

```json
{
   "error":{
      "code":"10002",
      "message":"The service is currently unavailable. Please try again later.",
      "innerError": {
        "requestId": "request-id",
        "date": "date-time"
      }
   }
}
```

<span data-ttu-id="feb5d-107">Para saber mais sobre erros do Microsoft Graph, confira [Respostas de erros e tipos de recurso do Microsoft Graph](errors.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-107">For more information about Microsoft Graph errors, see [Microsoft Graph error responses and resource types](errors.md).</span></span>

## <a name="codes-from-10001-to-19999"></a><span data-ttu-id="feb5d-108">Códigos de 10001 às 19999</span><span class="sxs-lookup"><span data-stu-id="feb5d-108">Codes from 10001 to 19999</span></span>
<span data-ttu-id="feb5d-109">O serviço está tendo problemas ou está enviando informações ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="feb5d-109">The service is having problems or is sending information to the application.</span></span>

### <a name="10001"></a><span data-ttu-id="feb5d-110">10001</span><span class="sxs-lookup"><span data-stu-id="feb5d-110">10001</span></span>
<span data-ttu-id="feb5d-111">Ocorreu um erro inesperado e a solicitação falhou.</span><span class="sxs-lookup"><span data-stu-id="feb5d-111">An unexpected error occurred and the request failed.</span></span>

### <a name="10002"></a><span data-ttu-id="feb5d-112">10002</span><span class="sxs-lookup"><span data-stu-id="feb5d-112">10002</span></span>
<span data-ttu-id="feb5d-113">O serviço não está disponível no momento.</span><span class="sxs-lookup"><span data-stu-id="feb5d-113">The service is not currently available.</span></span>

### <a name="10003"></a><span data-ttu-id="feb5d-114">10003</span><span class="sxs-lookup"><span data-stu-id="feb5d-114">10003</span></span>
<span data-ttu-id="feb5d-115">A conta do usuário atual excedeu o número máximo de solicitações ativas.</span><span class="sxs-lookup"><span data-stu-id="feb5d-115">The current user's account has exceeded the maximum number of active requests.</span></span> <span data-ttu-id="feb5d-116">Seu aplicativo terá que repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-116">Your app will have to repeat the request.</span></span>

### <a name="10004"></a><span data-ttu-id="feb5d-117">10004</span><span class="sxs-lookup"><span data-stu-id="feb5d-117">10004</span></span>
<span data-ttu-id="feb5d-118">O serviço não pode criar uma página na seção solicitada porque essa seção é protegida por uma senha.</span><span class="sxs-lookup"><span data-stu-id="feb5d-118">The service can't create a page in the requested section because that section is protected by a password.</span></span>

### <a name="10005"></a><span data-ttu-id="feb5d-119">10005</span><span class="sxs-lookup"><span data-stu-id="feb5d-119">10005</span></span>
<span data-ttu-id="feb5d-120">A solicitação contém mais do que o número máximo de marcas de imagem nas quais o atributo **data-render-src** contém um PDF.</span><span class="sxs-lookup"><span data-stu-id="feb5d-120">The request contains more than the maximum number of image tags in which the **data-render-src** attribute contains a PDF.</span></span> <span data-ttu-id="feb5d-121">Confira [Adicionar imagens e arquivos](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-images-files).</span><span class="sxs-lookup"><span data-stu-id="feb5d-121">See [Add images and files](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-images-files).</span></span>

### <a name="10006"></a><span data-ttu-id="feb5d-122">10006</span><span class="sxs-lookup"><span data-stu-id="feb5d-122">10006</span></span>
<span data-ttu-id="feb5d-123">A API do OneNote não pôde criar uma página na seção especificada porque a seção está corrompida.</span><span class="sxs-lookup"><span data-stu-id="feb5d-123">The OneNote API was unable to create a page in the specified section because that section is corrupt.</span></span>

### <a name="10007"></a><span data-ttu-id="feb5d-124">10007</span><span class="sxs-lookup"><span data-stu-id="feb5d-124">10007</span></span>
<span data-ttu-id="feb5d-125">O servidor está ocupado demais para lidar com a solicitação de entrada neste momento.</span><span class="sxs-lookup"><span data-stu-id="feb5d-125">The server is too busy to handle the incoming request at this moment.</span></span> <span data-ttu-id="feb5d-126">Tente novamente mais tarde.</span><span class="sxs-lookup"><span data-stu-id="feb5d-126">Please try again later.</span></span>

### <a name="10008"></a><span data-ttu-id="feb5d-127">10008</span><span class="sxs-lookup"><span data-stu-id="feb5d-127">10008</span></span>
<span data-ttu-id="feb5d-128">Uma ou mais das bibliotecas de documentos no OneDrive do usuário ou grupo contêm mais de 5.000 itens do OneNote (bloco de anotações, seções, grupos de seções) e não podem ser consultadas usando a API.</span><span class="sxs-lookup"><span data-stu-id="feb5d-128">One or more of the document libraries on the user or group's OneDrive contains more than 5000 OneNote items (notebooks, sections, section groups), and cannot be queried using the API.</span></span> <span data-ttu-id="feb5d-129">Certifique-se de que nenhuma das bibliotecas de documentos do grupo ou usuário contenha mais de 5000 itens do OneNote.</span><span class="sxs-lookup"><span data-stu-id="feb5d-129">Please make sure that none of the user or group's document libraries contains more than 5000 OneNote items.</span></span> <span data-ttu-id="feb5d-130">Confira o [blog de desenvolvimento do OneNote](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) para ver as etapas de mitigação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-130">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10012"></a><span data-ttu-id="feb5d-131">10012</span><span class="sxs-lookup"><span data-stu-id="feb5d-131">10012</span></span>
<span data-ttu-id="feb5d-132">Não é possível criar nem atualizar a entidade porque a biblioteca que contém o bloco de anotações exige que seja feito check-out dos itens para que eles possam ser editados.</span><span class="sxs-lookup"><span data-stu-id="feb5d-132">Unable to create or update the entity because the library that contains the notebook requires items to be checked out before they can be edited.</span></span> <span data-ttu-id="feb5d-133">Para saber mais, consulte https://support.office.com/en-us/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7.</span><span class="sxs-lookup"><span data-stu-id="feb5d-133">For more information, see</span></span>

<span data-ttu-id="feb5d-134">Remova o requisito de check-out da biblioteca ou mova o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="feb5d-134">Either remove the check-out requirement from the library, or move the notebook.</span></span>

### <a name="10013"></a><span data-ttu-id="feb5d-135">10013</span><span class="sxs-lookup"><span data-stu-id="feb5d-135">10013</span></span>
<span data-ttu-id="feb5d-136">Uma ou mais das bibliotecas de documentos no OneDrive do usuário ou grupo contêm mais de 20.000 itens e não podem ser indexadas para consulta usando a API.</span><span class="sxs-lookup"><span data-stu-id="feb5d-136">One or more of the document libraries on the user or group's OneDrive contains more than 20,000 items and cannot be indexed for querying using the API.</span></span> <span data-ttu-id="feb5d-137">Certifique-se de que nenhuma das bibliotecas de documentos do grupo ou usuário contenha mais de 20.000 itens.</span><span class="sxs-lookup"><span data-stu-id="feb5d-137">Please make sure that none of the user or group's document libraries contains more than 20,000 items.</span></span> <span data-ttu-id="feb5d-138">Confira o [blog de desenvolvimento do OneNote](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) para ver as etapas de mitigação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-138">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10014"></a><span data-ttu-id="feb5d-139">10014</span><span class="sxs-lookup"><span data-stu-id="feb5d-139">10014</span></span>
<span data-ttu-id="feb5d-140">O Azure Key Vault está ocupado demais para lidar com a solicitação de entrada neste momento.</span><span class="sxs-lookup"><span data-stu-id="feb5d-140">Azure Key Vault is too busy to handle the incoming request at this moment.</span></span> <span data-ttu-id="feb5d-141">Tente novamente mais tarde.</span><span class="sxs-lookup"><span data-stu-id="feb5d-141">Please try again later.</span></span>

### <a name="10015"></a><span data-ttu-id="feb5d-142">10015</span><span class="sxs-lookup"><span data-stu-id="feb5d-142">10015</span></span>
<span data-ttu-id="feb5d-143">O SharePoint atualmente não está disponível.</span><span class="sxs-lookup"><span data-stu-id="feb5d-143">SharePoint is currently unavailable.</span></span> <span data-ttu-id="feb5d-144">Tente novamente mais tarde.</span><span class="sxs-lookup"><span data-stu-id="feb5d-144">Please try again later.</span></span>

### <a name="10016"></a><span data-ttu-id="feb5d-145">10016</span><span class="sxs-lookup"><span data-stu-id="feb5d-145">10016</span></span>
<span data-ttu-id="feb5d-146">A biblioteca de documentos no OneDrive do usuário ou grupo excedeu o limite dos escopos exclusivos de segurança.</span><span class="sxs-lookup"><span data-stu-id="feb5d-146">Document library on the user or group’s OneDrive exceeded unique security scopes threshold limit.</span></span> <span data-ttu-id="feb5d-147">O número máximo de escopos exclusivos de segurança definido para uma biblioteca não pode exceder 50.000.</span><span class="sxs-lookup"><span data-stu-id="feb5d-147">The maximum number of unique security scopes set for a library cannot exceed 50,000.</span></span>

### <a name="10017"></a><span data-ttu-id="feb5d-148">10017</span><span class="sxs-lookup"><span data-stu-id="feb5d-148">10017</span></span>
<span data-ttu-id="feb5d-149">Solicitação Incorreta.</span><span class="sxs-lookup"><span data-stu-id="feb5d-149">Bad Request.</span></span>

### <a name="19999"></a><span data-ttu-id="feb5d-150">19999</span><span class="sxs-lookup"><span data-stu-id="feb5d-150">19999</span></span>
<span data-ttu-id="feb5d-151">A solicitação falhou porque ocorreu um erro indeterminado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-151">The request failed because an undetermined error occurred.</span></span>

## <a name="codes-from-20001-to-29999"></a><span data-ttu-id="feb5d-152">Códigos de 20001 às 29999</span><span class="sxs-lookup"><span data-stu-id="feb5d-152">Codes from 20001 to 29999</span></span>
<span data-ttu-id="feb5d-153">O código do aplicativo fez algo errado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-153">The application code has done something wrong.</span></span>

### <a name="20001"></a><span data-ttu-id="feb5d-154">20001</span><span class="sxs-lookup"><span data-stu-id="feb5d-154">20001</span></span>

<span data-ttu-id="feb5d-155">A parte "Apresentação" necessária está faltando na solicitação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-155">The request is missing the required "Presentation" part.</span></span> <span data-ttu-id="feb5d-156">Exatamente uma é necessária.</span><span class="sxs-lookup"><span data-stu-id="feb5d-156">Exactly one is required.</span></span> 

### <a name="20002"></a><span data-ttu-id="feb5d-157">20002</span><span class="sxs-lookup"><span data-stu-id="feb5d-157">20002</span></span>
<span data-ttu-id="feb5d-158">A solicitação contém duas ou mais partes de "Apresentação".</span><span class="sxs-lookup"><span data-stu-id="feb5d-158">The request contains two or more "Presentation" parts.</span></span> <span data-ttu-id="feb5d-159">Exatamente uma é necessária.</span><span class="sxs-lookup"><span data-stu-id="feb5d-159">Exactly one is required.</span></span>

### <a name="20003"></a><span data-ttu-id="feb5d-160">20003</span><span class="sxs-lookup"><span data-stu-id="feb5d-160">20003</span></span>
<span data-ttu-id="feb5d-161">O tipo de conteúdo da parte "Apresentação" pode ser somente texto/HTML ou aplicativo/XHTML+XML.</span><span class="sxs-lookup"><span data-stu-id="feb5d-161">The content type of the "Presentation" part can be only text/HTML or application/XHTML+XML.</span></span> 

### <a name="20004"></a><span data-ttu-id="feb5d-162">20004</span><span class="sxs-lookup"><span data-stu-id="feb5d-162">20004</span></span>
<span data-ttu-id="feb5d-163">O HTML da parte "Apresentação" contém uma marca de imagem com a **src** e o conjunto de propriedades **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="feb5d-163">The "Presentation" part HTML contains an image tag with both the **src** and the **data-render-src** properties set.</span></span> <span data-ttu-id="feb5d-164">A API vai ignorar a propriedade **src** e o uso da propriedade **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="feb5d-164">The API will ignore the **src** property and use the **data-render-src** property.</span></span> 

### <a name="20005"></a><span data-ttu-id="feb5d-165">20005</span><span class="sxs-lookup"><span data-stu-id="feb5d-165">20005</span></span>
<span data-ttu-id="feb5d-166">O URI da solicitação é muito longo.</span><span class="sxs-lookup"><span data-stu-id="feb5d-166">The request URI is too long.</span></span> <span data-ttu-id="feb5d-167">O tamanho máximo do URI (incluindo todos os parâmetros e dados) é de 16 KB ou 16.384 caracteres.</span><span class="sxs-lookup"><span data-stu-id="feb5d-167">The maximum size of the URI (including all parameters and data) is 16 KB or 16,384 characters.</span></span>

### <a name="20006"></a><span data-ttu-id="feb5d-168">20006</span><span class="sxs-lookup"><span data-stu-id="feb5d-168">20006</span></span>
<span data-ttu-id="feb5d-169">O HTML da parte "Apresentação" contém uma marca de imagem sem a src, nem o conjunto de propriedades **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="feb5d-169">The "Presentation" part HTML contains an image tag with neither the src nor the **data-render-src** properties set.</span></span> <span data-ttu-id="feb5d-170">A API vai ignorar a marca **image**.</span><span class="sxs-lookup"><span data-stu-id="feb5d-170">The API will ignore the **image** tag.</span></span> 

### <a name="20007"></a><span data-ttu-id="feb5d-171">20007</span><span class="sxs-lookup"><span data-stu-id="feb5d-171">20007</span></span>
<span data-ttu-id="feb5d-172">O HTML da parte "Apresentação" contém uma cadeia de caracteres de data/hora criada que não corresponde a nenhum dos formatos permitidos.</span><span class="sxs-lookup"><span data-stu-id="feb5d-172">The "Presentation" part HTML contains a created date/time string that does not match any of the allowed formats.</span></span> 

### <a name="20008"></a><span data-ttu-id="feb5d-173">20008</span><span class="sxs-lookup"><span data-stu-id="feb5d-173">20008</span></span>
<span data-ttu-id="feb5d-174">O tamanho da solicitação é muito grande.</span><span class="sxs-lookup"><span data-stu-id="feb5d-174">The size of the request is too large.</span></span> 

### <a name="20009"></a><span data-ttu-id="feb5d-175">20009</span><span class="sxs-lookup"><span data-stu-id="feb5d-175">20009</span></span>
<span data-ttu-id="feb5d-176">A solicitação contém partes com nomes duplicados.</span><span class="sxs-lookup"><span data-stu-id="feb5d-176">The request contains parts with duplicate names.</span></span> <span data-ttu-id="feb5d-177">Os nomes das partes devem ser exclusivos.</span><span class="sxs-lookup"><span data-stu-id="feb5d-177">Part names must be unique.</span></span> 

### <a name="20010"></a><span data-ttu-id="feb5d-178">20010</span><span class="sxs-lookup"><span data-stu-id="feb5d-178">20010</span></span>
<span data-ttu-id="feb5d-179">O cabeçalho Content-Disposition não foi fornecido para o tipo de conteúdo especificado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-179">The Content-Disposition header was not supplied for the specified content type.</span></span> 

### <a name="20011"></a><span data-ttu-id="feb5d-180">20011</span><span class="sxs-lookup"><span data-stu-id="feb5d-180">20011</span></span>
<span data-ttu-id="feb5d-181">A solicitação contém uma carga de partes múltiplas malformadas.</span><span class="sxs-lookup"><span data-stu-id="feb5d-181">The request contains a malformed multipart payload.</span></span> <span data-ttu-id="feb5d-182">Os problemas poderiam incluir ausência de linhas em branco, ausência de uma última linha, separadores de parte formatados incorretamente, etc.</span><span class="sxs-lookup"><span data-stu-id="feb5d-182">Problems could include missing blank lines, a missing last line, incorrectly formatted part separators, and so on.</span></span> <span data-ttu-id="feb5d-183">Se você estiver criando a mensagem de partes múltiplas à mão, verifique cuidadosamente a lógica, ou considere o uso de uma biblioteca de terceiros.</span><span class="sxs-lookup"><span data-stu-id="feb5d-183">If you're building the multipart message by hand, carefully check the logic, or consider using a third-party library.</span></span> 

### <a name="20012"></a><span data-ttu-id="feb5d-184">20012</span><span class="sxs-lookup"><span data-stu-id="feb5d-184">20012</span></span>
<span data-ttu-id="feb5d-185">A solicitação não fornece um tipo de conteúdo para a parte especificada.</span><span class="sxs-lookup"><span data-stu-id="feb5d-185">The request doesn't supply a content type for the specified part.</span></span> 
### <a name="20013"></a><span data-ttu-id="feb5d-186">20013</span><span class="sxs-lookup"><span data-stu-id="feb5d-186">20013</span></span>
<span data-ttu-id="feb5d-187">A solicitação não fornece cabeçalhos Content-Type e Content-Disposition para a parte especificada.</span><span class="sxs-lookup"><span data-stu-id="feb5d-187">The request doesn't supply Content-Type and Content-Disposition headers for the specified part.</span></span> 

### <a name="20014"></a><span data-ttu-id="feb5d-188">20014</span><span class="sxs-lookup"><span data-stu-id="feb5d-188">20014</span></span>
<span data-ttu-id="feb5d-189">O comprimento de uma parte na mensagem de partes múltiplas excede o tamanho máximo de 25 MB.</span><span class="sxs-lookup"><span data-stu-id="feb5d-189">The length of a part in the multipart message exceeds the maximum size of 25 MB.</span></span> 

### <a name="20015"></a><span data-ttu-id="feb5d-190">20015</span><span class="sxs-lookup"><span data-stu-id="feb5d-190">20015</span></span>
<span data-ttu-id="feb5d-191">A contagem das partes na mensagem de partes múltiplas excede o limite de 500.</span><span class="sxs-lookup"><span data-stu-id="feb5d-191">The count of parts in the multipart message exceeds the limit of 500.</span></span> 

### <a name="20016"></a><span data-ttu-id="feb5d-192">20016</span><span class="sxs-lookup"><span data-stu-id="feb5d-192">20016</span></span>
<span data-ttu-id="feb5d-193">O comprimento da mensagem de partes múltiplas excede o limite de 75 MB.</span><span class="sxs-lookup"><span data-stu-id="feb5d-193">The length of the multipart message exceeds the limit of 75 MB.</span></span> 

### <a name="20017"></a><span data-ttu-id="feb5d-194">20017</span><span class="sxs-lookup"><span data-stu-id="feb5d-194">20017</span></span>
<span data-ttu-id="feb5d-195">O MIME do email foi malformado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-195">The email MIME was malformed.</span></span> 

### <a name="20018"></a><span data-ttu-id="feb5d-196">20018</span><span class="sxs-lookup"><span data-stu-id="feb5d-196">20018</span></span>
<span data-ttu-id="feb5d-197">O MIME ou ICal da reunião foi malformado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-197">The meeting MIME or ICal was malformed.</span></span> 

### <a name="20019"></a><span data-ttu-id="feb5d-198">20019</span><span class="sxs-lookup"><span data-stu-id="feb5d-198">20019</span></span>
<span data-ttu-id="feb5d-199">Nenhum ICal foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-199">No ICal was found.</span></span> 

### <a name="20020"></a><span data-ttu-id="feb5d-200">20020</span><span class="sxs-lookup"><span data-stu-id="feb5d-200">20020</span></span>
<span data-ttu-id="feb5d-201">Json malformado encontrado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-201">Encountered malformed Json in request body.</span></span> 

### <a name="20100"></a><span data-ttu-id="feb5d-202">20100</span><span class="sxs-lookup"><span data-stu-id="feb5d-202">20100</span></span>
<span data-ttu-id="feb5d-203">Algo está errado com a sintaxe da sua solicitação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-203">Something is wrong with the syntax of your request.</span></span> 
### <a name="20101"></a><span data-ttu-id="feb5d-204">20101</span><span class="sxs-lookup"><span data-stu-id="feb5d-204">20101</span></span>
<span data-ttu-id="feb5d-205">A propriedade solicitada não existe.</span><span class="sxs-lookup"><span data-stu-id="feb5d-205">The property that you requested doesn't exist.</span></span>

### <a name="20102"></a><span data-ttu-id="feb5d-206">20102</span><span class="sxs-lookup"><span data-stu-id="feb5d-206">20102</span></span>
<span data-ttu-id="feb5d-207">Você solicitou um recurso que não existe.</span><span class="sxs-lookup"><span data-stu-id="feb5d-207">You requested a resource that doesn't exist.</span></span>

### <a name="20103"></a><span data-ttu-id="feb5d-208">20103</span><span class="sxs-lookup"><span data-stu-id="feb5d-208">20103</span></span>
<span data-ttu-id="feb5d-209">A consulta **expand** não tem suporte para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-209">The **expand** query is not supported for this request.</span></span> <span data-ttu-id="feb5d-210">Confira [Opções de cadeia de caracteres de consulta OData com suporte](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-get-content#query-options).</span><span class="sxs-lookup"><span data-stu-id="feb5d-210">See [Supported OData query string options](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-get-content#query-options).</span></span>

### <a name="20104"></a><span data-ttu-id="feb5d-211">20104</span><span class="sxs-lookup"><span data-stu-id="feb5d-211">20104</span></span>
<span data-ttu-id="feb5d-212">A opção de consulta **pagelevel** tem suporte somente na consulta para a coleção de páginas em uma seção ou para uma página específica.</span><span class="sxs-lookup"><span data-stu-id="feb5d-212">The **pagelevel** query option is supported only when querying for the pages collection in a section or for a specific page.</span></span> <span data-ttu-id="feb5d-213">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="feb5d-213">For example:</span></span>  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a><span data-ttu-id="feb5d-214">20106</span><span class="sxs-lookup"><span data-stu-id="feb5d-214">20106</span></span>
<span data-ttu-id="feb5d-215">Sua solicitação contém um operador de consulta que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="feb5d-215">Your request contains a query operator that is not supported.</span></span> 

### <a name="20108"></a><span data-ttu-id="feb5d-216">20108</span><span class="sxs-lookup"><span data-stu-id="feb5d-216">20108</span></span>
<span data-ttu-id="feb5d-217">Sua solicitação contém parâmetros de consulta OData sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feb5d-217">Your request contains unsupported OData query parameters.</span></span>

### <a name="20109"></a><span data-ttu-id="feb5d-218">20109</span><span class="sxs-lookup"><span data-stu-id="feb5d-218">20109</span></span>
<span data-ttu-id="feb5d-219">A carga na solicitação PATCH não foi criada corretamente.</span><span class="sxs-lookup"><span data-stu-id="feb5d-219">The payload in the PATCH request is not constructed correctly.</span></span>

### <a name="20110"></a><span data-ttu-id="feb5d-220">20110</span><span class="sxs-lookup"><span data-stu-id="feb5d-220">20110</span></span>
<span data-ttu-id="feb5d-221">As solicitações de criação de página com partes de dados exigem que o conteúdo seja de partes múltiplas, com uma parte "Apresentação".</span><span class="sxs-lookup"><span data-stu-id="feb5d-221">Page create requests with data parts require the content to be multipart, with a "Presentation" part.</span></span> 

### <a name="20111"></a><span data-ttu-id="feb5d-222">20111</span><span class="sxs-lookup"><span data-stu-id="feb5d-222">20111</span></span>
<span data-ttu-id="feb5d-223">Sua solicitação usa um recurso do OData que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="feb5d-223">Your request uses an OData feature that isn't supported.</span></span>

### <a name="20112"></a><span data-ttu-id="feb5d-224">20112</span><span class="sxs-lookup"><span data-stu-id="feb5d-224">20112</span></span>
<span data-ttu-id="feb5d-225">Sua solicitação contém uma ID inválida para o bloco de anotações, o grupo de seções, a seção ou a entidade de página do destino.</span><span class="sxs-lookup"><span data-stu-id="feb5d-225">Your request contains an invalid ID for the target notebook, section group, section, or page entity.</span></span>

### <a name="20113"></a><span data-ttu-id="feb5d-226">20113</span><span class="sxs-lookup"><span data-stu-id="feb5d-226">20113</span></span>
<span data-ttu-id="feb5d-227">O recurso especificado na solicitação foi excluído.</span><span class="sxs-lookup"><span data-stu-id="feb5d-227">The resource specified in the request has been deleted.</span></span>

### <a name="20115"></a><span data-ttu-id="feb5d-228">20115</span><span class="sxs-lookup"><span data-stu-id="feb5d-228">20115</span></span>
<span data-ttu-id="feb5d-229">O nome contém caracteres inválidos.</span><span class="sxs-lookup"><span data-stu-id="feb5d-229">The name contains invalid characters.</span></span> <span data-ttu-id="feb5d-230">Um nome de bloco de anotações não pode conter nenhum dos seguintes caracteres: `? * \ / : < > | ' "`</span><span class="sxs-lookup"><span data-stu-id="feb5d-230">A notebook name cannot contain any of the following characters: `? * \ / : < > | ' "`</span></span>

### <a name="20117"></a><span data-ttu-id="feb5d-231">20117</span><span class="sxs-lookup"><span data-stu-id="feb5d-231">20117</span></span>
<span data-ttu-id="feb5d-232">Um item com o nome especificado já existe no local que você especificou.</span><span class="sxs-lookup"><span data-stu-id="feb5d-232">An item with the name you specified already exists in the location that you specified.</span></span>

### <a name="20119"></a><span data-ttu-id="feb5d-233">20119</span><span class="sxs-lookup"><span data-stu-id="feb5d-233">20119</span></span>
<span data-ttu-id="feb5d-234">O HTML na parte "Apresentação" contém um atributo **data-attachment** que não tem um formato válido nem inclui um ou mais desses caracteres inválidos para um nome de arquivo: `\ / : * ? < > | "`.</span><span class="sxs-lookup"><span data-stu-id="feb5d-234">The HTML in the "Presentation" part contains a **data-attachment** attribute that either doesn't have a valid format or includes one or more of these invalid characters for a file name: `\ / : * ? < > | "`.</span></span> <span data-ttu-id="feb5d-235">A solicitação substituiu o valor indicado na mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="feb5d-235">The request substituted the value indicated in the error message.</span></span>

### <a name="20120"></a><span data-ttu-id="feb5d-236">20120</span><span class="sxs-lookup"><span data-stu-id="feb5d-236">20120</span></span>
<span data-ttu-id="feb5d-237">Sua solicitação especifica um destino PATCH que não pode ser localizado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-237">Your request specifies a PATCH target that can't be located.</span></span>

### <a name="20121"></a><span data-ttu-id="feb5d-238">20121</span><span class="sxs-lookup"><span data-stu-id="feb5d-238">20121</span></span>
<span data-ttu-id="feb5d-239">Sua solicitação contém um argumento PATCH inválido.</span><span class="sxs-lookup"><span data-stu-id="feb5d-239">Your request contains an invalid PATCH argument.</span></span> <span data-ttu-id="feb5d-240">Confira [Atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-240">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20122"></a><span data-ttu-id="feb5d-241">20122</span><span class="sxs-lookup"><span data-stu-id="feb5d-241">20122</span></span>
<span data-ttu-id="feb5d-242">Sua solicitação especifica uma ação PATCH sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feb5d-242">Your request specifies an unsupported PATCH action.</span></span> <span data-ttu-id="feb5d-243">Confira [Atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-243">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20123"></a><span data-ttu-id="feb5d-244">20123</span><span class="sxs-lookup"><span data-stu-id="feb5d-244">20123</span></span>
<span data-ttu-id="feb5d-245">A solicitação PATCH não pode alterar a página especificada.</span><span class="sxs-lookup"><span data-stu-id="feb5d-245">The PATCH request is unable to alter the specified page.</span></span>

### <a name="20124"></a><span data-ttu-id="feb5d-246">20124</span><span class="sxs-lookup"><span data-stu-id="feb5d-246">20124</span></span>
<span data-ttu-id="feb5d-247">Sua solicitação PATCH de partes múltiplas não inclui uma parte "comandos" com a estrutura JSON da ação PATCH.</span><span class="sxs-lookup"><span data-stu-id="feb5d-247">Your multipart PATCH request doesn't include a "commands" part with the PATCH action JSON structure.</span></span> <span data-ttu-id="feb5d-248">Confira [Atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-248">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20125"></a><span data-ttu-id="feb5d-249">20125</span><span class="sxs-lookup"><span data-stu-id="feb5d-249">20125</span></span>
<span data-ttu-id="feb5d-250">Sua solicitação PATCH não contém ações.</span><span class="sxs-lookup"><span data-stu-id="feb5d-250">Your PATCH request contains no actions.</span></span> <span data-ttu-id="feb5d-251">Confira [Atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-251">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20126"></a><span data-ttu-id="feb5d-252">20126</span><span class="sxs-lookup"><span data-stu-id="feb5d-252">20126</span></span>
<span data-ttu-id="feb5d-253">O corpo da mensagem contém JSON incorretamente formatado ou arquivos que não têm suporte para essa operação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-253">The message body contains either incorrectly formatted JSON or fields that are not supported for this operation.</span></span>

### <a name="20127"></a><span data-ttu-id="feb5d-254">20127</span><span class="sxs-lookup"><span data-stu-id="feb5d-254">20127</span></span>
<span data-ttu-id="feb5d-255">Sua solicitação especifica o nome de uma propriedade desconhecida.</span><span class="sxs-lookup"><span data-stu-id="feb5d-255">Your request specifies the name of an unknown property.</span></span>

### <a name="20128"></a><span data-ttu-id="feb5d-256">20128</span><span class="sxs-lookup"><span data-stu-id="feb5d-256">20128</span></span>
<span data-ttu-id="feb5d-257">Sua solicitação contém um erro de sintaxe OData na posição indicada na mensagem.</span><span class="sxs-lookup"><span data-stu-id="feb5d-257">Your request contains an OData syntax error at the position indicated in the message.</span></span>

### <a name="20129"></a><span data-ttu-id="feb5d-258">20129</span><span class="sxs-lookup"><span data-stu-id="feb5d-258">20129</span></span>
<span data-ttu-id="feb5d-259">Sua solicitação contém uma opção de cadeia de caracteres de consulta **top** cujo valor é muito alto.</span><span class="sxs-lookup"><span data-stu-id="feb5d-259">Your request contains a **top** query string option whose value is too high.</span></span> <span data-ttu-id="feb5d-260">Para consultas de página, o valor máximo é 100 e o valor padrão é 20.</span><span class="sxs-lookup"><span data-stu-id="feb5d-260">For page queries, the maximum value is 100, and the default value is 20.</span></span>

### <a name="20130"></a><span data-ttu-id="feb5d-261">20130</span><span class="sxs-lookup"><span data-stu-id="feb5d-261">20130</span></span>
<span data-ttu-id="feb5d-262">Sua solicitação contém um URI que aponta para um recurso HTTP que não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-262">Your request contains a URI that points to an HTTP resource that can't be found.</span></span>

### <a name="20131"></a><span data-ttu-id="feb5d-263">20131</span><span class="sxs-lookup"><span data-stu-id="feb5d-263">20131</span></span>
<span data-ttu-id="feb5d-264">Sua solicitação contém um valor inválido para Content-Type.</span><span class="sxs-lookup"><span data-stu-id="feb5d-264">Your request contains an invalid value for Content-Type.</span></span> <span data-ttu-id="feb5d-265">Use o valor indicado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="feb5d-265">Use the value indicated in the message.</span></span> 

### <a name="20132"></a><span data-ttu-id="feb5d-266">20132</span><span class="sxs-lookup"><span data-stu-id="feb5d-266">20132</span></span>
<span data-ttu-id="feb5d-267">Sua solicitação apresentas conteúdo inválido.</span><span class="sxs-lookup"><span data-stu-id="feb5d-267">Your request contains invalid content.</span></span> <span data-ttu-id="feb5d-268">As causas mais comuns para isso são a ausência do cabeçalho da solicitação Content-Type e/ou nenhum conteúdo no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-268">Common causes for this are a missing Content-Type request header and/or no content in the body of the request.</span></span> 

### <a name="20133"></a><span data-ttu-id="feb5d-269">20133</span><span class="sxs-lookup"><span data-stu-id="feb5d-269">20133</span></span>
<span data-ttu-id="feb5d-270">Sua solicitação especifica um destino PATCH sem suporte.</span><span class="sxs-lookup"><span data-stu-id="feb5d-270">Your request specifies a PATCH target that is not supported.</span></span> <span data-ttu-id="feb5d-271">Confira [Atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-271">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20134"></a><span data-ttu-id="feb5d-272">20134</span><span class="sxs-lookup"><span data-stu-id="feb5d-272">20134</span></span>
<span data-ttu-id="feb5d-273">Sua solicitação especifica um elemento inválido como o destino da ação PATCH.</span><span class="sxs-lookup"><span data-stu-id="feb5d-273">Your request specifies an invalid element as the target of the PATCH action.</span></span> <span data-ttu-id="feb5d-274">Se o destino usar o identificador **data-id**, verifique se ele tem o símbolo # como prefixo.</span><span class="sxs-lookup"><span data-stu-id="feb5d-274">If the target uses the **data-id** identifier, make sure it's prefixed with a # symbol.</span></span> <span data-ttu-id="feb5d-275">Confira [Atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-275">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20135"></a><span data-ttu-id="feb5d-276">20135</span><span class="sxs-lookup"><span data-stu-id="feb5d-276">20135</span></span>
<span data-ttu-id="feb5d-277">Sua solicitação especifica um tipo de entidade que não tem suporte para a operação PATCH.</span><span class="sxs-lookup"><span data-stu-id="feb5d-277">Your request specifies an entity type that is not supported for the PATCH operation.</span></span> <span data-ttu-id="feb5d-278">Confira [Atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-278">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20136"></a><span data-ttu-id="feb5d-279">20136</span><span class="sxs-lookup"><span data-stu-id="feb5d-279">20136</span></span>
<span data-ttu-id="feb5d-280">Sua solicitação contém um atributo **data-render-src** ou **data-render-method** inválido ou que está ausente.</span><span class="sxs-lookup"><span data-stu-id="feb5d-280">Your request contains an invalid or missing **data-render-src** or **data-render-method** attribute.</span></span> <span data-ttu-id="feb5d-281">Confira [Extrair dados de capturas](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-extract-data).</span><span class="sxs-lookup"><span data-stu-id="feb5d-281">See [Extract data from captures](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-extract-data).</span></span>

### <a name="20137"></a><span data-ttu-id="feb5d-282">20137</span><span class="sxs-lookup"><span data-stu-id="feb5d-282">20137</span></span>
<span data-ttu-id="feb5d-283">A página de destino não dá suporte a solicitações PATCH.</span><span class="sxs-lookup"><span data-stu-id="feb5d-283">The target page does not support PATCH requests.</span></span>

### <a name="20138"></a><span data-ttu-id="feb5d-284">20138</span><span class="sxs-lookup"><span data-stu-id="feb5d-284">20138</span></span>
<span data-ttu-id="feb5d-285">O tipo de elemento de destino em sua solicitação PATCH não dá suporte à ação **acrescentar**.</span><span class="sxs-lookup"><span data-stu-id="feb5d-285">The target element type in your PATCH request doesn't support the **append** action.</span></span> <span data-ttu-id="feb5d-286">Confira [Atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-286">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20139"></a><span data-ttu-id="feb5d-287">20139</span><span class="sxs-lookup"><span data-stu-id="feb5d-287">20139</span></span>
<span data-ttu-id="feb5d-288">Sua solicitação contém um valor de atributo **data-tag** inválido.</span><span class="sxs-lookup"><span data-stu-id="feb5d-288">Your request contains an invalid **data-tag** attribute value.</span></span> <span data-ttu-id="feb5d-289">Confira [Usar marcas de anotação](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-note-tags).</span><span class="sxs-lookup"><span data-stu-id="feb5d-289">See [Use note tags](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-note-tags).</span></span>

### <a name="20140"></a><span data-ttu-id="feb5d-290">20140</span><span class="sxs-lookup"><span data-stu-id="feb5d-290">20140</span></span>
<span data-ttu-id="feb5d-291">Sua solicitação contém um valor de status **data-tag** inválido.</span><span class="sxs-lookup"><span data-stu-id="feb5d-291">Your request contains an invalid **data-tag** status value.</span></span> <span data-ttu-id="feb5d-292">A caixa de seleção de marcas de anotação pode ter um status **concluído**.</span><span class="sxs-lookup"><span data-stu-id="feb5d-292">Check box note tags can have a **completed** status.</span></span> <span data-ttu-id="feb5d-293">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="feb5d-293">Example:</span></span>
```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
<span data-ttu-id="feb5d-294">Confira [Usar marcas de anotação](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-note-tags).</span><span class="sxs-lookup"><span data-stu-id="feb5d-294">See [Use note tags](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-note-tags).</span></span>

### <a name="20141"></a><span data-ttu-id="feb5d-295">20141</span><span class="sxs-lookup"><span data-stu-id="feb5d-295">20141</span></span>
<span data-ttu-id="feb5d-296">O destino em sua solicitação PATCH não dá suporte à ação especificada.</span><span class="sxs-lookup"><span data-stu-id="feb5d-296">The target in your PATCH request doesn't support the specified action.</span></span> <span data-ttu-id="feb5d-297">Confira [Atualizar conteúdo da página](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-297">See [Update page content](../api-reference/v1.0/api/page_update.md).</span></span>

### <a name="20142"></a><span data-ttu-id="feb5d-298">20142</span><span class="sxs-lookup"><span data-stu-id="feb5d-298">20142</span></span>
<span data-ttu-id="feb5d-299">Sua solicitação contém uma expressão **expand** para um pai de entidades filho ou um filho de entidades pai, que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="feb5d-299">Your request contains an **expand** expression for a parent of child entities or a child of parent entities, which is not supported.</span></span> <span data-ttu-id="feb5d-300">Confira [Opções de cadeia de caracteres de consulta OData com suporte](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-get-content#query-options).</span><span class="sxs-lookup"><span data-stu-id="feb5d-300">See [Supported OData query string options](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-get-content#query-options).</span></span>

### <a name="20143"></a><span data-ttu-id="feb5d-301">20143</span><span class="sxs-lookup"><span data-stu-id="feb5d-301">20143</span></span>
<span data-ttu-id="feb5d-302">A consulta OData é inválida.</span><span class="sxs-lookup"><span data-stu-id="feb5d-302">The OData query is invalid.</span></span>

### <a name="20144"></a><span data-ttu-id="feb5d-303">20144</span><span class="sxs-lookup"><span data-stu-id="feb5d-303">20144</span></span>
<span data-ttu-id="feb5d-304">Sua solicitação contém uma expressão **expand** para uma propriedade de não navegação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-304">Your request contains an **expand** expression for a non-navigation property.</span></span> <span data-ttu-id="feb5d-305">Somente as propriedades de navegação podem ser expandidas.</span><span class="sxs-lookup"><span data-stu-id="feb5d-305">Only navigation properties can be expanded.</span></span>

### <a name="20145"></a><span data-ttu-id="feb5d-306">20145</span><span class="sxs-lookup"><span data-stu-id="feb5d-306">20145</span></span>
<span data-ttu-id="feb5d-307">A expressão **select** ou **expand** em sua solicitação contém um termo inválido.</span><span class="sxs-lookup"><span data-stu-id="feb5d-307">The **select** or **expand** expression in your request contains an invalid term.</span></span>

### <a name="20146"></a><span data-ttu-id="feb5d-308">20146</span><span class="sxs-lookup"><span data-stu-id="feb5d-308">20146</span></span>
<span data-ttu-id="feb5d-309">O atributo `style="position:absolute"`é especificado em um elemento, mas o elemento **body** não especifica `data-absolute-enabled="true"`, que é exigido para dar suporte ao posicionamento.</span><span class="sxs-lookup"><span data-stu-id="feb5d-309">The `style="position:absolute"` attribute is specified on an element, but the **body** element does not specify `data-absolute-enabled="true"`, which is required to support positioning.</span></span> <span data-ttu-id="feb5d-310">Todas as configurações de posição serão ignoradas.</span><span class="sxs-lookup"><span data-stu-id="feb5d-310">All position settings will be ignored.</span></span> <span data-ttu-id="feb5d-311">Confira [Criar elementos posicionados absolutos](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-311">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20147"></a><span data-ttu-id="feb5d-312">20147</span><span class="sxs-lookup"><span data-stu-id="feb5d-312">20147</span></span>
<span data-ttu-id="feb5d-313">O atributo `style="position:absolute"` é especificado em um elemento que não é um filho direto do elemento **body**, que não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="feb5d-313">The `style="position:absolute"` attribute is specified on an element that is not a direct child of the **body** element, which is not supported.</span></span> <span data-ttu-id="feb5d-314">Se o elemento for um **div**, **img** ou **object**, torne-o um filho direto de body; caso contrário, as configurações de posição serão ignoradas e seu conteúdo será renderizado dentro de um div posicionado absoluto.</span><span class="sxs-lookup"><span data-stu-id="feb5d-314">If the element is a **div**, **img**, or **object**, make it a direct child of the body; otherwise the position settings will be ignored and its content will render inside an absolute positioned div.</span></span> <span data-ttu-id="feb5d-315">Confira [Criar elementos posicionados absolutos](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-315">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20148"></a><span data-ttu-id="feb5d-316">20148</span><span class="sxs-lookup"><span data-stu-id="feb5d-316">20148</span></span>
<span data-ttu-id="feb5d-317">O atributo `style="position:absolute"` é especificado em um tipo de elemento que não dá suporte a ele.</span><span class="sxs-lookup"><span data-stu-id="feb5d-317">The `style="position:absolute"` attribute is specified on an element type that does not support it.</span></span> <span data-ttu-id="feb5d-318">Somente elementos **div**, **img** e **object** que são filhos direto do corpo da página dão suporte ao posicionamento.</span><span class="sxs-lookup"><span data-stu-id="feb5d-318">Only **div**, **img**, and **object** elements that are direct children of the page body support positioning.</span></span> <span data-ttu-id="feb5d-319">Confira [Criar elementos posicionados absolutos](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="feb5d-319">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20149"></a><span data-ttu-id="feb5d-320">20149</span><span class="sxs-lookup"><span data-stu-id="feb5d-320">20149</span></span>
<span data-ttu-id="feb5d-321">Sua solicitação especifica um elemento de destino que não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-321">Your request specifies a target element that cannot be found.</span></span>

### <a name="20150"></a><span data-ttu-id="feb5d-322">20150</span><span class="sxs-lookup"><span data-stu-id="feb5d-322">20150</span></span>
<span data-ttu-id="feb5d-323">A solicitação não é válida para esse tipo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-323">The request is not valid for this authentication type.</span></span> <span data-ttu-id="feb5d-324">Use o caminho `../me/onenote/` no lugar.</span><span class="sxs-lookup"><span data-stu-id="feb5d-324">Use the `../me/onenote/` path instead.</span></span>

### <a name="20151"></a><span data-ttu-id="feb5d-325">20151</span><span class="sxs-lookup"><span data-stu-id="feb5d-325">20151</span></span>
<span data-ttu-id="feb5d-326">A solicitação não é válida para esse tipo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-326">The request is not valid for this authentication type.</span></span> <span data-ttu-id="feb5d-327">Use o ponto de extremidade `../me/onenote/section/{id}/pages` para criar uma página em uma seção específica.</span><span class="sxs-lookup"><span data-stu-id="feb5d-327">Use the `../me/onenote/section/{id}/pages` endpoint to create a page in a specific section.</span></span>

### <a name="20152"></a><span data-ttu-id="feb5d-328">20152</span><span class="sxs-lookup"><span data-stu-id="feb5d-328">20152</span></span>
<span data-ttu-id="feb5d-329">Não há qualquer valor de nome especificado para a entidade.</span><span class="sxs-lookup"><span data-stu-id="feb5d-329">There is no name value specified for the entity.</span></span> <span data-ttu-id="feb5d-330">O nome deve ser definido e não pode conter somente espaços em branco.</span><span class="sxs-lookup"><span data-stu-id="feb5d-330">The name must be defined, and it cannot contain whitespaces only.</span></span>

### <a name="20153"></a><span data-ttu-id="feb5d-331">20153</span><span class="sxs-lookup"><span data-stu-id="feb5d-331">20153</span></span>
<span data-ttu-id="feb5d-332">O nome da entidade contém caracteres inválidos.</span><span class="sxs-lookup"><span data-stu-id="feb5d-332">The entity name contains invalid characters.</span></span> <span data-ttu-id="feb5d-333">O nome não pode conter os seguintes caracteres: `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="feb5d-333">The name cannot contain the following characters: `? * \ / : < > | & # " % ~`</span></span>

### <a name="20154"></a><span data-ttu-id="feb5d-334">20154</span><span class="sxs-lookup"><span data-stu-id="feb5d-334">20154</span></span>
<span data-ttu-id="feb5d-335">O nome da entidade não pode começar com um espaço.</span><span class="sxs-lookup"><span data-stu-id="feb5d-335">The entity name cannot start with a space.</span></span>

### <a name="20155"></a><span data-ttu-id="feb5d-336">20155</span><span class="sxs-lookup"><span data-stu-id="feb5d-336">20155</span></span>
<span data-ttu-id="feb5d-337">O nome da entidade é muito longo.</span><span class="sxs-lookup"><span data-stu-id="feb5d-337">The entity name is too long.</span></span> <span data-ttu-id="feb5d-338">Os nomes do bloco de anotações têm um limite de 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="feb5d-338">Notebook names have a 128-character limit.</span></span> <span data-ttu-id="feb5d-339">Outros nomes de entidade têm um limite de 50 caracteres.</span><span class="sxs-lookup"><span data-stu-id="feb5d-339">Other entity names have a 50-character limit.</span></span>

### <a name="20156"></a><span data-ttu-id="feb5d-340">20156</span><span class="sxs-lookup"><span data-stu-id="feb5d-340">20156</span></span>
<span data-ttu-id="feb5d-341">A ID especificada para o recurso de destino não existe.</span><span class="sxs-lookup"><span data-stu-id="feb5d-341">The specified ID for the destination resource does not exist.</span></span>

### <a name="20157"></a><span data-ttu-id="feb5d-342">20157</span><span class="sxs-lookup"><span data-stu-id="feb5d-342">20157</span></span>
<span data-ttu-id="feb5d-343">A ID especificada para a entidade de destino é inválida.</span><span class="sxs-lookup"><span data-stu-id="feb5d-343">The specified ID for the destination entity is invalid.</span></span>

### <a name="20158"></a><span data-ttu-id="feb5d-344">20158</span><span class="sxs-lookup"><span data-stu-id="feb5d-344">20158</span></span>
<span data-ttu-id="feb5d-345">Não é possível obter metadados para a URL do site especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-345">Unable to get metadata for the site URL specified in the request.</span></span> <span data-ttu-id="feb5d-346">Verifique o formato da URL fornecida.</span><span class="sxs-lookup"><span data-stu-id="feb5d-346">Check the format of the supplied URL.</span></span> <span data-ttu-id="feb5d-347">Os formatos com suporte incluem `https://domain.sharepoint.com/site-a` e `https://domain.com/sites/site-a`.</span><span class="sxs-lookup"><span data-stu-id="feb5d-347">Supported formats include `https://domain.sharepoint.com/site-a` and `https://domain.com/sites/site-a`.</span></span>

### <a name="20160"></a><span data-ttu-id="feb5d-348">20160</span><span class="sxs-lookup"><span data-stu-id="feb5d-348">20160</span></span>
<span data-ttu-id="feb5d-349">Não é possível encontrar um grupo unificado do Office 365 que tem a ID especificada.</span><span class="sxs-lookup"><span data-stu-id="feb5d-349">Unable to find an Office 365 unified group that has the specified ID.</span></span>

### <a name="20161"></a><span data-ttu-id="feb5d-350">20161</span><span class="sxs-lookup"><span data-stu-id="feb5d-350">20161</span></span>
<span data-ttu-id="feb5d-351">O contexto não especifica uma ID de usuário válida.</span><span class="sxs-lookup"><span data-stu-id="feb5d-351">The context does not specify a valid user ID.</span></span> <span data-ttu-id="feb5d-352">Um erro comum é que PUID/CID foi transmitido como um longo, e não como um hexadecimal.</span><span class="sxs-lookup"><span data-stu-id="feb5d-352">One common error is that PUID/CID was passed in as a long instead of a hex.</span></span>

### <a name="20166"></a><span data-ttu-id="feb5d-353">20166</span><span class="sxs-lookup"><span data-stu-id="feb5d-353">20166</span></span>
<span data-ttu-id="feb5d-354">O aplicativo emitiu muitas solicitações em nome de um usuário em um curto período de tempo.</span><span class="sxs-lookup"><span data-stu-id="feb5d-354">The application has issued too many requests on behalf of a user in a short period of time.</span></span> <span data-ttu-id="feb5d-355">Para ajudar a garantir que a API do OneNote permaneça estável e responsiva, a API retorna um código de status 429 e esse erro quando detecta que um aplicativo está usando muitos recursos.</span><span class="sxs-lookup"><span data-stu-id="feb5d-355">To help ensure that the OneNote API remains stable and responsive, the API returns a 429 status code and this error when it detects that an application is using too many resources.</span></span> 

<span data-ttu-id="feb5d-356">Para saber mais, confira [Limitação da API do OneNote e como evitá-la](http://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span><span class="sxs-lookup"><span data-stu-id="feb5d-356">For more information, see [OneNote API throttling and how to avoid it](http://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span></span>

### <a name="20168"></a><span data-ttu-id="feb5d-357">20168</span><span class="sxs-lookup"><span data-stu-id="feb5d-357">20168</span></span>
<span data-ttu-id="feb5d-358">Não há suporte para a fonte do vídeo especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-358">The video source specified in the request is not supported.</span></span> <span data-ttu-id="feb5d-359">Confira [Sites de vídeo com suporte](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-images-files#videos) para a lista atual.</span><span class="sxs-lookup"><span data-stu-id="feb5d-359">See [Supported video sites](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-images-files#videos) for the current list.</span></span>


## <a name="codes-from-30001-to-39999"></a><span data-ttu-id="feb5d-360">Códigos de 30001 às 39999</span><span class="sxs-lookup"><span data-stu-id="feb5d-360">Codes from 30001 to 39999</span></span>
<span data-ttu-id="feb5d-361">Algo está errado com a conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="feb5d-361">Something is wrong with the user's account.</span></span>

### <a name="30101"></a><span data-ttu-id="feb5d-362">30101</span><span class="sxs-lookup"><span data-stu-id="feb5d-362">30101</span></span>
<span data-ttu-id="feb5d-363">A conta do usuário excedeu sua cota do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="feb5d-363">The user account has exceeded its OneDrive quota.</span></span> <span data-ttu-id="feb5d-364">Confira [OneDrive](https://onedrive.live.com/about/pt-BR/).</span><span class="sxs-lookup"><span data-stu-id="feb5d-364">See [OneDrive](https://onedrive.live.com/about/pt-BR/).</span></span>

### <a name="30102"></a><span data-ttu-id="feb5d-365">30102</span><span class="sxs-lookup"><span data-stu-id="feb5d-365">30102</span></span>
<span data-ttu-id="feb5d-366">Nada mais pode ser adicionado à seção solicitada porque ela atingiu seu tamanho máximo.</span><span class="sxs-lookup"><span data-stu-id="feb5d-366">Nothing more can be added to the requested section because it has reached its maximum size.</span></span>

### <a name="30103"></a><span data-ttu-id="feb5d-367">30103</span><span class="sxs-lookup"><span data-stu-id="feb5d-367">30103</span></span>
<span data-ttu-id="feb5d-368">O consumo de recursos é muito alto para a solicitação.</span><span class="sxs-lookup"><span data-stu-id="feb5d-368">Resource consumption is too high for the request.</span></span> <span data-ttu-id="feb5d-369">A conta de usuário de destino tem um grande conjunto de dados ou o serviço está recebendo um grande número de solicitações simultâneas para o mesmo site (por exemplo, o site pessoal do usuário ou um site de equipe).</span><span class="sxs-lookup"><span data-stu-id="feb5d-369">Either the target user account has a large dataset, or the service is receiving a high number of concurrent requests to the same site (for example, the user's personal site or a team site).</span></span>

### <a name="30104"></a><span data-ttu-id="feb5d-370">30104</span><span class="sxs-lookup"><span data-stu-id="feb5d-370">30104</span></span>
<span data-ttu-id="feb5d-371">A conta de usuário foi suspensa.</span><span class="sxs-lookup"><span data-stu-id="feb5d-371">The user account has been suspended.</span></span>

### <a name="30105"></a><span data-ttu-id="feb5d-372">30105</span><span class="sxs-lookup"><span data-stu-id="feb5d-372">30105</span></span>
<span data-ttu-id="feb5d-373">O site pessoal do OneDrive for Business do usuário não foi provisionado, que é obrigatório para acessar os blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="feb5d-373">The user's personal OneDrive for Business site is not provisioned, which is required to access notebooks.</span></span> <span data-ttu-id="feb5d-374">Agora, o serviço do OneNote provisionará o site.</span><span class="sxs-lookup"><span data-stu-id="feb5d-374">The OneNote service will provision the site now.</span></span> <span data-ttu-id="feb5d-375">Este processo pode levar algum tempo.</span><span class="sxs-lookup"><span data-stu-id="feb5d-375">This process may take several minutes.</span></span>

### <a name="30106"></a><span data-ttu-id="feb5d-376">30106</span><span class="sxs-lookup"><span data-stu-id="feb5d-376">30106</span></span>
<span data-ttu-id="feb5d-377">O OneDrive for Business está sendo provisionado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="feb5d-377">OneDrive for Business is being provisioned for the user.</span></span>

### <a name="30108"></a><span data-ttu-id="feb5d-378">30108</span><span class="sxs-lookup"><span data-stu-id="feb5d-378">30108</span></span>
<span data-ttu-id="feb5d-379">O OneDrive for Business pessoal do usuário não pôde ser recuperado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-379">The user's personal OneDrive for Business could not be retrieved.</span></span> <span data-ttu-id="feb5d-380">A tabela a seguir lista algumas possíveis causas.</span><span class="sxs-lookup"><span data-stu-id="feb5d-380">The following table lists some possible causes.</span></span>

| <span data-ttu-id="feb5d-381">Causa</span><span class="sxs-lookup"><span data-stu-id="feb5d-381">Cause</span></span> | <span data-ttu-id="feb5d-382">Resolução</span><span class="sxs-lookup"><span data-stu-id="feb5d-382">Resolution</span></span> |
|:------|:------|
| <span data-ttu-id="feb5d-383">O site pessoal do usuário não foi provisionado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-383">The user's personal site has not been provisioned.</span></span> | <span data-ttu-id="feb5d-384">O usuário deve abrir o OneDrive for Business e seguir as instruções para provisionar o site.</span><span class="sxs-lookup"><span data-stu-id="feb5d-384">The user should open OneDrive for Business and follow any instructions to provision the site.</span></span> <span data-ttu-id="feb5d-385">Se isso falhar, eles deverão entrar em contato com o administrador de locatários do Office 365.</span><span class="sxs-lookup"><span data-stu-id="feb5d-385">If this fails, they should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="feb5d-386">No momento, o site pessoal do usuário está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-386">The user's personal site is currently being provisioned.</span></span> | <span data-ttu-id="feb5d-387">Tente a solicitação mais tarde.</span><span class="sxs-lookup"><span data-stu-id="feb5d-387">Try the request later.</span></span> |
| <span data-ttu-id="feb5d-388">O usuário não tem uma licença válida do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="feb5d-388">The user does not have a valid OneDrive for Business license.</span></span> | <span data-ttu-id="feb5d-389">O usuário deve contatar o administrador de locatários do Office 365.</span><span class="sxs-lookup"><span data-stu-id="feb5d-389">The user should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="feb5d-390">Um problema de rede impediu a solicitação de ser enviada com êxito.</span><span class="sxs-lookup"><span data-stu-id="feb5d-390">A network issue prevented the request from being successfully sent.</span></span> | <span data-ttu-id="feb5d-391">Tente a solicitação mais tarde.</span><span class="sxs-lookup"><span data-stu-id="feb5d-391">Try the request later.</span></span> |

### <a name="30109"></a><span data-ttu-id="feb5d-392">30109</span><span class="sxs-lookup"><span data-stu-id="feb5d-392">30109</span></span>
<span data-ttu-id="feb5d-393">Alguns usuários na solicitação não existem.</span><span class="sxs-lookup"><span data-stu-id="feb5d-393">Some users in the request do not exist.</span></span>

### <a name="30110"></a><span data-ttu-id="feb5d-394">30110</span><span class="sxs-lookup"><span data-stu-id="feb5d-394">30110</span></span>
<span data-ttu-id="feb5d-395">Os Serviços de Informações do Aluno não foram registrados para esse locatário.</span><span class="sxs-lookup"><span data-stu-id="feb5d-395">Student Information Services has not been registered for this tenant.</span></span>

### <a name="30111"></a><span data-ttu-id="feb5d-396">30111</span><span class="sxs-lookup"><span data-stu-id="feb5d-396">30111</span></span>
<span data-ttu-id="feb5d-397">Há um erro genérico com os Serviços de Informações do Aluno.</span><span class="sxs-lookup"><span data-stu-id="feb5d-397">There is a generic error with Student Information Services.</span></span>

### <a name="30112"></a><span data-ttu-id="feb5d-398">30112</span><span class="sxs-lookup"><span data-stu-id="feb5d-398">30112</span></span>
<span data-ttu-id="feb5d-399">Vários usuários afetados pela solicitação tinham o mesmo nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="feb5d-399">Multiple users affected by the request had the same username.</span></span>

### <a name="30113"></a><span data-ttu-id="feb5d-400">30113</span><span class="sxs-lookup"><span data-stu-id="feb5d-400">30113</span></span>
<span data-ttu-id="feb5d-401">O bloco de anotações não está configurado para permitir convites.</span><span class="sxs-lookup"><span data-stu-id="feb5d-401">The notebook is not configured to allow invites.</span></span>

### <a name="30114"></a><span data-ttu-id="feb5d-402">30114</span><span class="sxs-lookup"><span data-stu-id="feb5d-402">30114</span></span>
<span data-ttu-id="feb5d-403">Há um parâmetro obrigatório ausente.</span><span class="sxs-lookup"><span data-stu-id="feb5d-403">There is a required parameter missing.</span></span>

## <a name="codes-from-40001-to-49999"></a><span data-ttu-id="feb5d-404">Códigos de 40001 às 49999</span><span class="sxs-lookup"><span data-stu-id="feb5d-404">Codes from 40001 to 49999</span></span>
<span data-ttu-id="feb5d-405">O usuário ou o aplicativo não tem as permissões corretas.</span><span class="sxs-lookup"><span data-stu-id="feb5d-405">The user or application does not have the correct permissions.</span></span>

### <a name="40001"></a><span data-ttu-id="feb5d-406">40001</span><span class="sxs-lookup"><span data-stu-id="feb5d-406">40001</span></span>
<span data-ttu-id="feb5d-407">A solicitação não contém um token OAuth válido.</span><span class="sxs-lookup"><span data-stu-id="feb5d-407">The request doesn't contain a valid OAuth token.</span></span> <span data-ttu-id="feb5d-408">Confira [Permissões de notas](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="feb5d-408">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40002"></a><span data-ttu-id="feb5d-409">40002</span><span class="sxs-lookup"><span data-stu-id="feb5d-409">40002</span></span>
<span data-ttu-id="feb5d-410">O usuário não tem permissão para gravar no local solicitado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-410">The user doesn't have permission to write to the requested location.</span></span>

### <a name="40003"></a><span data-ttu-id="feb5d-411">40003</span><span class="sxs-lookup"><span data-stu-id="feb5d-411">40003</span></span>
<span data-ttu-id="feb5d-412">O usuário não tem permissão para acessar o recurso solicitado.</span><span class="sxs-lookup"><span data-stu-id="feb5d-412">The user doesn't have permission to access the requested resource.</span></span>

### <a name="40004"></a><span data-ttu-id="feb5d-413">40004</span><span class="sxs-lookup"><span data-stu-id="feb5d-413">40004</span></span>
<span data-ttu-id="feb5d-414">O token OAuth não tem os escopos necessários para executar a ação solicitada.</span><span class="sxs-lookup"><span data-stu-id="feb5d-414">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="feb5d-415">Confira [Permissões de notas](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="feb5d-415">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40006"></a><span data-ttu-id="feb5d-416">40006</span><span class="sxs-lookup"><span data-stu-id="feb5d-416">40006</span></span> 
<span data-ttu-id="feb5d-417">O token OAuth não tem os escopos necessários para executar a ação solicitada.</span><span class="sxs-lookup"><span data-stu-id="feb5d-417">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="feb5d-418">Especificamente a permissão de edição.</span><span class="sxs-lookup"><span data-stu-id="feb5d-418">Specifically the edit permission.</span></span> <span data-ttu-id="feb5d-419">Confira [Permissões de notas](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="feb5d-419">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40007"></a><span data-ttu-id="feb5d-420">40007</span><span class="sxs-lookup"><span data-stu-id="feb5d-420">40007</span></span>
<span data-ttu-id="feb5d-421">O usuário não tem permissões para acessar esse recurso.</span><span class="sxs-lookup"><span data-stu-id="feb5d-421">The user does not have permissions to access this resource.</span></span>

### <a name="40008"></a><span data-ttu-id="feb5d-422">40008</span><span class="sxs-lookup"><span data-stu-id="feb5d-422">40008</span></span>
<span data-ttu-id="feb5d-423">O acesso é proibido para esse recurso.</span><span class="sxs-lookup"><span data-stu-id="feb5d-423">Access is Forbidden for this resource.</span></span>

### <a name="40009"></a><span data-ttu-id="feb5d-424">40009</span><span class="sxs-lookup"><span data-stu-id="feb5d-424">40009</span></span>
<span data-ttu-id="feb5d-425">O contêiner já está em uso por outro recurso.</span><span class="sxs-lookup"><span data-stu-id="feb5d-425">The container is already in use by another resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="feb5d-426">Confira também</span><span class="sxs-lookup"><span data-stu-id="feb5d-426">See also</span></span>

- [<span data-ttu-id="feb5d-427">Respostas de erro e tipos de recurso do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="feb5d-427">Microsoft Graph error responses and resource types</span></span>](errors.md)
- [<span data-ttu-id="feb5d-428">Referência do OneNote</span><span class="sxs-lookup"><span data-stu-id="feb5d-428">OneNote reference</span></span>](../api-reference/v1.0/resources/onenote.md)

