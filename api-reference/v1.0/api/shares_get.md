<span data-ttu-id="05af4-p101">Embora [**SharedDriveItem**](../resources/shareddriveitem.md) contenha algumas informações úteis, a maioria dos aplicativos acessará diretamente o [DriveItem](../resources/driveitem.md) compartilhado. O recurso **SharedDriveItem** inclui **root** e relações **itens** que podem acessar o conteúdo no escopo do item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="05af4-p101">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

Embora [**SharedDriveItem**](../resources/shareddriveitem.md) contenha algumas informações úteis, a maioria dos aplicativos acessará diretamente o [DriveItem](../resources/driveitem.md) compartilhado. O recurso **SharedDriveItem** inclui **root** e relações **itens** que podem acessar o conteúdo no escopo do item compartilhado.

### <span data-ttu-id="05af4-122">Exemplo (arquivo único)</span><span class="sxs-lookup"><span data-stu-id="05af4-122">Example (single file)</span></span>
<a id="example-single-file" class="xliff"></a>

##### <span data-ttu-id="05af4-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05af4-123">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="05af4-124">Solicitando a relação **root**, o **DriveItem** que foi compartilhado será retornado.</span><span class="sxs-lookup"><span data-stu-id="05af4-124">By requesting the **root** relationship, the **DriveItem** that was shared will be returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <span data-ttu-id="05af4-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="05af4-125">Response</span></span>
<a id="response" class="xliff"></a>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

### <span data-ttu-id="05af4-126">Exemplo (pasta compartilhada)</span><span class="sxs-lookup"><span data-stu-id="05af4-126">Example (shared folder)</span></span>
<a id="example-shared-folder" class="xliff"></a>

##### <span data-ttu-id="05af4-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05af4-127">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="05af4-128">Solicitando a relação **root** e expandindo a coleção **children**, o **DriveItem** que foi compartilhado será retornado junto com os arquivos da pasta compartilhada.</span><span class="sxs-lookup"><span data-stu-id="05af4-128">By requesting the **root** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <span data-ttu-id="05af4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="05af4-129">Response</span></span>
<a id="response" class="xliff"></a>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <span data-ttu-id="05af4-130">Transformar uma URL de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="05af4-130">Transform a sharing URL</span></span>
<a id="transform-a-sharing-url" class="xliff"></a>

<span data-ttu-id="05af4-131">Para acessar uma URL compartilhamento usando a API **shares**, a URL deve ser transformada em um token de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="05af4-131">To access a sharing URL using the **shares** API, the URL needs to be transformed into a sharing token.</span></span>

<span data-ttu-id="05af4-132">Transformar uma URL em um token de compartilhamento:</span><span class="sxs-lookup"><span data-stu-id="05af4-132">To transform a URL into a sharing token:</span></span>

1. <span data-ttu-id="05af4-133">Codifique na Base 64 a URL de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="05af4-133">Base64 encode the sharing URL.</span></span>
2. <span data-ttu-id="05af4-134">Converta os dados codificados na Base 64 para o [formato base64url sem preenchimento](https://en.wikipedia.org/wiki/Base64) da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="05af4-134">Convert the base64 encoded data to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by:</span></span>
  1. <span data-ttu-id="05af4-135">Cortar `=` caracteres à direita da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05af4-135">Trim trailing `=` characters from the string</span></span>
  2. <span data-ttu-id="05af4-136">Substitua caracteres não seguros da URL por um caractere equivalente; substitua `/` por `_` e `+` por `-`.</span><span class="sxs-lookup"><span data-stu-id="05af4-136">Replace unsafe URL characters with an equivalent character; replace `/` with `_` and `+` with `-`.</span></span>
3. <span data-ttu-id="05af4-137">Acrescente `u!` ao início da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="05af4-137">Append `u!` to the beginning of the string.</span></span>

<span data-ttu-id="05af4-138">Por exemplo, o seguinte método cC transforma uma cadeia de entrada em um token de compartilhamento:</span><span class="sxs-lookup"><span data-stu-id="05af4-138">For example, the following C# method transforms an input string into a sharing token:</span></span>

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
