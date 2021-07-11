---
title: Use o parâmetro de consulta $search no Microsoft Graph
description: Microsoft Graph dá suporte ao parâmetro de consulta $search OData para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: c552f510eb65370cd331784c98ea7359b278a56d
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367007"
---
# <a name="use-the-search-query-parameter-to-match-a-search-criterion"></a><span data-ttu-id="49033-103">Usar o parâmetro de consulta de pesquisa para corresponder a um critério de pesquisa</span><span class="sxs-lookup"><span data-stu-id="49033-103">Use the search query parameter to match a search criterion</span></span>

<span data-ttu-id="49033-104">Além de [outros parâmetros de consulta OData](/graph/query-parameters), o Microsoft Graph dá suporte ao parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="49033-104">In addition to [other OData query parameters](/graph/query-parameters), Microsoft Graph supports the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

<span data-ttu-id="49033-105">O suporte para o parâmetro de consulta `$search` varia de acordo com a entidade, com alguns, como recursos do Microsoft Azure Active Directory que derivam de [directoryObject](/graph/api/resources/directoryobject), dando suporte a `$search` somente em [consultas avançadas](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="49033-105">The support for the `$search` query parameter varies by entity, with some, such as Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), supporting `$search` only in [advanced queries](/graph/aad-advanced-queries).</span></span>

> [!NOTE]
> <span data-ttu-id="49033-106">O parâmetro de consulta `$search` não está disponível no momento nos locatários Azure AD B2C. </span><span class="sxs-lookup"><span data-stu-id="49033-106">The `$search` query parameter is currently not available in Azure AD B2C tenants.</span></span>

## <a name="using-search-on-message-collections"></a><span data-ttu-id="49033-107">Usando $search em conjuntos de mensagens</span><span class="sxs-lookup"><span data-stu-id="49033-107">Using $search on message collections</span></span>

