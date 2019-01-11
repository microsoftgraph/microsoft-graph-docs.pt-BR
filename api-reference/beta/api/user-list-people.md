---
title: Listar pessoas
description: Recupere uma lista de objetos de pessoa ordenados por sua relevância para o usuário, que é determinado pelo relacionamentos de negócios e os padrões de colaboração e comunicação do usuário.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 3bd9c8cdd3737cbd8d96fd4f9b24f5382ce04793
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872776"
---
# <a name="list-people"></a><span data-ttu-id="f5415-103">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="f5415-103">List people</span></span>

> <span data-ttu-id="f5415-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5415-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5415-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5415-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5415-106">Recupere uma lista de objetos de [pessoa](../resources/person.md) ordenados por sua relevância para o [usuário](../resources/user.md), que é determinado pelo relacionamentos de negócios e os padrões de colaboração e comunicação do usuário.</span><span class="sxs-lookup"><span data-stu-id="f5415-106">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5415-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f5415-107">Permissions</span></span>

<span data-ttu-id="f5415-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5415-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5415-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5415-110">Permission type</span></span>      | <span data-ttu-id="f5415-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5415-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5415-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5415-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5415-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="f5415-113">People.Read</span></span>    |
|<span data-ttu-id="f5415-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5415-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5415-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="f5415-115">People.Read</span></span>    |
|<span data-ttu-id="f5415-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5415-116">Application</span></span> | <span data-ttu-id="f5415-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5415-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5415-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5415-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f5415-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5415-119">Optional query parameters</span></span>

<span data-ttu-id="f5415-120">Esse método suporta os seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5415-120">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="f5415-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f5415-121">Name</span></span>|<span data-ttu-id="f5415-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f5415-122">Value</span></span>|<span data-ttu-id="f5415-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5415-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="f5415-124">$filter</span><span class="sxs-lookup"><span data-stu-id="f5415-124">$filter</span></span>|<span data-ttu-id="f5415-125">string</span><span class="sxs-lookup"><span data-stu-id="f5415-125">string</span></span>|<span data-ttu-id="f5415-126">Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="f5415-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="f5415-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="f5415-127">$orderby</span></span>|<span data-ttu-id="f5415-128">string</span><span class="sxs-lookup"><span data-stu-id="f5415-128">string</span></span>|<span data-ttu-id="f5415-129">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="f5415-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="f5415-130">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="f5415-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="f5415-131">$search</span><span class="sxs-lookup"><span data-stu-id="f5415-131">$search</span></span>|<span data-ttu-id="f5415-132">string</span><span class="sxs-lookup"><span data-stu-id="f5415-132">string</span></span>|<span data-ttu-id="f5415-133">Pesquisar pessoas por nome ou alias.</span><span class="sxs-lookup"><span data-stu-id="f5415-133">Search for people by name or alias.</span></span> <span data-ttu-id="f5415-134">Suporta correspondência difusa.</span><span class="sxs-lookup"><span data-stu-id="f5415-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="f5415-135">Parâmetro funciona apenas para a pesquisa de pessoas de relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários.</span><span class="sxs-lookup"><span data-stu-id="f5415-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="f5415-136">Também oferece suporte a `topic` palavra-chave para localizar pessoas com base em tópicos extraídos de conversas de email com essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="f5415-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="f5415-137">Consulte a seção de *executar uma pesquisa difusa* em [obter as informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para obter informações e exemplos.</span><span class="sxs-lookup"><span data-stu-id="f5415-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="f5415-138">$select</span><span class="sxs-lookup"><span data-stu-id="f5415-138">$select</span></span>|<span data-ttu-id="f5415-139">string</span><span class="sxs-lookup"><span data-stu-id="f5415-139">string</span></span>|<span data-ttu-id="f5415-p105">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="f5415-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="f5415-142">$skip</span><span class="sxs-lookup"><span data-stu-id="f5415-142">$skip</span></span>|<span data-ttu-id="f5415-143">int</span><span class="sxs-lookup"><span data-stu-id="f5415-143">int</span></span>|<span data-ttu-id="f5415-p106">Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.</span><span class="sxs-lookup"><span data-stu-id="f5415-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="f5415-146">$top</span><span class="sxs-lookup"><span data-stu-id="f5415-146">$top</span></span>|<span data-ttu-id="f5415-147">int</span><span class="sxs-lookup"><span data-stu-id="f5415-147">int</span></span>|<span data-ttu-id="f5415-148">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="f5415-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f5415-149">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5415-149">Request headers</span></span>

