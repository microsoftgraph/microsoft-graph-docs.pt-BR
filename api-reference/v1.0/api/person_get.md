# <a name="get-person"></a><span data-ttu-id="d50e9-101">Obter pessoa</span><span class="sxs-lookup"><span data-stu-id="d50e9-101">Get person</span></span>

<span data-ttu-id="d50e9-102">Recupere as propriedades e os relacionamentos de um objeto [person](../resources/person.md).</span><span class="sxs-lookup"><span data-stu-id="d50e9-102">Retrieve the properties and relationships of a [person](../resources/person.md) object.</span></span>

<span data-ttu-id="d50e9-p101">Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="d50e9-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d50e9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d50e9-105">Permissions</span></span>
<span data-ttu-id="d50e9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d50e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="d50e9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d50e9-108">Permission type</span></span>      | <span data-ttu-id="d50e9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d50e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d50e9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d50e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d50e9-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="d50e9-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="d50e9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d50e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d50e9-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="d50e9-113">People.Read</span></span>    |
|<span data-ttu-id="d50e9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d50e9-114">Application</span></span> | <span data-ttu-id="d50e9-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="d50e9-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d50e9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d50e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/{id}
GET /users/{id | userPrincipalName}/people/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d50e9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d50e9-117">Optional query parameters</span></span>
<span data-ttu-id="d50e9-118">Este método dá suporte aos seguintes [Parâmetros de consulta OData](../../../concepts/people_example.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d50e9-118">This method supports the [OData Query Parameters](../../../concepts/people_example.md) to help customize the response.</span></span>

|<span data-ttu-id="d50e9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d50e9-119">Name</span></span>|<span data-ttu-id="d50e9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d50e9-120">Value</span></span>|<span data-ttu-id="d50e9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d50e9-121">Description</span></span>| 
|:---------------|:--------|:-------| 
|<span data-ttu-id="d50e9-122">$filter</span><span class="sxs-lookup"><span data-stu-id="d50e9-122">$filter</span></span>|<span data-ttu-id="d50e9-123">string</span><span class="sxs-lookup"><span data-stu-id="d50e9-123">string</span></span>|<span data-ttu-id="d50e9-124">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="d50e9-124">Limits the response to only those people whose record contains the specified criteria.</span></span>| 
|<span data-ttu-id="d50e9-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="d50e9-125">$orderby</span></span>|<span data-ttu-id="d50e9-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d50e9-126">string</span></span>|<span data-ttu-id="d50e9-127">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="d50e9-127">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the $orderby parameter.</span></span> <span data-ttu-id="d50e9-128">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="d50e9-128">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>| 
|<span data-ttu-id="d50e9-129">$search</span><span class="sxs-lookup"><span data-stu-id="d50e9-129">$search</span></span>|<span data-ttu-id="d50e9-130">string</span><span class="sxs-lookup"><span data-stu-id="d50e9-130">string</span></span>|<span data-ttu-id="d50e9-131">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="d50e9-131">Search for people by name or alias. Supports fuzzy matching.</span></span> <span data-ttu-id="d50e9-132">Suporta correspondência difusa</span><span class="sxs-lookup"><span data-stu-id="d50e9-132">Supports Fuzzy matching</span></span>| 
|<span data-ttu-id="d50e9-133">$select</span><span class="sxs-lookup"><span data-stu-id="d50e9-133">$select</span></span>|<span data-ttu-id="d50e9-134">string</span><span class="sxs-lookup"><span data-stu-id="d50e9-134">string</span></span>|<span data-ttu-id="d50e9-p105">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="d50e9-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>| 
|<span data-ttu-id="d50e9-137">$skip</span><span class="sxs-lookup"><span data-stu-id="d50e9-137">$skip</span></span>|<span data-ttu-id="d50e9-138">int</span><span class="sxs-lookup"><span data-stu-id="d50e9-138">int</span></span>|<span data-ttu-id="d50e9-p106">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="d50e9-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>| 
|<span data-ttu-id="d50e9-141">$top</span><span class="sxs-lookup"><span data-stu-id="d50e9-141">$top</span></span>|<span data-ttu-id="d50e9-142">int</span><span class="sxs-lookup"><span data-stu-id="d50e9-142">int</span></span>|<span data-ttu-id="d50e9-143">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="d50e9-143">Number of results to be returned.</span></span>| 

## <a name="request-headers"></a><span data-ttu-id="d50e9-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d50e9-144">Request headers</span></span>
| <span data-ttu-id="d50e9-145">Nome</span><span class="sxs-lookup"><span data-stu-id="d50e9-145">Name</span></span>      |<span data-ttu-id="d50e9-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="d50e9-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d50e9-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="d50e9-147">Authorization</span></span>  | <span data-ttu-id="d50e9-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d50e9-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d50e9-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d50e9-150">Request body</span></span>
<span data-ttu-id="d50e9-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d50e9-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d50e9-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d50e9-152">Response</span></span>
<span data-ttu-id="d50e9-153">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [person](../resources/person.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d50e9-153">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/person.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d50e9-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d50e9-154">Examples</span></span>
#### <a name="request-1"></a><span data-ttu-id="d50e9-155">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="d50e9-155">Request 1</span></span>
<span data-ttu-id="d50e9-156">O seguinte é um exemplo da solicitação que obtém a pessoa que possui essa ID na organização do usuário.</span><span class="sxs-lookup"><span data-stu-id="d50e9-156">The following is an example of the request that gets the person who has this ID in the user's organization.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person_by_id"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people/e3d0513b-449e-4198-ba6f-bd97ae7cae85
```

#### <a name="response-1"></a><span data-ttu-id="d50e9-157">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="d50e9-157">Response 1</span></span>
<span data-ttu-id="d50e9-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d50e9-158">Here is an example of the response.</span></span>

><span data-ttu-id="d50e9-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d50e9-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d50e9-160">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d50e9-160">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_by_id",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 629

{
  "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
  "displayName": "Isaiah Langer",
  "givenName": "Isaiah",
  "surname": "Langer",
  "birthday": "",
  "personNotes": "",
  "isFavorite": false,
  "jobTitle": "Web Marketing Manager",
  "companyName": null,
  "yomiCompany": "",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": "",
  "userPrincipalName": "IsaiahL@contoso.com",
  "imAddress": "sip:isaiahl@contoso.com",
  "scoredEmailAddresses": [
      {
          "address": "IsaiahL@contoso.com",
          "relevanceScore": 20.0
      }
  ],
  "phones": [
      {
          "type": "business",
          "number": "+1 918 555 0101"
      }
  ],
  "postalAddresses": [],
  "websites": [],
  "personType": {
      "class": "Person",
      "subclass": "OrganizationUser"
  }
}
```

#### <a name="request-2"></a><span data-ttu-id="d50e9-161">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="d50e9-161">Request 2</span></span>
<span data-ttu-id="d50e9-162">O seguinte é um exemplo da solicitação que obtém a pessoa que possui essa ID na organização do usuário e restringe a resposta a propriedades selecionadas.</span><span class="sxs-lookup"><span data-stu-id="d50e9-162">The following is an example of the request that gets the person who has this ID in the user's organization and restricts the response to the selected properties.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_by_id_with_select"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people/e3d0513b-449e-4198-ba6f-bd97ae7cae85?$select=displayName
```
#### <a name="response-2"></a><span data-ttu-id="d50e9-163">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="d50e9-163">Response 2</span></span>
<span data-ttu-id="d50e9-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d50e9-164">Here is an example of the response.</span></span>

><span data-ttu-id="d50e9-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d50e9-165">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d50e9-166">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d50e9-166">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_by_id_with_select",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
  "displayName": "Isaiah Langer"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get person",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
