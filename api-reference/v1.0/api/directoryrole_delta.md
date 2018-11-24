# <a name="directoryrole-delta"></a><span data-ttu-id="2e843-101">directoryRole: delta</span><span class="sxs-lookup"><span data-stu-id="2e843-101">directoryRole: delta</span></span>

<span data-ttu-id="2e843-102">Get recentemente criado, atualizado ou excluído funções de diretório sem precisar realizar uma leitura completa do conjunto de recurso inteiro.</span><span class="sxs-lookup"><span data-stu-id="2e843-102">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="2e843-103">Consulte [Usando Delta consulta](../../../concepts/delta_query_overview.md) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="2e843-103">See [Using Delta Query](../../../concepts/delta_query_overview.md) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e843-104">Permissions</span><span class="sxs-lookup"><span data-stu-id="2e843-104">Permissions</span></span>

<span data-ttu-id="2e843-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e843-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="2e843-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e843-107">Permission type</span></span>      | <span data-ttu-id="2e843-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e843-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e843-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e843-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2e843-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2e843-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2e843-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e843-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e843-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e843-112">Not supported.</span></span>    |
|<span data-ttu-id="2e843-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e843-113">Application</span></span> | <span data-ttu-id="2e843-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e843-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e843-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e843-115">HTTP request</span></span>

<span data-ttu-id="2e843-116">Para começar a controlar alterações, você deve fazer uma solicitação, incluindo a função **delta** no recurso [directoryRole](../resources/directoryrole.md) .</span><span class="sxs-lookup"><span data-stu-id="2e843-116">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="2e843-117">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="2e843-117">Query parameters</span></span>

<span data-ttu-id="2e843-118">Controle de alterações provoca uma round de um ou mais chamadas de função **delta** .</span><span class="sxs-lookup"><span data-stu-id="2e843-118">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="2e843-119">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), você deve especificá-lo na solicitação inicial **delta** .</span><span class="sxs-lookup"><span data-stu-id="2e843-119">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="2e843-120">O Microsoft Graph codifica automaticamente quaisquer parâmetros especificados a parte de token do `nextLink` ou `deltaLink` URL fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="2e843-120">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="2e843-121">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="2e843-121">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="2e843-122">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="2e843-122">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="2e843-123">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="2e843-123">Query parameter</span></span>      | <span data-ttu-id="2e843-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e843-124">Type</span></span>   |<span data-ttu-id="2e843-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e843-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2e843-126">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="2e843-126">$deltatoken</span></span> | <span data-ttu-id="2e843-127">string</span><span class="sxs-lookup"><span data-stu-id="2e843-127">string</span></span> | <span data-ttu-id="2e843-128">Um [token de estado](../../../concepts/delta_query_overview.md) retornados no `deltaLink` URL da chamada de função **delta** anterior para o mesmo conjunto de recursos, indicando a conclusão do que round de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="2e843-128">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="2e843-129">Salvar e aplicar a toda a `deltaLink` URL incluindo este token na primeira solicitação da próxima fase de rastreamento para esse conjunto de alterações.</span><span class="sxs-lookup"><span data-stu-id="2e843-129">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="2e843-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="2e843-130">$skiptoken</span></span> | <span data-ttu-id="2e843-131">string</span><span class="sxs-lookup"><span data-stu-id="2e843-131">string</span></span> | <span data-ttu-id="2e843-132">Um [token de estado](../../../concepts/delta_query_overview.md) retornados no `nextLink` URL da chamada de função **delta** anterior, indicando que não há mais alterações a serem rastreados no mesmo conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="2e843-132">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="2e843-133">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="2e843-133">OData query parameters</span></span>

<span data-ttu-id="2e843-134">Este método oferece suporte a OData parâmetros de consulta para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e843-134">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="2e843-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="2e843-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="2e843-137">Não há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="2e843-137">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="2e843-138">A única suportada `$filter` expression é para controle de alterações de recursos específicos, por sua id: `$filter=id+eq+{value}` ou `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="2e843-138">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="2e843-139">O número de identificações, que você pode especificar é limitado pelo comprimento máximo da URL.</span><span class="sxs-lookup"><span data-stu-id="2e843-139">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e843-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e843-140">Request headers</span></span>

| <span data-ttu-id="2e843-141">Nome</span><span class="sxs-lookup"><span data-stu-id="2e843-141">Name</span></span>       | <span data-ttu-id="2e843-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e843-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2e843-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e843-143">Authorization</span></span>  | <span data-ttu-id="2e843-144">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="2e843-144">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="2e843-145">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e843-145">Content-Type</span></span>  | <span data-ttu-id="2e843-146">application/json</span><span class="sxs-lookup"><span data-stu-id="2e843-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e843-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e843-147">Request body</span></span>

<span data-ttu-id="2e843-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e843-148">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="2e843-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e843-149">Response</span></span>

<span data-ttu-id="2e843-150">Se tiver êxito, este método retornará `200 OK` objeto de coleção [directoryRole](../resources/directoryrole.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e843-150">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="2e843-151">A resposta também inclui um `nextLink` URL ou um `deltaLink` URL.</span><span class="sxs-lookup"><span data-stu-id="2e843-151">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="2e843-152">Se um `nextLink` URL é retornado, existem páginas adicionais de dados a ser recuperado na sessão.</span><span class="sxs-lookup"><span data-stu-id="2e843-152">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="2e843-153">O aplicativo continua fazendo solicitações usando o `nextLink` URL até um `deltaLink` URL está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="2e843-153">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="2e843-154">Se um `deltaLink` URL é retornado, não há nenhum dado mais sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="2e843-154">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="2e843-155">Salvar `deltaLink` URL e aplicá-la na próxima chamada **delta** para saber mais sobre as alterações do recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="2e843-155">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="2e843-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e843-156">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2e843-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e843-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="2e843-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e843-158">Response</span></span>

<span data-ttu-id="2e843-p110">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e843-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
      {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="2e843-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="2e843-161">See also</span></span>

- <span data-ttu-id="2e843-162">[Consulta de delta usar para rastrear alterações nos dados do Microsoft Graph](../../../concepts/delta_query_overview.md) para obter mais detalhes</span><span class="sxs-lookup"><span data-stu-id="2e843-162">[Use delta query to track changes in Microsoft Graph data](../../../concepts/delta_query_overview.md) for more details</span></span>
- <span data-ttu-id="2e843-163">[Obter as alterações incrementais para usuários](../../../concepts/delta_query_users.md) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="2e843-163">[Get incremental changes for users](../../../concepts/delta_query_users.md) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->