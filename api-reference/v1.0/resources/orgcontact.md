---
title: Tipo de recurso orgContact
description: Representa um contato organizacional
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5db56af8b2f734044331c0aab3320c6e25d49e39
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014296"
---
# <a name="orgcontact-resource-type"></a>Tipo de recurso orgContact

Namespace: microsoft.graph

Representa um contato organizacional. Os contatos organizacionais são gerenciados pelos administradores de uma organização e são diferentes dos [contatos pessoais.](contact.md) Além disso, os contatos organizacionais são sincronizados de diretórios locais ou de Exchange Online e são somente leitura no Microsoft Graph.

Herda de [directoryObject](directoryobject.md).

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/orgcontact-delta.md). Esse recurso é um tipo aberto que permite que outras propriedades sejam passadas.

## <a name="methods"></a>Methods

| Método                                                                  | Tipo de retorno                                      | Descrição                                                                                                                 |
|:------------------------------------------------------------------------|:-------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------|
| **Contatos organizacionais** |
| [Listar contatos organizacionais](../api/orgcontact-list.md)               | [orgContact](orgcontact.md)                      | Listar propriedades de contatos organizacionais.                                                                                 |
| [Obter contato organizacional](../api/orgcontact-get.md)                  | [orgContact](orgcontact.md)                      | Ler propriedades e relações de um contato organizacional.                                                             |
| **Hierarquia organizacional** |
| [Obter gerenciador](../api/orgcontact-get-manager.md)                         | [directoryObject](directoryobject.md)            | Obter o gerente do contato organizacional.                                                                                   |
| [Listar directReports](../api/orgcontact-list-directreports.md)           | Coleção [directoryObject](directoryobject.md) | Listar os relatórios diretos do contato organizacional.                                                                           |
| [Listar memberOf](../api/orgcontact-list-memberof.md)                     | Coleção [directoryObject](directoryobject.md) | Listar os grupos de que um contato organizacional é membro.                                                                   |
| [Listar transitiveMemberOf](../api/orgcontact-list-transitivememberof.md) | Conjunto [directoryObject](directoryobject.md) | Listar os grupos dos quais um contato organizacional é membro, incluindo grupos nos quais o contato organizacional está aninhado. |
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md)             | Coleção de cadeias de caracteres                                | Verifique se há associação ao grupo.                                                                                                 |
| [getMemberGroups](../api/directoryobject-getmembergroups.md)                 | Coleção de cadeias de caracteres                                | Retorne todos os grupos dos que o contato organizacional especificado é membro.                                             |
| [getMemberObjects](../api/directoryobject-getmemberobjects.md)               | Coleção de cadeias de caracteres                                | Retorna uma lista de directoryObjects do qual o contato organizacional é membro.                                               |

## <a name="properties"></a>Propriedades

> [!IMPORTANT]
> O uso específico de `$filter` e o parâmetro de consulta `$search` é suportado somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries#organizational-contacts-properties).

| Propriedade                     | Tipo                                                                     | Descrição                                                                                                                                                                                                                                                                                                                        |
|:-----------------------------|:-------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| addresses                    | [Coleção physicalOfficeAddress](physicalofficeaddress.md)             | Endereços postais para esse contato organizacional. Por enquanto, um contato só pode ter um endereço físico.                                                                                                                                                                                                                            |
| CompanyName                  | String                                                                   | Nome da empresa à que esse contato organizacional pertence.  Suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` no `null` valores).                                                                                                                                                                                          |
| departamento                   | String                                                                   | O nome do departamento no qual o contato funciona.  Suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` no `null` valores).                                                                                                                                                                                                   |
| displayName                  | String                                                                   | Nome de exibição para esse contato organizacional. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores), `$search`, e `$orderBy`.                                                                                                                                                                                   |
| givenName                    | String                                                                   | Primeiro nome para esse contato organizacional. Suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` no `null` valores).                                                                                                                                                                                                                |
| id                           | String                                                                   | Identificador exclusivo para esse contato organizacional.  Suporta `$filter` (`eq`, `ne`, `not`, `in`).                                                                                                                                                                                                                                  |
| jobTitle                     | String                                                                   | Cargo para esse contato organizacional. Suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` no `null` valores).                                                                                                                                                                                                                 |
| email                         | String                                                                   | O endereço SMTP do contato, por exemplo, "jeff@contoso.onmicrosoft.com". Suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` no `null` valores).                                                                                                                                                                             |
| mailNickname                 | String                                                                   | Alias de email (parte do endereço de email pré-pendente do símbolo @) para esse contato organizacional. Suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` no `null` valores).                                                                                                                                                           |
| onPremisesLastSyncDateTime   | DateTimeOffset                                                           | Data e hora em que esse contato organizacional foi sincronizado pela última vez do AD local. Essas informações de data e hora usam o formato ISO 8601 e estão sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`).                             |
| onPremisesProvisioningErrors | coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md) | Lista de erros de provisionamento de sincronização para esse contato organizacional. Suporta `$filter` (`eq`, `not`).                                                                                                                                                                                                                 |
| onPremisesSyncEnabled        | Boolean                                                                  | `true`se esse objeto for sincronizado de um diretório local; se esse objeto tiver sido originalmente sincronizado de um diretório local, mas não estiver mais sincronizado e agora mestre no Exchange; se esse objeto nunca tiver sido sincronizado de um diretório local `false` `null` (padrão). <br/> <br/> Suporte `$filter` (`eq`, `ne`, `not`, `in`, e `eq` no `null` valores). |
| telefones                       | Coleção [phone](phone.md)                                             | Lista de telefones para esse contato organizacional. Telefone tipos podem ser móveis, comerciais e businessFax. Somente um de cada tipo pode estar presente na coleção.                                                                                                                                                                 |
| proxyAddresses               | Coleção de cadeias de caracteres                                                        | Por exemplo: "SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com". O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. Suporta `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).                                                                                                               |
| surname                      | String                                                                   | Sobrenome para esse contato organizacional. Suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` no `null` valores).                                                                                                                                                                                                                 |

## <a name="relationships"></a>Relações

| Relação       | Tipo                                             | Descrição                                                                                                                                            |
|:-------------------|:-------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------|
| directReports      | Coleção [directoryObject](directoryobject.md) | Os relatórios diretos do contato. (Os usuários e contatos que têm suas propriedades de gerente definidas para esse contato.)  Somente leitura. Anulável. Suporta o `$expand`. |
| manager            | [directoryObject](directoryobject.md)            | O usuário ou contato que é o gerente desse contato. Somente leitura. Suporta o `$expand`.                                                                     |
| memberOf           | Coleção [directoryObject](directoryobject.md) | Grupos dos que esse contato é membro. Somente leitura. Anulável. Suporta o `$expand`.                                                                      |
| transitiveMemberOf | Conjunto [directoryObject](directoryobject.md) | Grupos dos quais esse contato é membro, incluindo grupos nos quais o contato está aninhado. Somente leitura. Anulável.                                       |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.orgcontact"
}-->

```json
{
  "addresses": [{"@odata.type": "microsoft.graph.physicalOfficeAddress"}],
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "string (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "proxyAddresses": ["string"],
  "surname": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

