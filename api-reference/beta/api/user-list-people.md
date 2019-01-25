---
title: Listar pessoas
description: Recupere uma lista de objetos de pessoa ordenados por sua relevância para o usuário, que é determinado pelo relacionamentos de negócios e os padrões de colaboração e comunicação do usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: deb9fd929a2b0b8ce4da9392cb465497c2236b0c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517810"
---
# <a name="list-people"></a><span data-ttu-id="9f65f-103">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="9f65f-103">List people</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f65f-104">Recupere uma lista de objetos de [pessoa](../resources/person.md) ordenados por sua relevância para o [usuário](../resources/user.md), que é determinado pelo relacionamentos de negócios e os padrões de colaboração e comunicação do usuário.</span><span class="sxs-lookup"><span data-stu-id="9f65f-104">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f65f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f65f-105">Permissions</span></span>

<span data-ttu-id="9f65f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f65f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f65f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f65f-108">Permission type</span></span>      | <span data-ttu-id="9f65f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f65f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f65f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f65f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f65f-111">People.Read</span><span class="sxs-lookup"><span data-stu-id="9f65f-111">People.Read</span></span>    |
|<span data-ttu-id="9f65f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f65f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f65f-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="9f65f-113">People.Read</span></span>    |
|<span data-ttu-id="9f65f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f65f-114">Application</span></span> | <span data-ttu-id="9f65f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f65f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f65f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f65f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f65f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9f65f-117">Optional query parameters</span></span>

