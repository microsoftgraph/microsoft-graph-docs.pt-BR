<span data-ttu-id="20547-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20547-p101">Bearer {token}. Required.</span></span>  | {token} de portador. Obrigatório. |

## <a name="request-body"></a><span data-ttu-id="20547-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20547-115">Request body</span></span>
<span data-ttu-id="20547-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20547-116">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="20547-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="20547-117">Response</span></span>
<span data-ttu-id="20547-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e os dados binários do arquivo ou imagem no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20547-118">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="20547-119">Observação: As imagens não serão renderizadas diretamente em um navegador porque elas exigem autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="20547-119">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="20547-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20547-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20547-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20547-121">Request</span></span>
<span data-ttu-id="20547-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20547-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="20547-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="20547-123">Response</span></span>
<span data-ttu-id="20547-124">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20547-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
