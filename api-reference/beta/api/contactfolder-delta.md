---
title: 'contactFolder: delta'
description: Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2d3f133f6f9c1e6e349902593e0f37191e3aecbc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520820"
---
# <a name="contactfolder-delta"></a><span data-ttu-id="a0ce7-103">contactFolder: delta</span><span class="sxs-lookup"><span data-stu-id="a0ce7-103">contactFolder: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0ce7-104">Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-104">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="a0ce7-p101">Uma chamada de função **delta** de pastas de contato em uma caixa de correio é semelhante a uma solicitação GET, exceto que, aplicando adequadamente os [tokens de estado](/graph/delta-query-overview) em uma ou mais dessas chamadas, permite consultar alterações incrementais nas pastas de contato. Isso permite manter e sincronizar um armazenamento local de pastas de contato do usuário sem ter que sempre buscar todas as pastas de contato dessa caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p101">A **delta** function call for contact folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the contact folders. This allows you to maintain and synchronize a local store of a user's contact folders without having to fetch all the contact folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0ce7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0ce7-107">Permissions</span></span>
<span data-ttu-id="a0ce7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a0ce7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0ce7-110">Permission type</span></span>      | <span data-ttu-id="a0ce7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0ce7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0ce7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0ce7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0ce7-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0ce7-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a0ce7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0ce7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0ce7-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0ce7-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a0ce7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0ce7-116">Application</span></span> | <span data-ttu-id="a0ce7-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0ce7-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0ce7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0ce7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/delta
GET /users/<id>/contactFolders/delta
```

## <a name="query-parameters"></a><span data-ttu-id="a0ce7-119">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="a0ce7-119">Query parameters</span></span>

<span data-ttu-id="a0ce7-p103">O controle de alterações em pastas de contato corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token (`skiptoken` ou `$deltatoken`) da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, basta copiar e aplicar a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p103">Tracking changes in contact folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion (`skiptoken` or `$deltatoken`) of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="a0ce7-125">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="a0ce7-125">Query parameter</span></span>      | <span data-ttu-id="a0ce7-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0ce7-126">Type</span></span>   |<span data-ttu-id="a0ce7-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0ce7-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a0ce7-128">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a0ce7-128">$deltatoken</span></span> | <span data-ttu-id="a0ce7-129">string</span><span class="sxs-lookup"><span data-stu-id="a0ce7-129">string</span></span> | <span data-ttu-id="a0ce7-p104">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de pastas de contato indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p104">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same contact folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a0ce7-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a0ce7-132">$skiptoken</span></span> | <span data-ttu-id="a0ce7-133">string</span><span class="sxs-lookup"><span data-stu-id="a0ce7-133">string</span></span> | <span data-ttu-id="a0ce7-134">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de pastas de contato.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-134">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact folder collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="a0ce7-135">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="a0ce7-135">OData query parameters</span></span>

<span data-ttu-id="a0ce7-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="a0ce7-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ce7-138">Request headers</span></span>
| <span data-ttu-id="a0ce7-139">Nome</span><span class="sxs-lookup"><span data-stu-id="a0ce7-139">Name</span></span>       | <span data-ttu-id="a0ce7-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0ce7-140">Type</span></span> | <span data-ttu-id="a0ce7-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0ce7-141">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="a0ce7-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0ce7-142">Authorization</span></span>  | <span data-ttu-id="a0ce7-143">string</span><span class="sxs-lookup"><span data-stu-id="a0ce7-143">string</span></span>  | <span data-ttu-id="a0ce7-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0ce7-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0ce7-146">Content-Type</span></span>  | <span data-ttu-id="a0ce7-147">string</span><span class="sxs-lookup"><span data-stu-id="a0ce7-147">string</span></span>  | <span data-ttu-id="a0ce7-p107">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p107">application/json. Required.</span></span> |
| <span data-ttu-id="a0ce7-150">Preferir</span><span class="sxs-lookup"><span data-stu-id="a0ce7-150">Prefer</span></span> | <span data-ttu-id="a0ce7-151">string</span><span class="sxs-lookup"><span data-stu-id="a0ce7-151">string</span></span>  | <span data-ttu-id="a0ce7-p108">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p108">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a0ce7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0ce7-154">Response</span></span>

<span data-ttu-id="a0ce7-155">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-155">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0ce7-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0ce7-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0ce7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0ce7-157">Request</span></span>
<span data-ttu-id="a0ce7-158">O exemplo a seguir mostra como fazer uma única chamada de função **delta** e limitar o número máximo de pastas de contato no corpo da resposta a 2.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-158">The following example shows how to make a single **delta** function call, and limit the maximum number of contact folders in the response body to 2.</span></span>

<span data-ttu-id="a0ce7-159">Para controlar as alterações nas pastas de contato de uma caixa de correio, faça uma ou mais chamadas de função **delta**, com os tokens de estado apropriados, para obter o conjunto de alterações incrementais desde a última consulta delta.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-159">To track changes in the contact folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="a0ce7-p109">Você pode encontrar um exemplo semelhante que mostra como usar os tokens de estado para controlar alterações em mensagens de uma pasta de email: [Obtenha alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages). As principais diferenças entre o controle de pastas de contato e o controle de mensagens em uma pasta encontram-se nas URLs das solicitações da consulta delta e nas respostas da consulta que retornam **contactFolder** em vez de coleções de **mensagens**.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p109">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking contact folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contactFolder** rather than **message** collections.</span></span>

<!-- {
  "blockType": "request",
  "name": "contactfolder_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="a0ce7-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0ce7-162">Response</span></span>

<span data-ttu-id="a0ce7-163">Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_</span><span class="sxs-lookup"><span data-stu-id="a0ce7-163">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="a0ce7-p110">(em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p110">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="a0ce7-166">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-166">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="a0ce7-p111">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/contactfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
     "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="a0ce7-169">Confira também</span><span class="sxs-lookup"><span data-stu-id="a0ce7-169">See also</span></span>

- [<span data-ttu-id="a0ce7-170">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a0ce7-170">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="a0ce7-171">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="a0ce7-171">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