| <span data-ttu-id="f5415-150">Nome</span><span class="sxs-lookup"><span data-stu-id="f5415-150">Name</span></span>      |<span data-ttu-id="f5415-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5415-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f5415-152">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5415-152">Authorization</span></span>  | <span data-ttu-id="f5415-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5415-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5415-155">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5415-155">Accept</span></span> | <span data-ttu-id="f5415-156">application/json</span><span class="sxs-lookup"><span data-stu-id="f5415-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5415-157">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5415-157">Request body</span></span>

<span data-ttu-id="f5415-158">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5415-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5415-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5415-159">Response</span></span>

<span data-ttu-id="f5415-160">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos da [pessoa](../resources/person.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5415-160">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5415-161">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f5415-161">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="f5415-162">Procurar</span><span class="sxs-lookup"><span data-stu-id="f5415-162">Browse</span></span>

<span data-ttu-id="f5415-163">As solicitações nesta seção obtém as pessoas importantes para o usuário conectado (`/me`), com base na comunicação, colaboração e relacionamentos de negócios.</span><span class="sxs-lookup"><span data-stu-id="f5415-163">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="f5415-164">Por padrão, cada resposta retorna 10 registros, mas você pode alterar esse número usando o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="f5415-164">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="f5415-165">Essas solicitações exigem a permissão People.Read.</span><span class="sxs-lookup"><span data-stu-id="f5415-165">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="f5415-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5415-166">Request</span></span>

<span data-ttu-id="f5415-167">O exemplo a seguir é um exemplo da solicitação padrão.</span><span class="sxs-lookup"><span data-stu-id="f5415-167">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="f5415-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5415-168">Response</span></span>

<span data-ttu-id="f5415-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5415-169">The following is an example of the response.</span></span>
><span data-ttu-id="f5415-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5415-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="f5415-172">Solicitação de uma página subsequente de pessoas</span><span class="sxs-lookup"><span data-stu-id="f5415-172">Requesting a subsequent page of people</span></span>

<span data-ttu-id="f5415-p110">Se a primeira resposta não contiver a lista completa das pessoas relevantes, você poderá fazer uma segunda solicitação usando *$top* e *$skip* para solicitar páginas adicionais de informações. Se a solicitação anterior tiver informações adicionais, a solicitação a seguir obterá a próxima página de pessoas do servidor.</span><span class="sxs-lookup"><span data-stu-id="f5415-p110">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="f5415-175">Classificar a resposta</span><span class="sxs-lookup"><span data-stu-id="f5415-175">Sort the response</span></span>

<span data-ttu-id="f5415-176">Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta.</span><span class="sxs-lookup"><span data-stu-id="f5415-176">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="f5415-177">Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="f5415-177">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="f5415-178">Essa consulta seleciona as pessoas mais relevantes para você classificando-as pelo nome de exibição e retorna as dez primeiras pessoas da lista classificada.</span><span class="sxs-lookup"><span data-stu-id="f5415-178">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="f5415-179">Alteração do número de pessoas e dos campos retornados</span><span class="sxs-lookup"><span data-stu-id="f5415-179">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="f5415-180">Você pode alterar o número de pessoas retornadas na resposta definindo o parâmetro *$top*.</span><span class="sxs-lookup"><span data-stu-id="f5415-180">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="f5415-181">O exemplo a seguir solicita as 1.000 pessoas mais relevantes para `/me`.</span><span class="sxs-lookup"><span data-stu-id="f5415-181">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="f5415-182">A solicitação também limita a quantidade de dados enviados pelo servidor, solicitando apenas o nome para exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="f5415-182">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="f5415-183">Seleção dos campos que devem ser retornados</span><span class="sxs-lookup"><span data-stu-id="f5415-183">Selecting the fields to return</span></span>

<span data-ttu-id="f5415-184">Você pode limitar a quantidade de dados retornadas do servidor usando o parâmetro *$select* para escolher um ou mais campos.</span><span class="sxs-lookup"><span data-stu-id="f5415-184">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="f5415-185">O campo *@odata.id* é sempre retornado.</span><span class="sxs-lookup"><span data-stu-id="f5415-185">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="f5415-186">O exemplo a seguir limita a resposta à *DisplayName* e *EmailAddress* das pessoas mais relevantes 10.</span><span class="sxs-lookup"><span data-stu-id="f5415-186">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="f5415-187">Uso de um filtro para limitar a resposta</span><span class="sxs-lookup"><span data-stu-id="f5415-187">Using a filter to limit the response</span></span>

<span data-ttu-id="f5415-188">Você pode usar o parâmetro *$filter* para limitar a resposta apenas às pessoas cujo registro contém os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="f5415-188">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="f5415-189">A seguinte consulta limita a resposta às pessoas com a fonte "Diretório".</span><span class="sxs-lookup"><span data-stu-id="f5415-189">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="f5415-190">Selecionar os campos para retornar em uma resposta filtrada</span><span class="sxs-lookup"><span data-stu-id="f5415-190">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="f5415-191">Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f5415-191">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="f5415-192">O exemplo a seguir obtém o *DisplayName* e *EmailAddress* de pessoas cujo nome de exibição é igual ao nome especificado.</span><span class="sxs-lookup"><span data-stu-id="f5415-192">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="f5415-193">Neste exemplo, somente as pessoas cujo nome de exibição é igual a "Nestor Kellum" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="f5415-193">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="f5415-194">Pesquisar pessoas</span><span class="sxs-lookup"><span data-stu-id="f5415-194">Search people</span></span>

<span data-ttu-id="f5415-195">As solicitações nesta seção também obtêm as pessoas importantes para o usuário conectado (`/me`).</span><span class="sxs-lookup"><span data-stu-id="f5415-195">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="f5415-196">Solicitações de pesquisa exigem a permissão People.Read.</span><span class="sxs-lookup"><span data-stu-id="f5415-196">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="f5415-197">Usando a pesquisa para selecionar as pessoas</span><span class="sxs-lookup"><span data-stu-id="f5415-197">Using search to select people</span></span>

<span data-ttu-id="f5415-198">Use o parâmetro *$search* para selecionar as pessoas que atendem a determinado conjunto de critérios.</span><span class="sxs-lookup"><span data-stu-id="f5415-198">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="f5415-199">A seguinte consulta de pesquisa retorna pessoas relevantes para `/me` cujos GivenName ou sobrenome começa com a letra "j".</span><span class="sxs-lookup"><span data-stu-id="f5415-199">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="f5415-200">Uso da pesquisa para especificar um tópico relevante</span><span class="sxs-lookup"><span data-stu-id="f5415-200">Using search to specify a relevant topic</span></span>

<span data-ttu-id="f5415-201">A solicitação a seguir retorna a pessoas relevantes para `/me` cujos nomes contêm "ma" e que têm uma associação com "planejamento do recurso".</span><span class="sxs-lookup"><span data-stu-id="f5415-201">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="f5415-202">Execução de uma pesquisa difusa</span><span class="sxs-lookup"><span data-stu-id="f5415-202">Performing a fuzzy search</span></span>

<span data-ttu-id="f5415-203">A solicitação a seguir faz uma pesquisa de uma pessoa chamada "Saguão Hermaini."</span><span class="sxs-lookup"><span data-stu-id="f5415-203">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="f5415-204">Como há uma pessoa chamada "Herminia Hull" relevantes para o usuário conectado, as informações de "Herminia Hull" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="f5415-204">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="f5415-205">Pessoas relacionadas</span><span class="sxs-lookup"><span data-stu-id="f5415-205">Related people</span></span>

<span data-ttu-id="f5415-206">A solicitação a seguir obtém as pessoas importantes para outra pessoa na organização do usuário.</span><span class="sxs-lookup"><span data-stu-id="f5415-206">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="f5415-207">Esta solicitação requer o User.ReadBasic.All para People.Read.All permissão.</span><span class="sxs-lookup"><span data-stu-id="f5415-207">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="f5415-208">Neste exemplo, as pessoas de relevantes do Nestor Kellum são exibidas.</span><span class="sxs-lookup"><span data-stu-id="f5415-208">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
