---
title: 'Application: Delta'
description: Obter aplicativos recém-criados, atualizados ou excluídos sem ter que executar uma leitura completa de toda a coleção de recursos. Consulte usando a consulta Delta para obter detalhes.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 13b6f7809cf47edcc9de8c9ddfb052645b15f25a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459244"
---
# <a name="application-delta"></a><span data-ttu-id="d63b8-104">Application: Delta</span><span class="sxs-lookup"><span data-stu-id="d63b8-104">application: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d63b8-105">Obter aplicativos recém-criados, atualizados ou excluídos sem ter que executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="d63b8-105">Get newly created, updated, or deleted applications without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="d63b8-106">Consulte [usando a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="d63b8-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="d63b8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d63b8-107">Permissions</span></span>

<span data-ttu-id="d63b8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d63b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d63b8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d63b8-110">Permission type</span></span>      | <span data-ttu-id="d63b8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d63b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d63b8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d63b8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d63b8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d63b8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d63b8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d63b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d63b8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d63b8-115">Not supported.</span></span>    |
|<span data-ttu-id="d63b8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d63b8-116">Application</span></span> | <span data-ttu-id="d63b8-117">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d63b8-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d63b8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d63b8-118">HTTP request</span></span>

<span data-ttu-id="d63b8-119">Para começar a controlar as alterações, faça uma solicitação incluindo a função Delta no recurso de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d63b8-119">To begin tracking changes, you make a request including the delta function on the application resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a><span data-ttu-id="d63b8-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="d63b8-120">Query parameters</span></span>

<span data-ttu-id="d63b8-121">As alterações de controle provocam uma rodada de uma ou mais chamadas de função **Delta** .</span><span class="sxs-lookup"><span data-stu-id="d63b8-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="d63b8-122">Se você usar qualquer parâmetro de consulta (diferente `$deltatoken` de `$skiptoken`e), você deve especificá-lo na solicitação de **Delta** inicial.</span><span class="sxs-lookup"><span data-stu-id="d63b8-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="d63b8-123">O Microsoft Graph codifica automaticamente qualquer parâmetro especificado na parte do token do URL `nextLink` ou `deltaLink` na resposta fornecida.</span><span class="sxs-lookup"><span data-stu-id="d63b8-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="d63b8-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="d63b8-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="d63b8-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="d63b8-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="d63b8-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="d63b8-126">Query parameter</span></span>      | <span data-ttu-id="d63b8-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d63b8-127">Type</span></span>   |<span data-ttu-id="d63b8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d63b8-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d63b8-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="d63b8-129">$deltatoken</span></span> | <span data-ttu-id="d63b8-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d63b8-130">string</span></span> | <span data-ttu-id="d63b8-131">Um [token de estado](/graph/delta-query-overview) retornado na `deltaLink` URL da chamada de função **Delta** anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="d63b8-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="d63b8-132">Salve e aplique a URL `deltaLink` inteira incluindo esse token na primeira solicitação da próxima rodada de controle de alterações para essa coleção.</span><span class="sxs-lookup"><span data-stu-id="d63b8-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="d63b8-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="d63b8-133">$skiptoken</span></span> | <span data-ttu-id="d63b8-134">string</span><span class="sxs-lookup"><span data-stu-id="d63b8-134">string</span></span> | <span data-ttu-id="d63b8-135">Um [token de estado](/graph/delta-query-overview) retornado na `nextLink` URL da chamada de função **Delta** anterior, indicando que há mais alterações a serem controladas na mesma coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="d63b8-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="d63b8-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d63b8-136">Optional query parameters</span></span>

<span data-ttu-id="d63b8-137">Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d63b8-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="d63b8-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="d63b8-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="d63b8-140">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="d63b8-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="d63b8-141">A única expressão `$filter` suportada é para controlar alterações de recursos específicos, por sua `$filter=id+eq+{value}` ID `$filter=id+eq+{value1}+or+id+eq+{value2}`: ou.</span><span class="sxs-lookup"><span data-stu-id="d63b8-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="d63b8-142">O número de IDs que você pode especificar é limitado pelo tamanho máximo de URL.</span><span class="sxs-lookup"><span data-stu-id="d63b8-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d63b8-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d63b8-143">Request headers</span></span>
| <span data-ttu-id="d63b8-144">Nome</span><span class="sxs-lookup"><span data-stu-id="d63b8-144">Name</span></span>       | <span data-ttu-id="d63b8-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="d63b8-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d63b8-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="d63b8-146">Authorization</span></span>  | <span data-ttu-id="d63b8-147">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="d63b8-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="d63b8-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d63b8-148">Content-Type</span></span>  | <span data-ttu-id="d63b8-149">application/json</span><span class="sxs-lookup"><span data-stu-id="d63b8-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d63b8-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d63b8-150">Request body</span></span>
<span data-ttu-id="d63b8-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d63b8-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="d63b8-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d63b8-152">Response</span></span>

<span data-ttu-id="d63b8-153">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [Application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d63b8-153">If successful, this method returns `200 OK` response code and [application](../resources/application.md) collection object in the response body.</span></span> <span data-ttu-id="d63b8-154">A resposta também inclui uma URL do nextLink ou uma URL do deltaLink.</span><span class="sxs-lookup"><span data-stu-id="d63b8-154">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="d63b8-155">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="d63b8-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="d63b8-156">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="d63b8-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="d63b8-157">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="d63b8-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="d63b8-158">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="d63b8-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="d63b8-159">Confira:</span><span class="sxs-lookup"><span data-stu-id="d63b8-159">See:</span></span></br>
- <span data-ttu-id="d63b8-160">[Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="d63b8-160">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="d63b8-161">[Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="d63b8-161">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="d63b8-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d63b8-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d63b8-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d63b8-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```http
GET https://graph.microsoft.com/beta/applications/delta
```

##### <a name="response"></a><span data-ttu-id="d63b8-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="d63b8-164">Response</span></span>
<span data-ttu-id="d63b8-p111">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d63b8-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