<span data-ttu-id="49033-108">Você pode pesquisar mensagens com base em um valor nas propriedades de mensagens específicas.</span><span class="sxs-lookup"><span data-stu-id="49033-108">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="49033-109">Os resultados da pesquisa são classificados pela data e hora em que a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="49033-109">The results of the search are sorted by the date and time that the message was sent.</span></span> <span data-ttu-id="49033-110">Uma solicitação de `$search` retorna até 250 resultados.</span><span class="sxs-lookup"><span data-stu-id="49033-110">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="49033-111">Se você realizar uma pesquisa em mensagens e especificar apenas um valor sem as propriedades de mensagens específicas, a pesquisa será realizada nas propriedades de pesquisa padrão **from**, **subject** e **body**.</span><span class="sxs-lookup"><span data-stu-id="49033-111">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="49033-112">O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:</span><span class="sxs-lookup"><span data-stu-id="49033-112">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="49033-113">Como alternativa, você pode pesquisar mensagens especificando os nomes de propriedade da mensagem na tabela a seguir, que são reconhecidos pela sintaxe da Linguagem de Consulta de Palavra-chave (KQL).</span><span class="sxs-lookup"><span data-stu-id="49033-113">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="49033-114">Esses nomes de propriedades correspondem às propriedades definidas na entidade **mensagem** do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="49033-114">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="49033-115">O Outlook e outros aplicativos do Microsoft 365 como o SharePoint são compatíveis com a sintaxe KQL, proporcionando a conveniência de um domínio de descoberta comum para seus repositórios de dados.</span><span class="sxs-lookup"><span data-stu-id="49033-115">Outlook and other Microsoft 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="49033-116">Propriedades de emails pesquisáveis</span><span class="sxs-lookup"><span data-stu-id="49033-116">Searchable email property</span></span>                | <span data-ttu-id="49033-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="49033-117">Description</span></span> | <span data-ttu-id="49033-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49033-118">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="49033-119">**attachment**</span><span class="sxs-lookup"><span data-stu-id="49033-119">**attachment**</span></span>           | <span data-ttu-id="49033-120">Os nomes dos arquivos anexados a uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="49033-120">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="49033-121">**bcc**</span><span class="sxs-lookup"><span data-stu-id="49033-121">**bcc**</span></span>           | <span data-ttu-id="49033-122">O campo **Cco** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="49033-122">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="49033-123">**body**</span><span class="sxs-lookup"><span data-stu-id="49033-123">**body**</span></span>           | <span data-ttu-id="49033-124">O corpo de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="49033-124">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="49033-125">**cc**</span><span class="sxs-lookup"><span data-stu-id="49033-125">**cc**</span></span>           | <span data-ttu-id="49033-126">O campo **Cc** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="49033-126">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="49033-127">**from**</span><span class="sxs-lookup"><span data-stu-id="49033-127">**from**</span></span>           | <span data-ttu-id="49033-128">O remetente de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="49033-128">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="49033-129">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="49033-129">**hasAttachment**</span></span> | <span data-ttu-id="49033-130">Verdadeiro se uma mensagem de email contiver um anexo que não seja um anexo embutido, caso contrário, falso.</span><span class="sxs-lookup"><span data-stu-id="49033-130">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments:true"`][search-from-example]
| <span data-ttu-id="49033-131">**importance**</span><span class="sxs-lookup"><span data-stu-id="49033-131">**importance**</span></span>           | <span data-ttu-id="49033-132">A prioridade de uma mensagem de email, que um remetente pode especificar ao enviar uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="49033-132">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="49033-133">Os valores possíveis são `low`, `medium` ou `high`.</span><span class="sxs-lookup"><span data-stu-id="49033-133">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="49033-134">**kind**</span><span class="sxs-lookup"><span data-stu-id="49033-134">**kind**</span></span>           | <span data-ttu-id="49033-135">O tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="49033-135">The type of message.</span></span> <span data-ttu-id="49033-136">Os valores possíveis são `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` ou `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="49033-136">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="49033-137">**participants**</span><span class="sxs-lookup"><span data-stu-id="49033-137">**participants**</span></span>           | <span data-ttu-id="49033-138">Os campos **de**, **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="49033-138">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="49033-139">**received**</span><span class="sxs-lookup"><span data-stu-id="49033-139">**received**</span></span>           | <span data-ttu-id="49033-140">A data em que uma mensagem de email foi recebida pelo destinatário.</span><span class="sxs-lookup"><span data-stu-id="49033-140">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="49033-141">**recipients**</span><span class="sxs-lookup"><span data-stu-id="49033-141">**recipients**</span></span>           | <span data-ttu-id="49033-142">Os campos **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="49033-142">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="49033-143">**sent**</span><span class="sxs-lookup"><span data-stu-id="49033-143">**sent**</span></span>           | <span data-ttu-id="49033-144">A data em que uma mensagem de email foi enviada pelo remetente.</span><span class="sxs-lookup"><span data-stu-id="49033-144">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="49033-145">**size**</span><span class="sxs-lookup"><span data-stu-id="49033-145">**size**</span></span>           | <span data-ttu-id="49033-146">O tamanho de um item em bytes.</span><span class="sxs-lookup"><span data-stu-id="49033-146">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="49033-147">**subject**</span><span class="sxs-lookup"><span data-stu-id="49033-147">**subject**</span></span>           | <span data-ttu-id="49033-p105">O texto na linha de assunto de uma mensagem de email. .</span><span class="sxs-lookup"><span data-stu-id="49033-p105">The text in the subject line of an email message. .</span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="49033-150">**to**</span><span class="sxs-lookup"><span data-stu-id="49033-150">**to**</span></span>           | <span data-ttu-id="49033-151">O campo **para** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.</span><span class="sxs-lookup"><span data-stu-id="49033-151">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="49033-152">Para saber mais sobre as propriedades de email pesquisáveis, KQL como a sintaxe, operadores com suporte e dicas de pesquisa, confira os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="49033-152">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="49033-153">[Propriedades pesquisáveis no Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span><span class="sxs-lookup"><span data-stu-id="49033-153">[Searchable properties in Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="49033-154">Referência de sintaxe da Linguagem de Consulta de Palavra-chave (KQL)</span><span class="sxs-lookup"><span data-stu-id="49033-154">Keyword Query Language (KQL) syntax reference</span></span>](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- [<span data-ttu-id="49033-155">Propriedades da mensagem e operadores de pesquisa para a Descoberta eletrônica In-loco no Exchange 2016</span><span class="sxs-lookup"><span data-stu-id="49033-155">Message properties and search operators for In-Place eDiscovery in Exchange 2016</span></span>](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators)

## <a name="using-search-on-person-collections"></a><span data-ttu-id="49033-156">Usando $search em conjuntos de pessoas</span><span class="sxs-lookup"><span data-stu-id="49033-156">Using $search on person collections</span></span>

<span data-ttu-id="49033-157">Você pode usar a [API de Pessoas](/graph/api/resources/person) do Microsoft Graph para recuperar as pessoas mais relevantes para um usuário.</span><span class="sxs-lookup"><span data-stu-id="49033-157">You can use the Microsoft Graph [People API](/graph/api/resources/person) to retrieve the people who are most relevant to a user.</span></span> <span data-ttu-id="49033-158">A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="49033-158">Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="49033-159">A API de Pessoas é compatível com o parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="49033-159">The People API supports the `$search` query parameter.</span></span> <span data-ttu-id="49033-160">Uma solicitação de `$search` retorna até 250 resultados.</span><span class="sxs-lookup"><span data-stu-id="49033-160">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="49033-161">As pesquisas de pessoas ocorrem nas propriedades **displayName** e **emailAddress** do recurso [person](/graph/api/resources/person).</span><span class="sxs-lookup"><span data-stu-id="49033-161">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person) resource.</span></span>

<span data-ttu-id="49033-162">A seguinte solicitação faz uma pesquisa por uma pessoa chamada "Clara Barbosa" nas propriedades **displayName** e **emailAddress** em todos os indivíduos no conjunto de **Pessoas** do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="49033-162">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="49033-163">Como uma pessoa denominada "Clara Barbosa" é relevante para o usuário conectado, as informações para "Clara Barbosa" são retornadas.</span><span class="sxs-lookup"><span data-stu-id="49033-163">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="49033-164">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="49033-164">The following example shows the response.</span></span> 

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

<span data-ttu-id="49033-165">Saiba mais sobre a API de Pessoas em [Obter informações sobre pessoas relevantes](./people-example.md#search-people).</span><span class="sxs-lookup"><span data-stu-id="49033-165">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

## <a name="using-search-on-directory-object-collections"></a><span data-ttu-id="49033-166">Como usar $search nos conjuntos de objetos do diretório</span><span class="sxs-lookup"><span data-stu-id="49033-166">Using $search on directory object collections</span></span>

<span data-ttu-id="49033-167">Os recursos do Microsoft Azure Active Directory e suas relações que derivam de [directoryObject](/graph/api/resources/directoryobject) dão suporte ao parâmetro de consulta `$search` somente em consultas avançadas.</span><span class="sxs-lookup"><span data-stu-id="49033-167">Azure AD resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject) support the `$search` query parameter only in advanced queries.</span></span> <span data-ttu-id="49033-168">A pesquisa usa uma abordagem de geração de tokens que funciona extraindo palavras da cadeia de caracteres de entrada e saída, usando espaços, números, maiúsculas e minúsculas diferentes e símbolos para separar as palavras, da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="49033-168">The search uses a tokenization approach which works by extracting words from your input and output string, using spaces, numbers, different casing, and symbols to separate the words, as follows:</span></span>

* <span data-ttu-id="49033-169">**Espaços**: `hello world` => `hello`, `world`</span><span class="sxs-lookup"><span data-stu-id="49033-169">**Spaces**: `hello world` => `hello`, `world`</span></span>
* <span data-ttu-id="49033-170">**Caixa diferente**⁽¹⁾: `HelloWorld` ou `helloWORLD` => `hello`, `world`</span><span class="sxs-lookup"><span data-stu-id="49033-170">**Different casing**⁽¹⁾: `HelloWorld` or `helloWORLD` => `hello`, `world`</span></span>
* <span data-ttu-id="49033-171">**Símbolos**⁽²⁾: `hello.world` => `hello`, `.`,`world`, `helloworld`</span><span class="sxs-lookup"><span data-stu-id="49033-171">**Symbols**⁽²⁾: `hello.world` => `hello`, `.`, `world`, `helloworld`</span></span>
* <span data-ttu-id="49033-172">**Números**: `hello123world` => `hello`,`123`, `world`</span><span class="sxs-lookup"><span data-stu-id="49033-172">**Numbers**: `hello123world` => `hello`, `123`, `world`</span></span>

<span data-ttu-id="49033-173">⁽¹⁾ Atualmente, a tokenização só funciona quando a caixa está mudando de minúsculas para maiúsculas, portanto, `HELLOworld` é considerada um único token: `helloworld`, e `HelloWORld` tem dois tokens: `hello`, `world`.</span><span class="sxs-lookup"><span data-stu-id="49033-173">⁽¹⁾ Currently, tokenization only works when the casing is changing from lowercase to uppercase, so `HELLOworld` is considered a single token: `helloworld`, and `HelloWORld` is two tokens: `hello`, `world`.</span></span> <span data-ttu-id="49033-174">⁽²⁾ A lógica de tokenização também combina palavras que são separadas apenas por símbolos; por exemplo, pesquisar por `helloworld` irá localizar `hello-world` e `hello.world`.</span><span class="sxs-lookup"><span data-stu-id="49033-174">⁽²⁾ Tokenization logic also combines words that are separated only by symbols; for example, searching for `helloworld` will find `hello-world` and `hello.world`.</span></span>

> <span data-ttu-id="49033-175">**Observação**: após a geração de tokens, os tokens são combinados independentemente da capitalização original e são combinados em qualquer ordem.</span><span class="sxs-lookup"><span data-stu-id="49033-175">**Note**: after tokenization, the tokens are matched independently of the original casing, and they are matched in any order.</span></span>

<span data-ttu-id="49033-176">O suporte à pesquisa com token funciona apenas nos campos **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="49033-176">The tokenized search support works only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="49033-177">Qualquer campo de tipo de cadeia de caracteres pode ser colocado em `$search`; campos diferentes de **displayName** e **descrição** tem comportamento `$filter` `startswith` por padrão.</span><span class="sxs-lookup"><span data-stu-id="49033-177">Any field of string type can be put in `$search`; fields other than **displayName** and **description** default to `$filter` `startswith` behavior.</span></span> <span data-ttu-id="49033-178">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="49033-178">For example:</span></span>

`https://graph.microsoft.com/beta/groups/?$search="displayName:OneVideo"`

<span data-ttu-id="49033-179">procurar todos os grupos com nomes de exibição que se pareçam com "OneVideo".</span><span class="sxs-lookup"><span data-stu-id="49033-179">This looks for all groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="49033-180">O parâmetro `$search` também pode ser usado junto com o `$filter`.</span><span class="sxs-lookup"><span data-stu-id="49033-180">`$search` can be used together with `$filter` as well.</span></span> <span data-ttu-id="49033-181">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="49033-181">For example:</span></span>

`https://graph.microsoft.com/beta/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"`

<span data-ttu-id="49033-182">procurar todos os grupos habilitados para email com nomes de exibição que se pareçam com "OneVideo".</span><span class="sxs-lookup"><span data-stu-id="49033-182">This looks for all mail-enabled groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="49033-183">Os resultados são restringidos com base em uma conjunção lógica (um “AND”) do parâmetro `$filter` e na consulta inteira no parâmetro `$search`.</span><span class="sxs-lookup"><span data-stu-id="49033-183">The results are restricted based on a logical conjunction (an "AND") of the `$filter` and the entire query in the `$search`.</span></span> <span data-ttu-id="49033-184">O texto da pesquisa é tokenizado com base nas letras maiúsculas ou minúsculas, mas as equiparações são executadas de maneira insensível ao fato de a letra ser maiúscula ou minúscula.</span><span class="sxs-lookup"><span data-stu-id="49033-184">The search text is tokenized based on casing, but matches are performed in a case-insensitive manner.</span></span> <span data-ttu-id="49033-185">Por exemplo, "OneVideo" seria dividido em dois tokens de entrada "one" e "video", mas correspondendo a propriedades que não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="49033-185">For example, "OneVideo" would be split into two input tokens "one" and "video", but matches properties insensitive to case.</span></span>

<span data-ttu-id="49033-186">A sintaxe da pesquisa segue as seguintes regras:</span><span class="sxs-lookup"><span data-stu-id="49033-186">The syntax of search follows these rules:</span></span>

* <span data-ttu-id="49033-187">Formato genérico: $search="clause1" \[AND \| OR\] "\[clauseX\]"\.</span><span class="sxs-lookup"><span data-stu-id="49033-187">Generic format: $search="clause1" \[AND \| OR\] "\[clauseX\]"\.</span></span>
* <span data-ttu-id="49033-188">O número de cláusulas (clause) não é limitado.</span><span class="sxs-lookup"><span data-stu-id="49033-188">Any number of clauses is supported.</span></span> <span data-ttu-id="49033-189">O uso de parênteses para a precedência também é suportado.</span><span class="sxs-lookup"><span data-stu-id="49033-189">Parentheses for precedence is also supported.</span></span>
* <span data-ttu-id="49033-190">A sintaxe para cada cláusula é: “\<property>:\<text to search>”.</span><span class="sxs-lookup"><span data-stu-id="49033-190">The syntax for each clause is: "\<property>:\<text to search>".</span></span>
* <span data-ttu-id="49033-191">O nome da propriedade deve ser especificado na cláusula.</span><span class="sxs-lookup"><span data-stu-id="49033-191">The property name must be specified in the clause.</span></span> <span data-ttu-id="49033-192">Qualquer propriedade que possa ser usada em `$filter` também pode ser usada dentro de `$search`.</span><span class="sxs-lookup"><span data-stu-id="49033-192">Any property that can be used in `$filter` can also be used inside `$search`.</span></span> <span data-ttu-id="49033-193">Dependendo da propriedade, o comportamento da pesquisa será "search" ou, se “search” não for suportado na propriedade, "startswith".</span><span class="sxs-lookup"><span data-stu-id="49033-193">Depending on the property, the search behavior is either "search" or "startswith" if search is not supported on the property.</span></span>
* <span data-ttu-id="49033-194">Todas as partes de cláusula devem ser colocadas entre aspas duplas.</span><span class="sxs-lookup"><span data-stu-id="49033-194">The whole clause part must be put inside double quotes.</span></span>
* <span data-ttu-id="49033-195">Os operadores lógicos “AND” e “OR” devem ser colocados fora das aspas duplas.</span><span class="sxs-lookup"><span data-stu-id="49033-195">Logical operator 'AND' 'OR' must be put outside double quotes.</span></span> <span data-ttu-id="49033-196">Devem sempre ser grafados em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="49033-196">They must be in upper case.</span></span>
* <span data-ttu-id="49033-p116">Considerando que toda a parte da cláusula precisa ser colocada entre aspas duplas, se ela contiver aspas duplas e barra invertida, ela precisará ter uma barra invertida como escape. Nenhum outro caractere precisa ter escape.</span><span class="sxs-lookup"><span data-stu-id="49033-p116">Given that the whole clause part needs to be put inside double quotes, if it contains double quote and backslash, it needs to be escaped with a backslash. No other characters need to be escaped.</span></span>

<span data-ttu-id="49033-199">A tabela a seguir mostra alguns exemplos.</span><span class="sxs-lookup"><span data-stu-id="49033-199">The following table shows some examples.</span></span>

| <span data-ttu-id="49033-200">Classe de objeto</span><span class="sxs-lookup"><span data-stu-id="49033-200">Object class</span></span> | <span data-ttu-id="49033-201">Descrição</span><span class="sxs-lookup"><span data-stu-id="49033-201">Description</span></span> | <span data-ttu-id="49033-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49033-202">Example</span></span> |
| ------------ | ----------- | ------- |
| <span data-ttu-id="49033-203">Usuário</span><span class="sxs-lookup"><span data-stu-id="49033-203">User</span></span> | <span data-ttu-id="49033-204">O caderno de endereços exibe o nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="49033-204">Address book display name of the user.</span></span> | <span data-ttu-id="49033-205">
  [
  https://graph.microsoft.com/beta/users?$search="displayName:Guthr"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span><span class="sxs-lookup"><span data-stu-id="49033-205">[https://graph.microsoft.com/beta/users?$search="displayName:Guthr"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span></span> |
| <span data-ttu-id="49033-206">Usuário</span><span class="sxs-lookup"><span data-stu-id="49033-206">User</span></span> | <span data-ttu-id="49033-207">O caderno de endereços exibe o nome ou o email do usuário.</span><span class="sxs-lookup"><span data-stu-id="49033-207">Address book display name or mail of the user.</span></span> | <span data-ttu-id="49033-208">
  [
  https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22%20OR%20%22mail%3AGuthr%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span><span class="sxs-lookup"><span data-stu-id="49033-208">[https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22%20OR%20%22mail%3AGuthr%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span></span> |
| <span data-ttu-id="49033-209">Grupo</span><span class="sxs-lookup"><span data-stu-id="49033-209">Group</span></span> | <span data-ttu-id="49033-210">O caderno de endereços exibe o nome ou a descrição de um grupo.</span><span class="sxs-lookup"><span data-stu-id="49033-210">Address book display name or description of the group.</span></span> | <span data-ttu-id="49033-211">
  [
  https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24search%3D%22description%3AOne%22%20AND%20(%22displayName%3AVideo%22%20OR%20%22displayName%3ADrive%22)&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span><span class="sxs-lookup"><span data-stu-id="49033-211">[https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24search%3D%22description%3AOne%22%20AND%20(%22displayName%3AVideo%22%20OR%20%22displayName%3ADrive%22)&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span></span> |
| <span data-ttu-id="49033-212">Grupo</span><span class="sxs-lookup"><span data-stu-id="49033-212">Group</span></span> | <span data-ttu-id="49033-213">Nome de exibição do catálogo de endereços em um grupo habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="49033-213">Address book display name on a mail-enabled group.</span></span> | <span data-ttu-id="49033-214">
  [
  https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DmailEnabled%20eq%20true%26%24search%3D%22displayName%3AOneVideo%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span><span class="sxs-lookup"><span data-stu-id="49033-214">[https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DmailEnabled%20eq%20true%26%24search%3D%22displayName%3AOneVideo%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span></span> |

<span data-ttu-id="49033-215">Ambas as entradas da cadeia de caracteres fornecidas em `$search`, bem como as propriedades pesquisáveis, são divididas em partes por espaços, uso de maiúsculas/minúsculas e tipos de caracteres (números e caracteres especiais).</span><span class="sxs-lookup"><span data-stu-id="49033-215">Both the string inputs you provide in `$search`, as well as the searchable properties, are split up into parts by spaces, different casing, and character types (numbers and special characters).</span></span>

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0

## <a name="see-also"></a><span data-ttu-id="49033-216">Confira também</span><span class="sxs-lookup"><span data-stu-id="49033-216">See also</span></span>

- [<span data-ttu-id="49033-217">Usar parâmetros de consulta para personalizar respostas</span><span class="sxs-lookup"><span data-stu-id="49033-217">Use query parameters to customize responses</span></span>](/graph/query-parameters)
- [<span data-ttu-id="49033-218">Recursos avançados de consulta em objetos de diretório do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="49033-218">Advanced query capabilities on Azure AD directory objects</span></span>](/graph/aad-advanced-queries)
- [<span data-ttu-id="49033-219">Limitações de parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="49033-219">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)