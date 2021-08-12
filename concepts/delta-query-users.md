---
title: Obter as alterações incrementais para usuários
description: A consulta delta permite que você consulte adições, exclusões ou atualizações de usuários, por meio de uma série de chamadas de função delta. A consulta Delta permite que você descubra alterações em usuários sem ter que buscar todo o conjunto de usuários do Microsoft Graph e comparar as alterações.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: be944c68d3c21fae5c1267cf95a7a926faaa2b355e6ea96dcb160b6f55107138
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180436"
---
# <a name="get-incremental-changes-for-users"></a>Obter as alterações incrementais para usuários

A [consulta delta](./delta-query-overview.md) permite que você consulte adições, exclusões ou atualizações de usuários, por meio de uma série de chamadas de função [delta](/graph/api/user-delta?view=graph-rest-1.0). A consulta Delta permite que você descubra alterações em usuários sem ter que buscar todo o conjunto de usuários do Microsoft Graph e comparar as alterações.

Clientes que sincronizam usuários com um repositório de perfil local podem usar a Consulta Delta para a sincronização completa inicial juntamente com as sincronizações incrementais no futuro. Normalmente, um cliente faria uma sincronização completa inicial de todos os usuários em um locatário e, logo após, obteria alterações incrementais para esses usuários periodicamente.

## <a name="tracking-user-changes"></a>Controle de alterações de usuários

O controle de alterações de usuários corresponde a uma série de uma ou mais solicitações GET com a função **delta**. Criar uma solicitação GET é muito parecido com a forma de [listar usuários](/graph/api/user-list?view=graph-rest-1.0), exceto se você incluir o seguinte:

- A função **delta**.
- Um [token de estado](./delta-query-overview.md) (_deltaToken_ ou _skipToken_) da chamada de função GET **delta** anterior.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra uma série de solicitações para rastrear as alterações nos usuários:

1. [Solicitação inicial](#initial-request) e [resposta](#initial-response)
2. [solicitação nextLink](#nextlink-request) e [resposta](#nextlink-response)
3. [Solicitação final nextLink](#final-nextlink-request) e [resposta](#final-nextlink-response)
4. [Solicitação deltaLink](#deltalink-request) e [resposta deltaLink](#deltalink-response)

## <a name="initial-request"></a>Solicitação inicial

Para iniciar o controle das alterações no recurso de usuário, faça uma solicitação incluindo a função delta do recurso de usuário.

Observe o seguinte:

- O parâmetro de consulta $select opcional está incluído na solicitação para demonstrar como os parâmetros de consulta são automaticamente incluídos nas futuras solicitações.
- A solicitação inicial não inclui um token de estado. Os tokens de estado serão usados nas solicitações subsequentes.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

## <a name="initial-response"></a>Resposta inicial

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção [user](/graph/api/resources/user?view=graph-rest-1.0) no corpo da resposta. Pressupondo que todo o conjunto de usuários é muito grande, a resposta também incluirá um token de estado nextLink.

Neste exemplo, uma URL nextLink é retornada indicando que não há páginas adicionais de dados a serem recuperados na sessão. O parâmetro de consulta $select da solicitação inicial é codificado na URL nextLink.

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

## <a name="nextlink-request"></a>solicitação nextLink

A segunda solicitação especifica o `skipToken` retornado da resposta anterior. Observe que o parâmetro `$select` não é obrigatório, pois o `skipToken` codifica e o inclui.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

## <a name="nextlink-response"></a>Resposta nextLink

A resposta contém outro `nextLink` com outro valor de `skipToken`, indicando que há mais grupos disponíveis. Você deve continuar criando solicitações usando a `nextLink` URL até que uma `deltaLink` URL seja retornada na resposta final, mesmo que o valor seja uma matriz vazia (isso pode ocorrer em determinadas circunstâncias).

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

## <a name="final-nextlink-request"></a>Solicitação nextLink final

A terceira solicitação continua a usar os últimos `skipToken` retornados da última solicitação de sincronização. 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

## <a name="final-nextlink-response"></a>Resposta nextLink final

Quando a URL deltaLink é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL deltaLink para se inteirar das alterações feitas no recurso. Salve o `deltaToken` e use-o na solicitação da URL para descobrir as alterações feitas nos usuários. 

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

## <a name="deltalink-request"></a>Solicitação deltaLink

Usando o `deltaToken` da [última resposta](#final-nextlink-response), você poderá obter usuários alterados (ao ser adicionado, excluído ou atualizado) desde o último pedido.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a>Resposta deltaLink

Se não houve alterações, uma diferente `deltatoken` é retornada com nenhum resultado.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": []
}
```

Se houve alterações, uma diferente `deltatoken` é retornada incluindo um conjunto de usuários alterados.

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

Alguns aspectos a observar sobre a resposta do exemplo acima:

- Quando o usuário é excluído, o item contém uma anotação: `@removed` com valor de `"reason": "changed"`.

- Quando o usuário é excluído permanentemente, o item contém uma anotação: `@removed` com valor de `"reason": "deleted"`.

- Quando o usuário é criado ou restaurado, não há nenhuma anotação.

## <a name="see-also"></a>Confira também
Visão geral da [consulta delta do Microsoft Graph](delta-query-overview.md).
