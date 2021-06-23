---
title: Obter as alterações incrementais para usuários
description: A consulta delta permite que você consulte adições, exclusões ou atualizações de usuários, por meio de uma série de chamadas de função delta. A consulta Delta permite que você descubra alterações em usuários sem ter que buscar todo o conjunto de usuários do Microsoft Graph e comparar as alterações.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 39253f03175c9c33c6e358afc2e629a77e449a0c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082059"
---
# <a name="get-incremental-changes-for-users"></a><span data-ttu-id="6c9fc-104">Obter as alterações incrementais para usuários</span><span class="sxs-lookup"><span data-stu-id="6c9fc-104">Get incremental changes for users</span></span>

<span data-ttu-id="6c9fc-p102">A [consulta delta](./delta-query-overview.md) permite que você consulte adições, exclusões ou atualizações de usuários, por meio de uma série de chamadas de função [delta](/graph/api/user-delta?view=graph-rest-1.0). A consulta Delta permite que você descubra alterações em usuários sem ter que buscar todo o conjunto de usuários do Microsoft Graph e comparar as alterações.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-p102">[Delta query](./delta-query-overview.md) lets you query for additions, deletions, or updates to users, by way of a series of [delta](/graph/api/user-delta?view=graph-rest-1.0) function calls. Delta query enables you discover changes to users without having to fetch the entire set of users from Microsoft Graph and compare changes.</span></span>

<span data-ttu-id="6c9fc-p103">Clientes que sincronizam usuários com um repositório de perfil local podem usar a Consulta Delta para a sincronização completa inicial juntamente com as sincronizações incrementais no futuro. Normalmente, um cliente faria uma sincronização completa inicial de todos os usuários em um locatário e, logo após, obteria alterações incrementais para esses usuários periodicamente.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-p103">Clients using synchronizing users with a local profile store can use Delta Query for both their initial full synchronization along with incremental synchronizations in the future. Typically, a client would do an initial full synchronization of all the users in a tenant, and subsequently, get incremental changes to users periodically.</span></span>

## <a name="tracking-user-changes"></a><span data-ttu-id="6c9fc-109">Controle de alterações de usuários</span><span class="sxs-lookup"><span data-stu-id="6c9fc-109">Tracking user changes</span></span>

<span data-ttu-id="6c9fc-p104">O controle de alterações de usuários corresponde a uma série de uma ou mais solicitações GET com a função **delta**. Criar uma solicitação GET é muito parecido com a forma de [listar usuários](/graph/api/user-list?view=graph-rest-1.0), exceto se você incluir o seguinte:</span><span class="sxs-lookup"><span data-stu-id="6c9fc-p104">Tracking user changes is a round of one or more GET requests with the **delta** function. You make a GET request much like the way you [list users](/graph/api/user-list?view=graph-rest-1.0), except that you include the following:</span></span>

- <span data-ttu-id="6c9fc-112">A função **delta**.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-112">The **delta** function.</span></span>
- <span data-ttu-id="6c9fc-113">Um [token de estado](./delta-query-overview.md) (_deltaToken_ ou _skipToken_) da chamada de função GET **delta** anterior.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-113">A [state token](./delta-query-overview.md) (_deltaToken_ or _skipToken_) from the previous GET **delta** function call.</span></span>

## <a name="example"></a><span data-ttu-id="6c9fc-114">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c9fc-114">Example</span></span>

<span data-ttu-id="6c9fc-115">O exemplo a seguir mostra uma série de solicitações para rastrear as alterações nos usuários:</span><span class="sxs-lookup"><span data-stu-id="6c9fc-115">The following example shows a series  requests to track changes to users:</span></span>

