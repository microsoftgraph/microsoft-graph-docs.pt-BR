---
title: 'servicePrincipal: delta'
description: Get recentemente criado, atualizado ou excluído entidades de serviço sem precisar realizar uma leitura completa do conjunto de recurso inteiro. Consulte usando Delta consulta para obter detalhes.
localization_priority: Normal
ms.openlocfilehash: ed0cf279d1d076e324d24e1774734e9aa14a6b34
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520071"
---
# <a name="serviceprincipal-delta"></a><span data-ttu-id="27fcc-104">servicePrincipal: delta</span><span class="sxs-lookup"><span data-stu-id="27fcc-104">servicePrincipal: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27fcc-105">Get recentemente criado, atualizado ou excluído entidades de serviço sem precisar realizar uma leitura completa do conjunto de recurso inteiro.</span><span class="sxs-lookup"><span data-stu-id="27fcc-105">Get newly created, updated, or deleted service principals without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="27fcc-106">Consulte [Usando Delta consulta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="27fcc-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="27fcc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="27fcc-107">Permissions</span></span>

<span data-ttu-id="27fcc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27fcc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="27fcc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27fcc-110">Permission type</span></span>      | <span data-ttu-id="27fcc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27fcc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27fcc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27fcc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27fcc-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="27fcc-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="27fcc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27fcc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27fcc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27fcc-115">Not supported.</span></span>    |
|<span data-ttu-id="27fcc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27fcc-116">Application</span></span> | <span data-ttu-id="27fcc-117">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="27fcc-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27fcc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27fcc-118">HTTP request</span></span>

<span data-ttu-id="27fcc-119">Para começar a controlar alterações, você deve fazer uma solicitação, incluindo a função delta no recurso servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="27fcc-119">To begin tracking changes, you make a request including the delta function on the servicePrincipal resource.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/delta
```

### <a name="query-parameters"></a><span data-ttu-id="27fcc-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="27fcc-120">Query parameters</span></span>

<span data-ttu-id="27fcc-121">Controle de alterações provoca uma round de um ou mais chamadas de função **delta** .</span><span class="sxs-lookup"><span data-stu-id="27fcc-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="27fcc-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), você deve especificá-lo na solicitação inicial **delta** .</span><span class="sxs-lookup"><span data-stu-id="27fcc-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="27fcc-123">O Microsoft Graph codifica automaticamente quaisquer parâmetros especificados a parte de token do `nextLink` ou `deltaLink` URL fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="27fcc-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="27fcc-124">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="27fcc-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="27fcc-125">Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="27fcc-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="27fcc-126">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="27fcc-126">Query parameter</span></span>      | <span data-ttu-id="27fcc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="27fcc-127">Type</span></span>   |<span data-ttu-id="27fcc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="27fcc-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="27fcc-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="27fcc-129">$deltatoken</span></span> | <span data-ttu-id="27fcc-130">string</span><span class="sxs-lookup"><span data-stu-id="27fcc-130">string</span></span> | <span data-ttu-id="27fcc-131">Um [token de estado](/graph/delta-query-overview) retornados no `deltaLink` URL da chamada de função **delta** anterior para o mesmo conjunto de recursos, indicando a conclusão do que round de controle de alterações.</span><span class="sxs-lookup"><span data-stu-id="27fcc-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="27fcc-132">Salvar e aplicar a toda a `deltaLink` URL incluindo este token na primeira solicitação da próxima fase de rastreamento para esse conjunto de alterações.</span><span class="sxs-lookup"><span data-stu-id="27fcc-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="27fcc-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="27fcc-133">$skiptoken</span></span> | <span data-ttu-id="27fcc-134">string</span><span class="sxs-lookup"><span data-stu-id="27fcc-134">string</span></span> | <span data-ttu-id="27fcc-135">Um [token de estado](/graph/delta-query-overview) retornados no `nextLink` URL da chamada de função **delta** anterior, indicando que não há mais alterações a serem rastreados no mesmo conjunto de recursos.</span><span class="sxs-lookup"><span data-stu-id="27fcc-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="27fcc-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27fcc-136">Optional query parameters</span></span>

<span data-ttu-id="27fcc-137">Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27fcc-137">This method supports OData Query Parameters to help customize the response.</span></span>

- <span data-ttu-id="27fcc-p106">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="27fcc-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span> 

- <span data-ttu-id="27fcc-140">Não há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="27fcc-140">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="27fcc-141">A única suportada `$filter` expression é para controle de alterações de recursos específicos, por sua id: `$filter=id+eq+{value}` ou `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="27fcc-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="27fcc-142">O número de identificações, que você pode especificar é limitado pelo comprimento máximo da URL.</span><span class="sxs-lookup"><span data-stu-id="27fcc-142">The number of ids you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="27fcc-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27fcc-143">Request headers</span></span>
| <span data-ttu-id="27fcc-144">Nome</span><span class="sxs-lookup"><span data-stu-id="27fcc-144">Name</span></span>       | <span data-ttu-id="27fcc-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="27fcc-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="27fcc-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="27fcc-146">Authorization</span></span>  | <span data-ttu-id="27fcc-147">&lt;Token&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="27fcc-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="27fcc-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27fcc-148">Content-Type</span></span>  | <span data-ttu-id="27fcc-149">application/json</span><span class="sxs-lookup"><span data-stu-id="27fcc-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="27fcc-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27fcc-150">Request body</span></span>
<span data-ttu-id="27fcc-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27fcc-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="27fcc-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="27fcc-152">Response</span></span>

<span data-ttu-id="27fcc-153">Se tiver êxito, este método retornará `200 OK` objeto de coleção [servicePrincipal](../resources/serviceprincipal.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27fcc-153">If successful, this method returns `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) collection object in the response body.</span></span> <span data-ttu-id="27fcc-154">A resposta também inclui uma URL de nextLink ou uma URL de deltaLink.</span><span class="sxs-lookup"><span data-stu-id="27fcc-154">The response also includes a nextLink URL or a deltaLink URL.</span></span> 

- <span data-ttu-id="27fcc-155">Se um `nextLink` URL é retornado, existem páginas adicionais de dados a ser recuperado na sessão.</span><span class="sxs-lookup"><span data-stu-id="27fcc-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="27fcc-156">O aplicativo continua fazendo solicitações usando o `nextLink` URL até um `deltaLink` URL está incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="27fcc-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="27fcc-157">Se um `deltaLink` URL é retornado, não há nenhum dado mais sobre o estado existente do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="27fcc-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="27fcc-158">Persistir e usar o `deltaLink` URL para saber mais sobre as alterações do recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="27fcc-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="27fcc-159">Confira:</span><span class="sxs-lookup"><span data-stu-id="27fcc-159">See:</span></span></br>
- <span data-ttu-id="27fcc-160">[Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="27fcc-160">[Using Delta Query](/graph/delta-query-overview) for more details</span></span></br>
- <span data-ttu-id="27fcc-161">[Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</span><span class="sxs-lookup"><span data-stu-id="27fcc-161">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span></br>

### <a name="example"></a><span data-ttu-id="27fcc-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27fcc-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27fcc-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27fcc-163">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_delta"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```

##### <a name="response"></a><span data-ttu-id="27fcc-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="27fcc-164">Response</span></span>
<span data-ttu-id="27fcc-p111">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27fcc-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#servicePrincipals",
  "@odata.nextLink":"https://graph.microsoft.com/beta/servicePrincipals/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
     {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
