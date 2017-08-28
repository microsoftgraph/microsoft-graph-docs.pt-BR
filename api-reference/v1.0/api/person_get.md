# <a name="get-person"></a><span data-ttu-id="97c96-101">Obter pessoa</span><span class="sxs-lookup"><span data-stu-id="97c96-101">Get person</span></span>

<span data-ttu-id="97c96-102">Recupere as propriedades e os relacionamentos de um objeto [person](../resources/person.md).</span><span class="sxs-lookup"><span data-stu-id="97c96-102">Retrieve the properties and relationships of [plannertaskdetails](../resources/person.md) object.</span></span>

<span data-ttu-id="97c96-p101">Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="97c96-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="97c96-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="97c96-105">Permissions</span></span>
<span data-ttu-id="97c96-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97c96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="97c96-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97c96-108">Permission type</span></span>      | <span data-ttu-id="97c96-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97c96-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="97c96-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97c96-110">Delegated (work or school account)</span></span> | <span data-ttu-id="97c96-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="97c96-111">People.Read, People.Read.All</span></span>    | 
|<span data-ttu-id="97c96-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97c96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97c96-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="97c96-113">People.Read</span></span>    | 
|<span data-ttu-id="97c96-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97c96-114">Application</span></span> | <span data-ttu-id="97c96-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="97c96-115">People.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="97c96-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97c96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97c96-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="97c96-117">Optional query parameters</span></span>
|<span data-ttu-id="97c96-118">Nome</span><span class="sxs-lookup"><span data-stu-id="97c96-118">Name</span></span>|<span data-ttu-id="97c96-119">Valor</span><span class="sxs-lookup"><span data-stu-id="97c96-119">Value</span></span>|<span data-ttu-id="97c96-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="97c96-120">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="97c96-121">$filter</span><span class="sxs-lookup"><span data-stu-id="97c96-121">$filter</span></span>|<span data-ttu-id="97c96-122">string</span><span class="sxs-lookup"><span data-stu-id="97c96-122">string</span></span>|<span data-ttu-id="97c96-123">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="97c96-123">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="97c96-124">$orderby</span><span class="sxs-lookup"><span data-stu-id="97c96-124">$orderby</span></span>|<span data-ttu-id="97c96-125">string</span><span class="sxs-lookup"><span data-stu-id="97c96-125">string</span></span>|<span data-ttu-id="97c96-p103">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="97c96-p103">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="97c96-128">$search</span><span class="sxs-lookup"><span data-stu-id="97c96-128">$search</span></span>|<span data-ttu-id="97c96-129">string</span><span class="sxs-lookup"><span data-stu-id="97c96-129">string</span></span>|<span data-ttu-id="97c96-p104">Pesquisar pessoas por nome ou alias. Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="97c96-p104">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="97c96-132">$select</span><span class="sxs-lookup"><span data-stu-id="97c96-132">$select</span></span>|<span data-ttu-id="97c96-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97c96-133">string</span></span>|<span data-ttu-id="97c96-p105">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="97c96-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="97c96-136">$skip</span><span class="sxs-lookup"><span data-stu-id="97c96-136">$skip</span></span>|<span data-ttu-id="97c96-137">int</span><span class="sxs-lookup"><span data-stu-id="97c96-137">int</span></span>|<span data-ttu-id="97c96-p106">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="97c96-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="97c96-140">$top</span><span class="sxs-lookup"><span data-stu-id="97c96-140">$top</span></span>|<span data-ttu-id="97c96-141">int</span><span class="sxs-lookup"><span data-stu-id="97c96-141">int</span></span>|<span data-ttu-id="97c96-142">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="97c96-142">Number of results to be returned.</span></span>|

## <a name="parameters"></a><span data-ttu-id="97c96-143">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="97c96-143">Parameters</span></span>
| <span data-ttu-id="97c96-144">Parâmetro	</span><span class="sxs-lookup"><span data-stu-id="97c96-144">Parameter</span></span> |<span data-ttu-id="97c96-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="97c96-145">Type</span></span>       |<span data-ttu-id="97c96-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="97c96-146">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="97c96-147">property_value</span><span class="sxs-lookup"><span data-stu-id="97c96-147">property_value</span></span>|<span data-ttu-id="97c96-148">String</span><span class="sxs-lookup"><span data-stu-id="97c96-148">String</span></span>     |<span data-ttu-id="97c96-p107">O valor da propriedade estendida a ser correspondida. Obrigatório onde listado na seção **Solicitação HTTP**.</span><span class="sxs-lookup"><span data-stu-id="97c96-p107">The value of the extended property to match. Required where listed in the **HTTP request** section above.</span></span>|
|<span data-ttu-id="97c96-151">person_property</span><span class="sxs-lookup"><span data-stu-id="97c96-151">person_property</span></span>|<span data-ttu-id="97c96-152">String</span><span class="sxs-lookup"><span data-stu-id="97c96-152">String</span></span>    |<span data-ttu-id="97c96-p108">A propriedade person para fazer a correspondência. Obrigatório onde listado na seção **Solicitação HTTP**.</span><span class="sxs-lookup"><span data-stu-id="97c96-p108">The value of the extended property to match. Required where listed in the **HTTP request** section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="97c96-155">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97c96-155">Request headers</span></span>
| <span data-ttu-id="97c96-156">Nome</span><span class="sxs-lookup"><span data-stu-id="97c96-156">Name</span></span>      |<span data-ttu-id="97c96-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="97c96-157">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="97c96-158">Autorização</span><span class="sxs-lookup"><span data-stu-id="97c96-158">Authorization</span></span>  | <span data-ttu-id="97c96-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97c96-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97c96-161">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97c96-161">Request body</span></span>
<span data-ttu-id="97c96-162">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97c96-162">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="97c96-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="97c96-163">Response</span></span>
<span data-ttu-id="97c96-p110">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [person](../resources/person.md) no corpo da resposta. A resposta pode conter uma instância person ou uma coleção de instâncias person.</span><span class="sxs-lookup"><span data-stu-id="97c96-p110">If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body. The response can contain one person instance or a collection of person instances.</span></span> 
## <a name="examples"></a><span data-ttu-id="97c96-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="97c96-166">Examples</span></span>
### <a name="perform-a-search"></a><span data-ttu-id="97c96-167">Realizar uma pesquisa</span><span class="sxs-lookup"><span data-stu-id="97c96-167">Perform a search</span></span> 
<span data-ttu-id="97c96-168">A solicitação a seguir faz uma pesquisa por uma pessoa denominada Clara Barbosa.</span><span class="sxs-lookup"><span data-stu-id="97c96-168">The following request does a search for a person named Irene McGowan.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

<span data-ttu-id="97c96-169">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="97c96-169">The following example shows the formula bar</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="97c96-170">Selecionar os campos a serem retornados em uma resposta filtrada</span><span class="sxs-lookup"><span data-stu-id="97c96-170">Select the fields to return in a filtered response</span></span> 
<span data-ttu-id="97c96-171">Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="97c96-171">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="97c96-p111">O exemplo a seguir obtém **displayName** e **scoredEmailAddresses** das pessoas cujo nome de exibição corresponde ao nome especificado. Neste exemplo, somente as pessoas cujo nome para exibição corresponde a "Lorrie Frye" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="97c96-p111">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="97c96-174">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="97c96-174">The following example shows the formula bar</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        }
    ]
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