<span data-ttu-id="9f65f-118">Esse método suporta os seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9f65f-118">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="9f65f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9f65f-119">Name</span></span>|<span data-ttu-id="9f65f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9f65f-120">Value</span></span>|<span data-ttu-id="9f65f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f65f-121">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="9f65f-122">$filter</span><span class="sxs-lookup"><span data-stu-id="9f65f-122">$filter</span></span>|<span data-ttu-id="9f65f-123">string</span><span class="sxs-lookup"><span data-stu-id="9f65f-123">string</span></span>|<span data-ttu-id="9f65f-124">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="9f65f-124">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="9f65f-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="9f65f-125">$orderby</span></span>|<span data-ttu-id="9f65f-126">string</span><span class="sxs-lookup"><span data-stu-id="9f65f-126">string</span></span>|<span data-ttu-id="9f65f-127">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="9f65f-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="9f65f-128">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="9f65f-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="9f65f-129">$search</span><span class="sxs-lookup"><span data-stu-id="9f65f-129">$search</span></span>|<span data-ttu-id="9f65f-130">string</span><span class="sxs-lookup"><span data-stu-id="9f65f-130">string</span></span>|<span data-ttu-id="9f65f-131">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="9f65f-131">Search for people by name or alias.</span></span> <span data-ttu-id="9f65f-132">Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="9f65f-132">Supports Fuzzy matching.</span></span> <span data-ttu-id="9f65f-133">Parâmetro funciona apenas para a pesquisa de pessoas de relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários.</span><span class="sxs-lookup"><span data-stu-id="9f65f-133">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="9f65f-134">Também oferece suporte a `topic` palavra-chave para localizar pessoas com base em tópicos extraídos de conversas de email com essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="9f65f-134">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="9f65f-135">Consulte a seção de *executar uma pesquisa difusa* em [obter as informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para obter informações e exemplos.</span><span class="sxs-lookup"><span data-stu-id="9f65f-135">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="9f65f-136">$select</span><span class="sxs-lookup"><span data-stu-id="9f65f-136">$select</span></span>|<span data-ttu-id="9f65f-137">string</span><span class="sxs-lookup"><span data-stu-id="9f65f-137">string</span></span>|<span data-ttu-id="9f65f-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="9f65f-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="9f65f-140">$skip</span><span class="sxs-lookup"><span data-stu-id="9f65f-140">$skip</span></span>|<span data-ttu-id="9f65f-141">int</span><span class="sxs-lookup"><span data-stu-id="9f65f-141">int</span></span>|<span data-ttu-id="9f65f-p105">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="9f65f-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="9f65f-144">$top</span><span class="sxs-lookup"><span data-stu-id="9f65f-144">$top</span></span>|<span data-ttu-id="9f65f-145">int</span><span class="sxs-lookup"><span data-stu-id="9f65f-145">int</span></span>|<span data-ttu-id="9f65f-146">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="9f65f-146">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9f65f-147">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f65f-147">Request headers</span></span>

| <span data-ttu-id="9f65f-148">Nome</span><span class="sxs-lookup"><span data-stu-id="9f65f-148">Name</span></span>      |<span data-ttu-id="9f65f-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f65f-149">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9f65f-150">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f65f-150">Authorization</span></span>  | <span data-ttu-id="9f65f-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f65f-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f65f-153">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f65f-153">Accept</span></span> | <span data-ttu-id="9f65f-154">application/json</span><span class="sxs-lookup"><span data-stu-id="9f65f-154">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f65f-155">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f65f-155">Request body</span></span>

<span data-ttu-id="9f65f-156">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f65f-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f65f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f65f-157">Response</span></span>

<span data-ttu-id="9f65f-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos da [pessoa](../resources/person.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f65f-158">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f65f-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9f65f-159">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="9f65f-160">Procurar</span><span class="sxs-lookup"><span data-stu-id="9f65f-160">Browse</span></span>

<span data-ttu-id="9f65f-161">As solicitações nesta seção obtém as pessoas importantes para o usuário conectado (`/me`), com base na comunicação, colaboração e relacionamentos de negócios.</span><span class="sxs-lookup"><span data-stu-id="9f65f-161">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="9f65f-162">Por padrão, cada resposta retorna 10 registros, mas você pode *alterar esse número* usando o parâmetro $top.</span><span class="sxs-lookup"><span data-stu-id="9f65f-162">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="9f65f-163">Essas solicitações exigem a permissão People.Read.</span><span class="sxs-lookup"><span data-stu-id="9f65f-163">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="9f65f-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f65f-164">Request</span></span>

<span data-ttu-id="9f65f-165">O exemplo a seguir é um exemplo da solicitação padrão.</span><span class="sxs-lookup"><span data-stu-id="9f65f-165">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="9f65f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f65f-166">Response</span></span>

<span data-ttu-id="9f65f-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f65f-167">The following is an example of the response.</span></span>
><span data-ttu-id="9f65f-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f65f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
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
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="9f65f-170"> Solicitação de uma página subsequente de pessoas</span><span class="sxs-lookup"><span data-stu-id="9f65f-170">Requesting a subsequent page of people</span></span>

<span data-ttu-id="9f65f-p109">Se a primeira resposta não contiver a lista completa das pessoas relevantes, você poderá fazer uma segunda solicitação usando *$top* e *$skip* para solicitar páginas adicionais de informações. Se a solicitação anterior tiver informações adicionais, a solicitação a seguir obterá a próxima página de pessoas do servidor.</span><span class="sxs-lookup"><span data-stu-id="9f65f-p109">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="9f65f-173">Classificar a resposta</span><span class="sxs-lookup"><span data-stu-id="9f65f-173">Sort the response</span></span>

<span data-ttu-id="9f65f-174">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="9f65f-174">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="9f65f-175">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="9f65f-175">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="9f65f-176">Essa consulta seleciona as pessoas mais relevantes para você classificando-as pelo nome de exibição e retorna as dez primeiras pessoas da lista classificada.</span><span class="sxs-lookup"><span data-stu-id="9f65f-176">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="9f65f-177"> Alteração do número de pessoas e dos campos retornados</span><span class="sxs-lookup"><span data-stu-id="9f65f-177">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="9f65f-178">Você pode alterar o número de pessoas retornadas na resposta definindo o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="9f65f-178">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="9f65f-179">O exemplo a seguir solicita as 1.000 pessoas mais relevantes para `/me`.</span><span class="sxs-lookup"><span data-stu-id="9f65f-179">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="9f65f-180">A solicitação também limita a quantidade de dados enviados pelo servidor, solicitando apenas o nome para exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="9f65f-180">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="9f65f-181"> Seleção dos campos que devem ser retornados</span><span class="sxs-lookup"><span data-stu-id="9f65f-181">Selecting the fields to return</span></span>

<span data-ttu-id="9f65f-182">Você pode limitar a quantidade de dados retornadas do servidor usando o parâmetro *$select* para escolher um ou mais campos.</span><span class="sxs-lookup"><span data-stu-id="9f65f-182">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="9f65f-183">O campo *@odata.id* é sempre retornado.</span><span class="sxs-lookup"><span data-stu-id="9f65f-183">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="9f65f-184">O exemplo a seguir limita a resposta à *DisplayName* e *EmailAddress* das pessoas mais relevantes 10.</span><span class="sxs-lookup"><span data-stu-id="9f65f-184">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="9f65f-185"> Uso de um filtro para limitar a resposta</span><span class="sxs-lookup"><span data-stu-id="9f65f-185">Using a filter to limit the response</span></span>

<span data-ttu-id="9f65f-186">Você pode usar o parâmetro *$filter* para limitar a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="9f65f-186">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="9f65f-187">A seguinte consulta limita a resposta às pessoas com a fonte "Diretório".</span><span class="sxs-lookup"><span data-stu-id="9f65f-187">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="9f65f-188">Selecionar os campos para retornar em uma resposta filtrada</span><span class="sxs-lookup"><span data-stu-id="9f65f-188">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="9f65f-189">Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f65f-189">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="9f65f-190">O exemplo a seguir obtém o *DisplayName* e *EmailAddress* de pessoas cujo nome de exibição é igual ao nome especificado.</span><span class="sxs-lookup"><span data-stu-id="9f65f-190">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="9f65f-191">Neste exemplo, somente as pessoas cujo nome de exibição é igual a "Nestor Kellum" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="9f65f-191">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="9f65f-192">Pesquisar pessoas</span><span class="sxs-lookup"><span data-stu-id="9f65f-192">Search people</span></span>

<span data-ttu-id="9f65f-193">As solicitações nesta seção também obtêm as pessoas importantes para o usuário conectado (`/me`).</span><span class="sxs-lookup"><span data-stu-id="9f65f-193">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="9f65f-194">Solicitações de pesquisa exigem a permissão People.Read.</span><span class="sxs-lookup"><span data-stu-id="9f65f-194">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="9f65f-195">Usando a pesquisa para selecionar as pessoas</span><span class="sxs-lookup"><span data-stu-id="9f65f-195">Using search to select people</span></span>

<span data-ttu-id="9f65f-196">Use o parâmetro *$search* para selecionar as pessoas que atendem a determinado conjunto de critérios.</span><span class="sxs-lookup"><span data-stu-id="9f65f-196">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="9f65f-197">A seguinte consulta de pesquisa retorna pessoas relevantes para `/me` cujos GivenName ou sobrenome começa com a letra "j".</span><span class="sxs-lookup"><span data-stu-id="9f65f-197">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="9f65f-198"> Uso da pesquisa para especificar um tópico relevante</span><span class="sxs-lookup"><span data-stu-id="9f65f-198">Using search to specify a relevant topic</span></span>

<span data-ttu-id="9f65f-199">A solicitação a seguir retorna a pessoas relevantes para `/me` cujos nomes contêm "ma" e que têm uma associação com "planejamento do recurso".</span><span class="sxs-lookup"><span data-stu-id="9f65f-199">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="9f65f-200">  Execução de uma pesquisa difusa</span><span class="sxs-lookup"><span data-stu-id="9f65f-200">Performing a fuzzy search</span></span>

<span data-ttu-id="9f65f-201">A solicitação a seguir faz uma pesquisa de uma pessoa chamada "Saguão Hermaini."</span><span class="sxs-lookup"><span data-stu-id="9f65f-201">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="9f65f-202">Como há uma pessoa chamada "Herminia Hull" relevantes para o usuário conectado, as informações de "Herminia Hull" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="9f65f-202">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="9f65f-203">Pessoas relacionadas</span><span class="sxs-lookup"><span data-stu-id="9f65f-203">Related people</span></span>

<span data-ttu-id="9f65f-204">A solicitação a seguir obtém as pessoas importantes para outra pessoa na organização do usuário.</span><span class="sxs-lookup"><span data-stu-id="9f65f-204">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="9f65f-205">Esta solicitação requer o User.ReadBasic.All para People.Read.All permissão.</span><span class="sxs-lookup"><span data-stu-id="9f65f-205">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="9f65f-206">Neste exemplo, as pessoas de relevantes do Nestor Kellum são exibidas.</span><span class="sxs-lookup"><span data-stu-id="9f65f-206">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-people.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
