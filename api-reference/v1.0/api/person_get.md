# <a name="get-person"></a><span data-ttu-id="93bb3-101">Obter pessoa</span><span class="sxs-lookup"><span data-stu-id="93bb3-101">Get person</span></span>

<span data-ttu-id="93bb3-102">Recupere as propriedades e os relacionamentos de um objeto [person](../resources/person.md).</span><span class="sxs-lookup"><span data-stu-id="93bb3-102">Retrieve the properties and relationships of [plannerAssignedToTaskBoardTaskFormat](../resources/person.md) object.</span></span>

<span data-ttu-id="93bb3-p101">Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="93bb3-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93bb3-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93bb3-105">Prerequisites</span></span>
<span data-ttu-id="93bb3-106">As **permissões** a seguir são necessárias para executar partes dessa API: *People.Read*; *People.Read.All*</span><span class="sxs-lookup"><span data-stu-id="93bb3-106">The following **permissions** are required to execute portions of this API: *People.Read*; *People.Read.All*</span></span>
 
## <a name="http-request"></a><span data-ttu-id="93bb3-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93bb3-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93bb3-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="93bb3-108">Optional query parameters</span></span>
|<span data-ttu-id="93bb3-109">Nome</span><span class="sxs-lookup"><span data-stu-id="93bb3-109">Name</span></span>|<span data-ttu-id="93bb3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="93bb3-110">Value</span></span>|<span data-ttu-id="93bb3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="93bb3-111">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="93bb3-112">$filter</span><span class="sxs-lookup"><span data-stu-id="93bb3-112">$filter</span></span>|<span data-ttu-id="93bb3-113">string</span><span class="sxs-lookup"><span data-stu-id="93bb3-113">string</span></span>|<span data-ttu-id="93bb3-114">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="93bb3-114">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="93bb3-115">$orderby</span><span class="sxs-lookup"><span data-stu-id="93bb3-115">$orderby</span></span>|<span data-ttu-id="93bb3-116">string</span><span class="sxs-lookup"><span data-stu-id="93bb3-116">string</span></span>|<span data-ttu-id="93bb3-p102">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="93bb3-p102">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="93bb3-119">$search</span><span class="sxs-lookup"><span data-stu-id="93bb3-119">$search</span></span>|<span data-ttu-id="93bb3-120">string</span><span class="sxs-lookup"><span data-stu-id="93bb3-120">string</span></span>|<span data-ttu-id="93bb3-p103">Pesquisar pessoas por nome ou alias. Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="93bb3-p103">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="93bb3-123">$select</span><span class="sxs-lookup"><span data-stu-id="93bb3-123">$select</span></span>|<span data-ttu-id="93bb3-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93bb3-124">string</span></span>|<span data-ttu-id="93bb3-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="93bb3-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="93bb3-127">$skip</span><span class="sxs-lookup"><span data-stu-id="93bb3-127">$skip</span></span>|<span data-ttu-id="93bb3-128">int</span><span class="sxs-lookup"><span data-stu-id="93bb3-128">int</span></span>|<span data-ttu-id="93bb3-p105">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="93bb3-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="93bb3-131">$top</span><span class="sxs-lookup"><span data-stu-id="93bb3-131">$top</span></span>|<span data-ttu-id="93bb3-132">int</span><span class="sxs-lookup"><span data-stu-id="93bb3-132">int</span></span>|<span data-ttu-id="93bb3-133">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="93bb3-133">Number of results to be returned.</span></span>|

## <a name="parameters"></a><span data-ttu-id="93bb3-134">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="93bb3-134">Parameters</span></span>
| <span data-ttu-id="93bb3-135">Parâmetro	</span><span class="sxs-lookup"><span data-stu-id="93bb3-135">Parameter</span></span> |<span data-ttu-id="93bb3-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="93bb3-136">Type</span></span>       |<span data-ttu-id="93bb3-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="93bb3-137">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="93bb3-138">property_value</span><span class="sxs-lookup"><span data-stu-id="93bb3-138">property_value</span></span>|<span data-ttu-id="93bb3-139">String</span><span class="sxs-lookup"><span data-stu-id="93bb3-139">String</span></span>     |<span data-ttu-id="93bb3-p106">O valor da propriedade estendida a ser correspondida. Obrigatório onde listado na seção **Solicitação HTTP**.</span><span class="sxs-lookup"><span data-stu-id="93bb3-p106">The value of the extended property to match. Required where listed in the HTTP request section above.</span></span>|
|<span data-ttu-id="93bb3-142">person_property</span><span class="sxs-lookup"><span data-stu-id="93bb3-142">person_property</span></span>|<span data-ttu-id="93bb3-143">String</span><span class="sxs-lookup"><span data-stu-id="93bb3-143">String</span></span>    |<span data-ttu-id="93bb3-p107">A propriedade person para fazer a correspondência. Obrigatório onde listado na seção **Solicitação HTTP**.</span><span class="sxs-lookup"><span data-stu-id="93bb3-p107">The value of the extended property to match. Required where listed in the HTTP request section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="93bb3-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93bb3-146">Request headers</span></span>
| <span data-ttu-id="93bb3-147">Nome</span><span class="sxs-lookup"><span data-stu-id="93bb3-147">Name</span></span>      |<span data-ttu-id="93bb3-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="93bb3-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="93bb3-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="93bb3-149">Authorization</span></span>  | <span data-ttu-id="93bb3-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93bb3-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93bb3-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93bb3-152">Request body</span></span>
<span data-ttu-id="93bb3-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93bb3-153">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="93bb3-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="93bb3-154">Response</span></span>
<span data-ttu-id="93bb3-p109">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [person](../resources/person.md) no corpo da resposta. A resposta pode conter uma instância person ou uma coleção de instâncias person.</span><span class="sxs-lookup"><span data-stu-id="93bb3-p109">If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body. The response can contain one person instance or a collection of person instances.</span></span> 
## <a name="examples"></a><span data-ttu-id="93bb3-157">Exemplos</span><span class="sxs-lookup"><span data-stu-id="93bb3-157">Examples</span></span>
### <a name="perform-a-search"></a><span data-ttu-id="93bb3-158">Realizar uma pesquisa</span><span class="sxs-lookup"><span data-stu-id="93bb3-158">Perform a search</span></span> 
<span data-ttu-id="93bb3-159">A solicitação a seguir faz uma pesquisa por uma pessoa denominada Clara Barbosa.</span><span class="sxs-lookup"><span data-stu-id="93bb3-159">The following request does a search for a person named Irene McGowan.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

<span data-ttu-id="93bb3-160">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="93bb3-160">The following example shows the formula bar</span></span> 

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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="93bb3-161">Selecionar os campos a serem retornados em uma resposta filtrada</span><span class="sxs-lookup"><span data-stu-id="93bb3-161">Select the fields to return in a filtered response</span></span> 
<span data-ttu-id="93bb3-162">Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="93bb3-162">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="93bb3-p110">O exemplo a seguir obtém **displayName** e **scoredEmailAddresses** das pessoas cujo nome de exibição corresponde ao nome especificado. Neste exemplo, somente as pessoas cujo nome para exibição corresponde a "Lorrie Frye" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="93bb3-p110">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="93bb3-165">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="93bb3-165">The following example shows the formula bar</span></span> 

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