1. <span data-ttu-id="6c9fc-116">[Solicitação inicial](#initial-request) e [resposta](#initial-response)</span><span class="sxs-lookup"><span data-stu-id="6c9fc-116">[Initial request](#initial-request) and [response](#initial-response)</span></span>
2. <span data-ttu-id="6c9fc-117">[solicitação nextLink](#nextlink-request) e [resposta](#nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="6c9fc-117">[nextLink request](#nextlink-request) and [response](#nextlink-response)</span></span>
3. <span data-ttu-id="6c9fc-118">[Solicitação final nextLink](#final-nextlink-request) e [resposta](#final-nextlink-response)</span><span class="sxs-lookup"><span data-stu-id="6c9fc-118">[Final nextLink request](#final-nextlink-request) and [response](#final-nextlink-response)</span></span>
4. <span data-ttu-id="6c9fc-119">[Solicitação deltaLink](#deltalink-request) e [resposta deltaLink](#deltalink-response)</span><span class="sxs-lookup"><span data-stu-id="6c9fc-119">[deltaLink request](#deltalink-request) and [deltaLink response](#deltalink-response)</span></span>

## <a name="initial-request"></a><span data-ttu-id="6c9fc-120">Solicitação inicial</span><span class="sxs-lookup"><span data-stu-id="6c9fc-120">Initial request</span></span>

<span data-ttu-id="6c9fc-121">Para iniciar o controle das alterações no recurso de usuário, faça uma solicitação incluindo a função delta do recurso de usuário.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-121">To begin tracking changes in the user resource, you make a request including the delta function on the user resource.</span></span>

<span data-ttu-id="6c9fc-122">Observe o seguinte:</span><span class="sxs-lookup"><span data-stu-id="6c9fc-122">Note the following:</span></span>

- <span data-ttu-id="6c9fc-123">O parâmetro de consulta $select opcional está incluído na solicitação para demonstrar como os parâmetros de consulta são automaticamente incluídos nas futuras solicitações.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-123">The optional $select query parameter is included in the request to demonstrate how query parameters are automatically included in future requests.</span></span>
- <span data-ttu-id="6c9fc-p105">A solicitação inicial não inclui um token de estado. Os tokens de estado serão usados nas solicitações subsequentes.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-p105">The initial request does not include a state token. State tokens will be used in subsequent requests.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

## <a name="initial-response"></a><span data-ttu-id="6c9fc-126">Resposta inicial</span><span class="sxs-lookup"><span data-stu-id="6c9fc-126">Initial response</span></span>

<span data-ttu-id="6c9fc-p106">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [user](/graph/api/resources/user?view=graph-rest-1.0) no corpo da resposta. Pressupondo que todo o conjunto de usuários é muito grande, a resposta também incluirá um token de estado nextLink.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-p106">If successful, this method returns `200 OK` response code and [user](/graph/api/resources/user?view=graph-rest-1.0) collection object in the response body. Assuming the entire set of users is too large, the response will also include a nextLink state token.</span></span>

<span data-ttu-id="6c9fc-p107">Neste exemplo, uma URL nextLink é retornada indicando que não há páginas adicionais de dados a serem recuperados na sessão. O parâmetro de consulta $select da solicitação inicial é codificado na URL nextLink.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-p107">In this example, a nextLink URL is returned indicating there are additional pages of data to be retrieved in the session. The $select query parameter from the initial request is encoded into the nextLink URL.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Testuser1",
      "givenName":"John",
      "surname":"Doe",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Testuser2",
      "givenName":"Jane",
      "surname":"Doe",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    }
  ]
}
```

## <a name="nextlink-request"></a><span data-ttu-id="6c9fc-131">solicitação nextLink</span><span class="sxs-lookup"><span data-stu-id="6c9fc-131">nextLink request</span></span>

<span data-ttu-id="6c9fc-p108">A segunda solicitação especifica o `skipToken` retornado da resposta anterior. Observe que o parâmetro `$select` não é obrigatório, pois o `skipToken` codifica e o inclui.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-p108">The second request specifies the `skipToken` returned from the previous response. Notice the `$select` parameter is not required, as the `skipToken` encodes and includes it.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

## <a name="nextlink-response"></a><span data-ttu-id="6c9fc-134">Resposta nextLink</span><span class="sxs-lookup"><span data-stu-id="6c9fc-134">nextLink response</span></span>

<span data-ttu-id="6c9fc-135">A resposta contém outro `nextLink` com outro valor de `skipToken`, indicando que há mais grupos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-135">The response contains another `nextLink` with a new `skipToken` value, which indicates that more groups are available.</span></span> <span data-ttu-id="6c9fc-136">Você deve continuar criando solicitações usando a `nextLink` URL até que uma `deltaLink` URL seja retornada na resposta final, mesmo que o valor seja uma matriz vazia (isso pode ocorrer em determinadas circunstâncias).</span><span class="sxs-lookup"><span data-stu-id="6c9fc-136">You should continue making requests using the `nextLink` URL until a `deltaLink` URL is returned in the final response, even if the value is an empty array (this can happen under certain circumstances).</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Testuser3",
      "givenName":"Pat",
      "surname":"Doe",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Testuser4",
      "givenName":"Meghan",
      "surname":"Doe",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

## <a name="final-nextlink-request"></a><span data-ttu-id="6c9fc-137">Solicitação nextLink final</span><span class="sxs-lookup"><span data-stu-id="6c9fc-137">Final nextLink request</span></span>

<span data-ttu-id="6c9fc-138">A terceira solicitação continua a usar os últimos `skipToken` retornados da última solicitação de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-138">The third request continues to use the latest `skipToken` returned from the last sync request.</span></span> 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a><span data-ttu-id="6c9fc-139">Resposta nextLink final</span><span class="sxs-lookup"><span data-stu-id="6c9fc-139">Final nextLink response</span></span>

<span data-ttu-id="6c9fc-p110">Quando a URL deltaLink é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL deltaLink para se inteirar das alterações feitas no recurso. Salve o `deltaToken` e use-o na solicitação da URL para descobrir as alterações feitas nos usuários.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-p110">When the deltaLink URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the deltaLink URL to learn about changes to the resource. Save the `deltaToken` and use it in the request URL to discover changes to users.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Testuser5",
      "givenName":"Al",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Testuser6",
      "givenName":"Sam",
      "surname":"Doe",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

## <a name="deltalink-request"></a><span data-ttu-id="6c9fc-143">Solicitação deltaLink</span><span class="sxs-lookup"><span data-stu-id="6c9fc-143">deltaLink request</span></span>

<span data-ttu-id="6c9fc-144">Usando o `deltaToken` da [última resposta](#final-nextlink-response), você poderá obter usuários alterados (ao ser adicionado, excluído ou atualizado) desde o último pedido.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-144">Using the `deltaToken` from the [last response](#final-nextlink-response), you will be able to get changed (by being added, deleted, or updated) users since the last request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a><span data-ttu-id="6c9fc-145">Resposta deltaLink</span><span class="sxs-lookup"><span data-stu-id="6c9fc-145">deltaLink response</span></span>

<span data-ttu-id="6c9fc-146">Se não houve alterações, uma diferente `deltatoken` é retornada com nenhum resultado.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-146">If no changes have occurred, a different `deltatoken` is returned with no results.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": []
}
```

<span data-ttu-id="6c9fc-147">Se houve alterações, uma diferente `deltatoken` é retornada incluindo um conjunto de usuários alterados.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-147">If changes have occurred, a different `deltatoken` is returned including a collection of changed users.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": [
    {
      "displayName":"Testuser7",
      "givenName":"Joe",
      "surname":"Doe",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "id":"8ffff70c-1c63-4860-b963-e34ec660931d",
      "@removed": {
         "reason": "changed"
      }
    }
  ]
}
```

<span data-ttu-id="6c9fc-148">Alguns aspectos a observar sobre a resposta do exemplo acima:</span><span class="sxs-lookup"><span data-stu-id="6c9fc-148">Some things to note about the previous example response:</span></span>

- <span data-ttu-id="6c9fc-149">Quando o usuário é excluído, o item contém uma anotação: `@removed` com valor de `"reason": "changed"`.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-149">When the user is deleted, the item contains an annotation: `@removed` with value of `"reason": "changed"`.</span></span>

- <span data-ttu-id="6c9fc-150">Quando o usuário é excluído permanentemente, o item contém uma anotação: `@removed` com valor de `"reason": "deleted"`.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-150">When the user is permanently deleted, the item contains an annotation: `@removed` with value of `"reason": "deleted"`.</span></span>

- <span data-ttu-id="6c9fc-151">Quando o usuário é criado ou restaurado, não há nenhuma anotação.</span><span class="sxs-lookup"><span data-stu-id="6c9fc-151">When the user is created, or restored, there is no annotation.</span></span>

## <a name="see-also"></a><span data-ttu-id="6c9fc-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="6c9fc-152">See also</span></span>
<span data-ttu-id="6c9fc-153">Visão geral da [consulta delta do Microsoft Graph](delta-query-overview.md).</span><span class="sxs-lookup"><span data-stu-id="6c9fc-153">[Microsoft Graph delta query](delta-query-overview.md) overview.</span></span>
