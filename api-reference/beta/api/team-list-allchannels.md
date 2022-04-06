---
title: Listar allChannels
description: Obtenha a lista de canais nesta equipe ou compartilhados com essa equipe (canais de entrada).
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 4f5f025062089d3550fe8f2212b353757059bd12
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685317"
---
# <a name="list-allchannels"></a>Listar allChannels
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a lista de [canais nesta](../resources/channel.md) equipe [ou](../resources/team.md) compartilhados com essa [equipe](../resources/team.md) (canais de entrada).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All |


> **Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/allChannels
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método oferece suporte aos parâmetros de consulta `$filter` e `$select`[OData](/graph/query-parameters)para ajudar a personalizar a resposta.

### <a name="use-select-for-better-performance"></a>Use $select para melhorar o desempenho
Preencher as propriedades **email** e **moderationSettings** de um canal é uma operação cara que resulta em desempenho lento. Use `$select` para excluir o **email** e as propriedades **moderationSettings** para melhorar o desempenho.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e uma coleção de objetos [de](../resources/channel.md) canal no corpo da resposta. A resposta também inclui a **propriedade @odata.id** que pode ser usada para acessar o canal e executar outras operações no objeto [de](../resources/channel.md) canal.

> [!Note]
> Atualmente, a invocação da URL retornada da propriedade **@odata.id** falha para canais compartilhados entre locatários. Você poderá resolver esse problema se remover a `/tenants/{tenant-id}` parte da URL antes de chamar essa API. Para obter mais detalhes, consulte [Problemas conhecidos com o Microsoft Graph](/graph/known-issues#unable-to-access-a-cross-tenant-shared-channel-when-the-request-url-contains-tenantscross-tenant-id).

## <a name="examples"></a>Exemplos

### <a name="example-1-list-all-channels"></a>Exemplo 1: Listar todos os canais

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "list_all_channel"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/allChannels
```


#### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
       "@odata.id": "https://graph.microsoft.com/beta/tenants/b3246f44-b4gb-4627-96c6-25b18fa2c910/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "General",
      "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
      "membershipType": "standard",
      "tenantId": "b3246f44-b4gb-4627-96c6-25b18fa2c910"
    },
    {
       "@odata.id": "https://graph.microsoft.com/beta/tenants/b3246f44-b4gb-5678-96c6-25b18fa2c910/teams/893075dd-5678-5634-925f-022c42e20265/channels/19:561fbdbbfca848a484gabdf00ce9dbbd@thread.tacv",
      "id": "19:561fbdbbfca848a484gabdf00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "Shared channel from Contosso",
      "membershipType": "shared",
      "tenantId": "b3246f44-b4gb-5678-96c6-25b18fa2c910"
    }
  ]
}
```


### <a name="example-2-list-all-shared-channels"></a>Exemplo 2: Listar todos os canais compartilhados

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "list_all_shared_channel"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/allChannels?$filter=membershipType eq 'shared'
```


#### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
       "@odata.id": "https://graph.microsoft.com/beta/tenants/b3246f44-b4gb-5678-96c6-25b18fa2c910/teams/893075dd-5678-5634-925f-022c42e20265/channels/19:561fbdbbfca848a484gabdf00ce9dbbd@thread.tacv",
      "id": "19:561fbdbbfca848a484gabdf00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "Shared channel from Contosso",
      "membershipType": "shared",
      "tenantId": "b3246f44-b4gb-5678-96c6-25b18fa2c910"
    }
  ]
}
```

