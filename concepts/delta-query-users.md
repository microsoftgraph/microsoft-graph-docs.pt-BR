---
title: Obter as alterações incrementais para usuários
description: A consulta delta no Microsoft Graph permite consultar adições, exclusões ou atualizações para recursos com suporte. Ela é habilitada por meio de uma série de solicitações delta. Para usuários, a consulta delta permite descobrir alterações sem buscar todo o conjunto de usuários para comparar as alterações.
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: d03762372a789d76d3f38121da47d662e281b2f2
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247221"
---
# <a name="get-incremental-changes-for-users"></a>Obter as alterações incrementais para usuários

A [consulta delta](./delta-query-overview.md) no Microsoft Graph permite consultar adições, exclusões ou atualizações de [recursos com suporte](delta-query-overview.md#supported-resources). Ela é habilitada por meio de uma série de solicitações [delta](/graph/api/user-delta). Para usuários, a consulta delta permite descobrir alterações sem buscar todo o conjunto de usuários para comparar as alterações.

Os clientes que sincronizam usuários com um repositório de perfis local podem usar a consulta delta para a sincronização completa inicial e para as sincronizações incrementais subsequentes. Normalmente, um cliente faria uma sincronização completa inicial de todos os usuários em um locatário e, em seguida, obteria alterações incrementais nos usuários periodicamente.

## <a name="track-changes-to-users"></a>Acompanhar alterações a usuários

Acompanhe as alterações de usuários por meio de uma ou mais solicitações GET com função **delta**. A solicitação GET é como uma solicitação de [usuários de lista](/graph/api/user-list), exceto com os seguintes objetos adicionais na URL:

- A função **delta**.
- Um [token de estado](./delta-query-overview.md) (_deltaToken_ ou _skipToken_) da chamada de função GET **delta** anterior.

## <a name="example-to-track-changes-to-users"></a>Exemplo para acompanhar alterações em usuários

O exemplo a seguir mostra uma série de solicitações para controlar alterações em usuários:

1. Uma [solicitação inicial](#initial-request) e [réplica](#initial-response)
2. Uma [solicitação do nextLink](#nextlink-request) e [réplica](#nextlink-response)
3. Uma [final da solicitação nextLink](#final-nextlink-request) e [réplica](#final-nextlink-response)
4. Uma [solicitação de deltaLink](#deltalink-request) e [réplica de deltaLink](#deltalink-response)

Anote o seguinte nas réplicas:

- Quando o usuário é excluído, o item contém uma anotação: `@removed` com valor de `"reason": "changed"`.
- Quando o usuário é excluído permanentemente, o item contém uma anotação: `@removed` com valor de `"reason": "deleted"`.
- Quando o usuário é criado ou restaurado, não há nenhuma anotação.

### <a name="initial-request"></a>Solicitação inicial

Para acompanhar as alterações no recurso de usuário, faça uma solicitação e inclua a função **delta** como um segmento de URL.

Anote os seguintes itens:

- O parâmetro de consulta `$select` opcional está incluído na solicitação para demonstrar como os parâmetros de consulta são automaticamente incluídos nas futuras solicitações.
- A solicitação inicial não inclui um token de estado. Os tokens de estado serão usados em solicitações subsequentes.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$select=displayName,givenName,surname
```

### <a name="initial-response"></a>Resposta inicial

Se for bem-sucedido, esse método retornará o código de resposta `200 OK` e o objeto de coleção [user](/graph/api/resources/user) no corpo da resposta. Supondo que todo o conjunto de usuários seja muito grande, a resposta também incluirá um token de estado `@odata.nextLink` em um parâmetro `@odata.nextLink`.

Neste exemplo, um URL `@odata.nextLink` é retornado indicando que há mais páginas de dados a serem recuperadas na sessão. O parâmetro de consulta `$select` da solicitação inicial é codificado no URL `@odata.nextLink`.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users(displayName,givenName,surname)",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa",
  "value": [
    {
      "displayName":"Cameron White",
      "givenName":"Cameron",
      "surname":"White",
      "id":"ffff7b1a-13b6-477b-8c0c-380905cd99f7"
    },
    {
      "displayName":"Delia Dennis",
      "givenName":"Delia",
      "surname":"Dennis",
      "id":"605d1257-ffff-40b6-8e6f-528a53f5dc55"
    },
    {
      "id": "86462606-fde0-4fc4-9e0c-a20eb73e54c6",
      "@removed": {
        "reason": "deleted"
      }
    },
    {
      "displayName": "Conf Room Adams",
      "id": "6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0"
    }
  ]
}
```

### <a name="nextlink-request"></a>solicitação nextLink

A segunda solicitação especifica o `skipToken` retornado da resposta anterior. Observe que o parâmetro `$select` está codificado e incluído no `skipToken`.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=oEBwdSP6uehIAxQOWq_3Ksh_TLol6KIm3stvdc6hGhZRi1hQ7Spe__dpvm3U4zReE4CYXC2zOtaKdi7KHlUtC2CbRiBIUwOxPKLa
```

### <a name="nextlink-response"></a>Resposta nextLink

A resposta contém outro `@odata.nextLink` com um novo valor `skipToken`, o que indica que mais alterações controladas para usuários estão disponíveis. Use a URL `@odata.nextLink` em mais solicitações até que uma URL `@odata.deltaLink` (em um parâmetro `@odata.deltaLink`) seja retornada na resposta final, mesmo que o valor seja uma matriz vazia.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7",
  "value": [
    {
      "displayName":"Mallory Cortez",
      "givenName":"Mallory",
      "surname":"Cortez",
      "id":"d8c37826-ffff-4cae-b348-e2725b1e814b"
    },
    {
      "displayName":"Diego Sicilian",
      "givenName":"Diego",
      "surname":"Sicilian",
      "id":"8b1ee412-cd8f-4d59-ffff-24010edb9f1f"
    }
  ]
}
```

### <a name="final-nextlink-request"></a>Solicitação nextLink final

A terceira solicitação usa a última `skipToken` retornada da última solicitação de sincronização. 

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjtQ5LOhVoS7qQG_wdVCHHlbQpga7
```

### <a name="final-nextlink-response"></a>Resposta nextLink final

Quando um URL `@odata.deltaLink` é retornado, não há mais dados sobre o estado existente dos objetos de usuário. Para solicitações futuras, o aplicativo usa a URL `@odata.deltaLink` para conhecer outras alterações nos usuários. Salve o `deltaToken` e use-o no URL de solicitação subsequente para descobrir mais alterações nos usuários.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460",
  "value": [
    {
      "displayName":"Lidia Holloway",
      "givenName":"Lidia",
      "surname":"Holloway",
      "id":"25dcffff-959e-4ece-9973-e5d9b800e8cc"
    },
    {
      "displayName":"Patti Fernandez",
      "givenName":"Patti",
      "surname":"Fernandez",
      "id":"f6ede700-27d0-4c42-bfb9-4dffff43c74a"
    }
  ]
}
```

### <a name="deltalink-request"></a>Solicitação deltaLink

Usando o `deltaToken` da [última réplica](#final-nextlink-response), você receberá alterações (adições, exclusões ou atualizações) para usuários desde a última solicitação.

``` http
GET https://graph.microsoft.com/v1.0/users/delta?$deltatoken=oEcOySpF_hWYmTIUZBOIfPzcwisr_rPe8o9M54L45qEXQGmvQC6T2dbL-9O7nSU-njKhFiGlAZqewNAThmCVnNxqPu5gOBegrm1CaVZ-ZtFZ2tPOAO98OD9y0ao460
```

## <a name="deltalink-response"></a>Resposta deltaLink

Se nenhuma alteração tiver sido feita, um `@odata.deltaLink` será retornado sem resultados - a propriedade **valor** é uma matriz vazia.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": []
}
```

Se ocorreram alterações, um conjunto de objetos de usuário alterados será incluído. A resposta também contém um `@odata.nextLink`, caso haja várias páginas de alterações a serem recuperadas, ou um `@odata.deltaLink`. Implemente o mesmo padrão de seguir o `@odata.nextLink` e persistir o `@odata.deltaLink` final para chamadas futuras.

>**Observação:** essa solicitação pode ter atrasos de replicação para usuários que foram criados, atualizados ou excluídos recentemente. Repita `@odata.nextLink` ou `@odata.deltaLink` depois de algum tempo para recuperar as alterações mais recentes.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "@odata.deltaLink":"https://graph.microsoft.com/v1.0/users/delta?$deltatoken=MF1LuFYbK6Lw4DtZ4o9PDrcGekRP65WEJfDmM0H26l4v9zILCPFiPwSAAeRBghxgiwsXEfywcVQ9R8VEWuYAB50Yw3KvJ-8Z1zamVotGX2b_AHVS_Z-3b0NAtmGpod",
  "value": [
    {
      "displayName":"MOD Administrator",
      "givenName":"MOD",
      "surname":"Administrator",
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

## <a name="see-also"></a>Confira também
+ Visão geral da [consulta delta do Microsoft Graph](delta-query-overview.md).
