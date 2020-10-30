---
title: Listar grupos
description: Liste todos os grupos disponíveis em uma organização, incluindo, entre outros, os grupos do Microsoft 365.
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2ea8ed7de6dab441f6311a96a74e014ccd7e625f
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796903"
---
# <a name="list-groups"></a><span data-ttu-id="fcc80-103">Listar grupos</span><span class="sxs-lookup"><span data-stu-id="fcc80-103">List groups</span></span>

<span data-ttu-id="fcc80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcc80-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fcc80-105">Liste todos os grupos em uma organização, incluindo, entre outros, os grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fcc80-105">List all the groups in an organization, including but not limited to Microsoft 365 groups.</span></span> 

<span data-ttu-id="fcc80-106">Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="fcc80-106">This operation returns by default only a subset of the properties for each group.</span></span> <span data-ttu-id="fcc80-107">Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).</span><span class="sxs-lookup"><span data-stu-id="fcc80-107">These default properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="fcc80-108">Para obter propriedades _não_ retornadas por padrão, execute uma operação [GET](group-get.md) para o grupo e especifique as propriedades em uma opção de consulta `$select` do OData.</span><span class="sxs-lookup"><span data-stu-id="fcc80-108">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="fcc80-109">A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`.</span><span class="sxs-lookup"><span data-stu-id="fcc80-109">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcc80-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="fcc80-110">Permissions</span></span>
<span data-ttu-id="fcc80-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcc80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcc80-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcc80-113">Permission type</span></span>      | <span data-ttu-id="fcc80-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcc80-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcc80-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcc80-115">Delegated (work or school account)</span></span> | <span data-ttu-id="fcc80-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fcc80-116">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="fcc80-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcc80-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcc80-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcc80-118">Not supported.</span></span>    |
|<span data-ttu-id="fcc80-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcc80-119">Application</span></span> | <span data-ttu-id="fcc80-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcc80-120">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcc80-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcc80-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcc80-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fcc80-122">Optional query parameters</span></span>
<span data-ttu-id="fcc80-123">Para listar apenas grupos do Microsoft 365 (também conhecidos como grupos unificados), aplique um filtro em **groupTypes** :</span><span class="sxs-lookup"><span data-stu-id="fcc80-123">To list only Microsoft 365 groups (aka unified groups), apply a filter on **groupTypes** :</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="fcc80-124">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName** , conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="fcc80-124">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="fcc80-125">Você também pode usar os `$count` e `$search` parâmetros de consulta para limitar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fcc80-125">You can also use the `$count` and `$search` query parameters to limit the response.</span></span> <span data-ttu-id="fcc80-126">O `$search` parâmetro de consulta suporta a tokenização apenas nos campos **displayName** e **descrição** .</span><span class="sxs-lookup"><span data-stu-id="fcc80-126">The `$search` query parameter supports tokenization only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="fcc80-127">Outros campos são padrão para o `$filter` comportamento.</span><span class="sxs-lookup"><span data-stu-id="fcc80-127">Other fields default to `$filter` behavior.</span></span> <span data-ttu-id="fcc80-128">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="fcc80-128">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="fcc80-129">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="fcc80-129">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="fcc80-130">Para obter mais informações sobre as opções de consulta OData, veja [ Parâmetros de consulta OData ](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fcc80-130">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcc80-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc80-131">Request headers</span></span>

| <span data-ttu-id="fcc80-132">Nome</span><span class="sxs-lookup"><span data-stu-id="fcc80-132">Name</span></span> | <span data-ttu-id="fcc80-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcc80-133">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="fcc80-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcc80-134">Authorization</span></span>  | <span data-ttu-id="fcc80-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcc80-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fcc80-137">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="fcc80-137">ConsistencyLevel</span></span> | <span data-ttu-id="fcc80-138">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="fcc80-138">eventual.</span></span> <span data-ttu-id="fcc80-139">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="fcc80-139">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="fcc80-140">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="fcc80-140">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcc80-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc80-141">Request body</span></span>
<span data-ttu-id="fcc80-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fcc80-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcc80-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcc80-143">Response</span></span>
<span data-ttu-id="fcc80-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcc80-144">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="fcc80-145">A resposta inclui somente as propriedades padrão de cada grupo.</span><span class="sxs-lookup"><span data-stu-id="fcc80-145">The response includes only the default properties of each group.</span></span>

## <a name="examples"></a><span data-ttu-id="fcc80-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fcc80-146">Examples</span></span>

### <a name="example-1-get-a-list-of-groups"></a><span data-ttu-id="fcc80-147">Exemplo 1: Obter uma lista de grupos</span><span class="sxs-lookup"><span data-stu-id="fcc80-147">Example 1: Get a list of groups</span></span>

#### <a name="request"></a><span data-ttu-id="fcc80-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc80-148">Request</span></span>

<span data-ttu-id="fcc80-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcc80-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="fcc80-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcc80-150">Response</span></span>

<span data-ttu-id="fcc80-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fcc80-151">The following is an example of the response.</span></span>

><span data-ttu-id="fcc80-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fcc80-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fcc80-153">Todas as propriedades padrão são retornadas para cada grupo em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcc80-153">All the default properties are returned for each group in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "mail": "group1@contoso.com",
      "mailEnabled": true,
      "mailNickname": "ContosoGroup1",
      "securityEnabled": true
    }
  ]
}

```

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a><span data-ttu-id="fcc80-154">Exemplo 2: Obter uma lista filtrada de grupos, incluindo a contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="fcc80-154">Example 2: Get a filtered list of groups including the count of returned objects</span></span>

