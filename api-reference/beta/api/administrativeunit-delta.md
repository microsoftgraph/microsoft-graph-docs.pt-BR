---
title: 'administrativeUnit: delta'
description: Obter unidades administrativas recém-criadas, atualizadas ou excluídas sem precisar executar uma leitura completa de toda a coleção de recursos.
localization_priority: Normal
author: anandyadavMSFT
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b3056615a09a027911fd98c0636c6e313a2cad2c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438887"
---
# <a name="administrativeunit-delta"></a><span data-ttu-id="20748-103">administrativeUnit: delta</span><span class="sxs-lookup"><span data-stu-id="20748-103">administrativeUnit: delta</span></span>

<span data-ttu-id="20748-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20748-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20748-105">Get newly created, updated, or **deleted administrativeUnits** without having to perform a full read of the entire resource collection.</span><span class="sxs-lookup"><span data-stu-id="20748-105">Get newly created, updated, or deleted **administrativeUnits** without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="20748-106">Para obter detalhes, consulte [Using delta query](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="20748-106">For details, see [Using delta query](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="20748-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="20748-107">Permissions</span></span>

<span data-ttu-id="20748-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20748-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="20748-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20748-110">Permission type</span></span>      | <span data-ttu-id="20748-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20748-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20748-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20748-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20748-113">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20748-113">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20748-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20748-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20748-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20748-115">Not supported.</span></span>    |
|<span data-ttu-id="20748-116">administrativeunit</span><span class="sxs-lookup"><span data-stu-id="20748-116">administrativeunit</span></span> | <span data-ttu-id="20748-117">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20748-117">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20748-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20748-118">HTTP request</span></span>

<span data-ttu-id="20748-119">Para começar a controlar as alterações, você faz uma solicitação que inclui a função delta no **recurso administrativeUnit.**</span><span class="sxs-lookup"><span data-stu-id="20748-119">To begin tracking changes, you make a request that includes the delta function on the **administrativeUnit** resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/delta
```

## <a name="query-parameters"></a><span data-ttu-id="20748-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="20748-120">Query parameters</span></span>

<span data-ttu-id="20748-121">O controle de alterações incorre em uma rodada de uma ou mais chamadas **de função delta.**</span><span class="sxs-lookup"><span data-stu-id="20748-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="20748-122">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="20748-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="20748-123">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="20748-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="20748-124">Você só precisa especificar os parâmetros de consulta uma vez na frente.</span><span class="sxs-lookup"><span data-stu-id="20748-124">You only need to specify any query parameters once up front.</span></span> <span data-ttu-id="20748-125">Em solicitações subsequentes, copie e aplique `nextLink` a URL ou da resposta `deltaLink` anterior.</span><span class="sxs-lookup"><span data-stu-id="20748-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response.</span></span> <span data-ttu-id="20748-126">Essa URL já inclui os parâmetros codificados.</span><span class="sxs-lookup"><span data-stu-id="20748-126">That URL already includes the encoded parameters.</span></span>

| <span data-ttu-id="20748-127">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="20748-127">Query parameter</span></span>      | <span data-ttu-id="20748-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="20748-128">Type</span></span>   |<span data-ttu-id="20748-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="20748-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="20748-130">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="20748-130">$deltatoken</span></span> | <span data-ttu-id="20748-131">string</span><span class="sxs-lookup"><span data-stu-id="20748-131">string</span></span> | <span data-ttu-id="20748-132">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de `deltaLink` alterações. </span><span class="sxs-lookup"><span data-stu-id="20748-132">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="20748-133">Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.</span><span class="sxs-lookup"><span data-stu-id="20748-133">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="20748-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="20748-134">$skiptoken</span></span> | <span data-ttu-id="20748-135">string</span><span class="sxs-lookup"><span data-stu-id="20748-135">string</span></span> | <span data-ttu-id="20748-136">Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na mesma coleção de `nextLink` recursos. </span><span class="sxs-lookup"><span data-stu-id="20748-136">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="optional-query-parameters"></a><span data-ttu-id="20748-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20748-137">Optional query parameters</span></span>

<span data-ttu-id="20748-138">Este método suporta os seguintes parâmetros de consulta OData para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="20748-138">This method supports the following OData query parameters to help customize the response:</span></span>

- <span data-ttu-id="20748-p105">Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade **id** sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="20748-p105">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The **id** property is always returned.</span></span> 

- <span data-ttu-id="20748-141">Há suporte limitado para `$filter`:</span><span class="sxs-lookup"><span data-stu-id="20748-141">There is limited support for `$filter`:</span></span>
  * <span data-ttu-id="20748-142">A única expressão `$filter` com suporte é para controlar alterações para recursos específicos, por sua ID: ou  `$filter=id+eq+{value}` `$filter=id+eq+{value1}+or+id+eq+{value2}` .</span><span class="sxs-lookup"><span data-stu-id="20748-142">The only supported `$filter` expression is for tracking changes for specific resources, by their ID:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="20748-143">O número de IDs que você pode especificar é limitado pelo tamanho máximo da URL.</span><span class="sxs-lookup"><span data-stu-id="20748-143">The number of IDs you can specify is limited by the maximum URL length.</span></span>


## <a name="request-headers"></a><span data-ttu-id="20748-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20748-144">Request headers</span></span>
| <span data-ttu-id="20748-145">Nome</span><span class="sxs-lookup"><span data-stu-id="20748-145">Name</span></span>       | <span data-ttu-id="20748-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="20748-146">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20748-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="20748-147">Authorization</span></span>  | <span data-ttu-id="20748-148">&lt;token&gt; de portador.</span><span class="sxs-lookup"><span data-stu-id="20748-148">Bearer &lt;token&gt;.</span></span> <span data-ttu-id="20748-149">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20748-149">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20748-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20748-150">Request body</span></span>
<span data-ttu-id="20748-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20748-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20748-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="20748-152">Response</span></span>

<span data-ttu-id="20748-153">Se tiver êxito, este método retornará o código de resposta e um objeto de coleção `200 OK` [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20748-153">If successful, this method returns `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) collection object in the response body.</span></span> <span data-ttu-id="20748-154">A resposta também inclui uma URL `nextLink` ou uma URL `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="20748-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span> 

- <span data-ttu-id="20748-155">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="20748-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="20748-156">A **administrativeUnit continua** fazendo solicitações usando `nextLink` a URL até que uma URL seja incluída na `deltaLink` resposta.</span><span class="sxs-lookup"><span data-stu-id="20748-156">The **administrativeUnit** continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="20748-157">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="20748-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="20748-158">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="20748-158">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="20748-159">Para obter detalhes e um exemplo, consulte [Using delta query](/graph/delta-query-overview) and [Get incremental changes for users](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="20748-159">For details and an example, see [Using delta query](/graph/delta-query-overview) and [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="example"></a><span data-ttu-id="20748-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20748-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="20748-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20748-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="20748-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="20748-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "administrativeunit_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/delta
```
# <a name="c"></a>[<span data-ttu-id="20748-163">C#</span><span class="sxs-lookup"><span data-stu-id="20748-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/administrativeunit-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20748-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20748-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/administrativeunit-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20748-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20748-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/administrativeunit-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20748-166">Java</span><span class="sxs-lookup"><span data-stu-id="20748-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/administrativeunit-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20748-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="20748-167">Response</span></span>
><span data-ttu-id="20748-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20748-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#administrativeunits",
  "@odata.nextLink":"https://graph.microsoft.com/beta/administrativeunits/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "Management Fast Track",
      "visibility": null,
      "extension_fe2174665583431c953114ff7268b7b3_Education_ObjectType": "School",
      "extension_fe2174665583431c953114ff7268b7b3_Education_StateId": "WA",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Address": "2 Microsoft Way",
      "extension_fe2174665583431c953114ff7268b7b3_Education_City": "Redmond",
      "extension_fe2174665583431c953114ff7268b7b3_Education_State": "WA",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Country": "US",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Zip": "98052",
      "extension_fe2174665583431c953114ff7268b7b3_Education_Phone": "555-123-4567",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SyncSource": "SIS",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SyncSource_SchoolId": "10002",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalSyncSourceId": "14008",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalName": "Amy Roebuck",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolPrincipalEmail": "aroebuck@principal.edu",
      "extension_fe2174665583431c953114ff7268b7b3_Education_SchoolZone": "1",
      "id": "8a07f5a8-edc9-4847-bbf2-dde106594bf4",
      "members@delta": [
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "b66ecf79-a093-4d51-86e0-efcc4531f37a"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "5bde3e51-d13b-4db1-9948-fe4b109d11a7"
        },
        {
            "@odata.type": "#microsoft.graph.group",
            "id": "801f2093-de7e-4883-a786-8a5f30874ff4"
        },
        {
            "@odata.type": "#microsoft.graph.group",
            "id": "7e4ec76c-8276-43ef-ba10-9aaa197cb212"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "f5289423-7233-4d60-831a-fe107a8551cc"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "48d31887-5fad-4d73-a9f5-3c356e68a038"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "87d349ed-44d7-43e1-9a83-5f2406dee5bd"
        },
        {
            "@odata.type": "#microsoft.graph.user",
            "id": "c03e6eaa-b6ab-46d7-905b-73ec7ea1f755"
        }
      ]
  }
  ]
}
```

<!-- uuid: 69848a18-6b48-44fd-a398-4521803a0a00
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeunit: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


