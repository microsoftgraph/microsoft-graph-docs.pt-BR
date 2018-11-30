---
title: 'contactFolder: delta'
description: Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.
ms.openlocfilehash: 3ba1d09fb280389f3b6dd1ea3af4aa8601d4ca37
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035988"
---
# <a name="contactfolder-delta"></a><span data-ttu-id="736fe-103">contactFolder: delta</span><span class="sxs-lookup"><span data-stu-id="736fe-103">contactFolder: delta</span></span>

> <span data-ttu-id="736fe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="736fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="736fe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="736fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="736fe-106">Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="736fe-106">Get a set of contact folders that have been added, deleted, or removed from the user's mailbox.</span></span>

<span data-ttu-id="736fe-p102">Uma chamada de função **delta** de pastas de contato em uma caixa de correio é semelhante a uma solicitação GET, exceto que, aplicando adequadamente os [tokens de estado](/graph/delta-query-overview) em uma ou mais dessas chamadas, permite consultar alterações incrementais nas pastas de contato. Isso permite manter e sincronizar um armazenamento local de pastas de contato do usuário sem ter que sempre buscar todas as pastas de contato dessa caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="736fe-p102">A **delta** function call for contact folders in a mailbox is similar to a GET request, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in the contact folders. This allows you to maintain and synchronize a local store of a user's contact folders without having to fetch all the contact folders of that mailbox from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="736fe-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="736fe-109">Permissions</span></span>
<span data-ttu-id="736fe-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="736fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="736fe-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="736fe-112">Permission type</span></span>      | <span data-ttu-id="736fe-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="736fe-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="736fe-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="736fe-114">Delegated (work or school account)</span></span> | <span data-ttu-id="736fe-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="736fe-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="736fe-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="736fe-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="736fe-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="736fe-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="736fe-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="736fe-118">Application</span></span> | <span data-ttu-id="736fe-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="736fe-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="736fe-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="736fe-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/delta
GET /users/<id>/contactFolders/delta
```

## <a name="query-parameters"></a><span data-ttu-id="736fe-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="736fe-121">Query parameters</span></span>

<span data-ttu-id="736fe-p104">O controle de alterações em pastas de contato corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token (`skiptoken` ou `$deltatoken`) da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, basta copiar e aplicar a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="736fe-p104">Tracking changes in contact folders incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion (`skiptoken` or `$deltatoken`) of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="736fe-127">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="736fe-127">Query parameter</span></span>      | <span data-ttu-id="736fe-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="736fe-128">Type</span></span>   |<span data-ttu-id="736fe-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="736fe-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="736fe-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="736fe-130">$deltatoken</span></span> | <span data-ttu-id="736fe-131">string</span><span class="sxs-lookup"><span data-stu-id="736fe-131">string</span></span> | <span data-ttu-id="736fe-p105">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de pastas de contato indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.</span><span class="sxs-lookup"><span data-stu-id="736fe-p105">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same contact folder collection, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="736fe-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="736fe-134">$skiptoken</span></span> | <span data-ttu-id="736fe-135">string</span><span class="sxs-lookup"><span data-stu-id="736fe-135">string</span></span> | <span data-ttu-id="736fe-136">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de pastas de contato.</span><span class="sxs-lookup"><span data-stu-id="736fe-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same contact folder collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="736fe-137">Parâmetros de consulta OData</span><span class="sxs-lookup"><span data-stu-id="736fe-137">OData query parameters</span></span>

<span data-ttu-id="736fe-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="736fe-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="736fe-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="736fe-140">Request headers</span></span>
| <span data-ttu-id="736fe-141">Nome</span><span class="sxs-lookup"><span data-stu-id="736fe-141">Name</span></span>       | <span data-ttu-id="736fe-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="736fe-142">Type</span></span> | <span data-ttu-id="736fe-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="736fe-143">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="736fe-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="736fe-144">Authorization</span></span>  | <span data-ttu-id="736fe-145">string</span><span class="sxs-lookup"><span data-stu-id="736fe-145">string</span></span>  | <span data-ttu-id="736fe-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="736fe-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="736fe-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="736fe-148">Content-Type</span></span>  | <span data-ttu-id="736fe-149">string</span><span class="sxs-lookup"><span data-stu-id="736fe-149">string</span></span>  | <span data-ttu-id="736fe-p108">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="736fe-p108">application/json. Required.</span></span> |
| <span data-ttu-id="736fe-152">Preferir</span><span class="sxs-lookup"><span data-stu-id="736fe-152">Prefer</span></span> | <span data-ttu-id="736fe-153">string</span><span class="sxs-lookup"><span data-stu-id="736fe-153">string</span></span>  | <span data-ttu-id="736fe-p109">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="736fe-p109">odata.maxpagesize={x}. Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="736fe-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="736fe-156">Response</span></span>

<span data-ttu-id="736fe-157">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="736fe-157">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="736fe-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="736fe-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="736fe-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="736fe-159">Request</span></span>
<span data-ttu-id="736fe-160">O exemplo a seguir mostra como fazer uma única chamada de função **delta** e limitar o número máximo de pastas de contato no corpo da resposta a 2.</span><span class="sxs-lookup"><span data-stu-id="736fe-160">The following example shows how to make a single **delta** function call, and limit the maximum number of contact folders in the response body to 2.</span></span>

<span data-ttu-id="736fe-161">Para controlar as alterações nas pastas de contato de uma caixa de correio, faça uma ou mais chamadas de função **delta**, com os tokens de estado apropriados, para obter o conjunto de alterações incrementais desde a última consulta delta.</span><span class="sxs-lookup"><span data-stu-id="736fe-161">To track changes in the contact folders of a mailbox, you would make one or more **delta** function calls, with appropriate state tokens, to get the set of incremental changes since the last delta query.</span></span> 

<span data-ttu-id="736fe-p110">Você pode encontrar um exemplo semelhante que mostra como usar os tokens de estado para controlar alterações em mensagens de uma pasta de email: [Obtenha alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages). As principais diferenças entre o controle de pastas de contato e o controle de mensagens em uma pasta encontram-se nas URLs das solicitações da consulta delta e nas respostas da consulta que retornam **contactFolder** em vez de coleções de **mensagens**.</span><span class="sxs-lookup"><span data-stu-id="736fe-p110">You can find a similar example that shows how to use the state tokens to track changes in the messages of a mail folder: [Get incremental changes to messages in a folder](/graph/delta-query-messages). The main differences between tracking contact folders and tracking messages in a folder are in the delta query request URLs, and the query responses returning **contactFolder** rather than **message** collections.</span></span>

<!-- {
  "blockType": "request",
  "name": "contactfolder_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/delta

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="736fe-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="736fe-164">Response</span></span>

<span data-ttu-id="736fe-165">Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_</span><span class="sxs-lookup"><span data-stu-id="736fe-165">If the request is successful, the response would include a state token, which is either a _skipToken_</span></span>  
<span data-ttu-id="736fe-p111">(em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.</span><span class="sxs-lookup"><span data-stu-id="736fe-p111">(in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="736fe-168">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="736fe-168">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="736fe-p112">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="736fe-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="see-also"></a><span data-ttu-id="736fe-171">Confira também</span><span class="sxs-lookup"><span data-stu-id="736fe-171">See also</span></span>

- [<span data-ttu-id="736fe-172">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="736fe-172">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="736fe-173">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="736fe-173">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