<span data-ttu-id="fcc80-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcc80-155">The following is an example of the request.</span></span>

#### <a name="request"></a><span data-ttu-id="fcc80-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc80-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="fcc80-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcc80-157">Response</span></span>

<span data-ttu-id="fcc80-158">Veja a seguir o exemplo de uma resposta que inclui apenas as propriedades solicitadas.</span><span class="sxs-lookup"><span data-stu-id="fcc80-158">The following is an example of the response which includes only the requested properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName)",
  "@odata.count":2,
  "value": [
    {
      "id": "11111111-2222-3333-4444-555555555555",
      "displayName": "Contoso Group 1"
    },
    {
      "id": "22222222-3333-4444-5555-666666666666",
      "displayName": "Contoso Group 2"
    }
  ]
}
```

### <a name="example-3-get-only-a-count-of-groups"></a><span data-ttu-id="fcc80-159">Exemplo 3: Obter apenas uma contagem de grupos</span><span class="sxs-lookup"><span data-stu-id="fcc80-159">Example 3: Get only a count of groups</span></span>

#### <a name="request"></a><span data-ttu-id="fcc80-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc80-160">Request</span></span>

<span data-ttu-id="fcc80-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcc80-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
  }-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="fcc80-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcc80-162">Response</span></span>

<span data-ttu-id="fcc80-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fcc80-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`893`

### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="fcc80-164">Exemplo 4: Utilize $filter e $top para obter um grupo com um nome de exibição que comece com 'a', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="fcc80-164">Example 4: Use $filter and $top to get one group with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="fcc80-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc80-165">Request</span></span>

<span data-ttu-id="fcc80-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcc80-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="fcc80-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcc80-167">Response</span></span>

<span data-ttu-id="fcc80-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fcc80-168">The following is an example of the response.</span></span>

><span data-ttu-id="fcc80-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcc80-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count":1,
  "value":[
    {
      "displayName":"a",
      "mailNickname":"a241"
    }
  ]
}
```

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="fcc80-171">Exemplo 5: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'Vídeo', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="fcc80-171">Example 5: Use $search to get groups with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="fcc80-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc80-172">Request</span></span>

<span data-ttu-id="fcc80-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcc80-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="fcc80-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcc80-174">Response</span></span>

<span data-ttu-id="fcc80-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fcc80-175">The following is an example of the response.</span></span>

><span data-ttu-id="fcc80-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcc80-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    }
  ]
}
```

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a><span data-ttu-id="fcc80-178">Exemplo 6: Utilize $search para obter grupos com nomes de exibição que contenham as letras 'Vídeo' ou uma descrição que contenha as letras 'prod', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="fcc80-178">Example 6: Use $search to get groups with display names that contain the letters 'Video' or a description that contains the letters 'prod' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="fcc80-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcc80-179">Request</span></span>

<span data-ttu-id="fcc80-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcc80-180">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="fcc80-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcc80-181">Response</span></span>

<span data-ttu-id="fcc80-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fcc80-182">The following is an example of the response.</span></span>

><span data-ttu-id="fcc80-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcc80-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    },
    {
      "description":"Video Production",
      "displayName":"Video Production",
      "mail":"videoprod@service.contoso.com",
      "mailNickname":"VideoProduction"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

