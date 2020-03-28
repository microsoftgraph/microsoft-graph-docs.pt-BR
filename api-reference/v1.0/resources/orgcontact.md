---
title: tipo de recurso orgContact
description: Representa um contato organizacional
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 44fdd10d1e86405c9a24ed0dab97125e3cc52360
ms.sourcegitcommit: 2ac179fb774a15c9e9c01502e59c76efb57803a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2020
ms.locfileid: "42986072"
---
# <a name="orgcontact-resource-type"></a>tipo de recurso orgContact

Namespace: microsoft.graph

Representa um contato organizacional. Os contatos organizacionais são gerenciados pelos administradores de uma organização e são diferentes dos [contatos pessoais](contact.md). Além disso, os contatos organizacionais são sincronizados a partir dos diretórios locais ou do Exchange Online e são somente leitura.

Herda de [directoryObject](directoryobject.md).

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/orgcontact-delta.md).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar contatos da organização](../api/orgcontact-list.md) | [orgContact](orgcontact.md) |Listar Propriedades de contatos organizacionais.|
|[Obter contato da organização](../api/orgcontact-get.md) | [orgContact](orgcontact.md) |Leia as propriedades e as relações de um contato organizacional.|
|[Obter gerenciador](../api/orgcontact-get-manager.md) |[directoryObject](directoryobject.md)| Obtenha o gerente do contato organizacional.|
|[Listar directReports](../api/orgcontact-list-directreports.md) |Coleção [directoryObject](directoryobject.md)| Listar os subordinados diretos do contato organizacional.|
|[List memberOf](../api/orgcontact-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Listar os grupos dos quais um contato organizacional é membro.|
|[Listar transitiveMemberOf](../api/orgcontact-list-transitivememberof.md) |Coleção [directoryObject](directoryobject.md)| Listar os grupos dos quais um contato organizacional é membro, incluindo grupos nos quais o contato organizacional está aninhado.|
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|String collection| Verifique a associação ao grupo. |
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|String collection| Retornar todos os grupos dos quais o contato organizacional especificado é membro. |
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|String collection| Retorna uma lista de directoryObjects o contato organizacional é um membro. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| endereços                    | coleção [physicalOfficeAddress](physicalofficeaddress.md)           | Endereços postais para este contato organizacional. Por enquanto, um contato só pode ter um endereço físico. |
| companyName                  | String                                                    | Nome da empresa à qual este contato organizacional pertence.                                                                                                                                                                                                                                                                                                                 |
| department                   | String                                                     | O nome do departamento no qual o contato funciona.                                                                                                                                                                                                                                                                                                                                |
| displayName                  | Cadeia de caracteres                                                     | Nome para exibição desse contato organizacional.                                                                                                                                                                                                                                                                                                                                   |
| givenName                    | String                                                     | Nome para este contato organizacional.                                                                                                                                                                                                                                                                                                                                     |
| id                           | String                                                     | Identificador exclusivo desse contato organizacional.                                                                                                                                                                                                                                                                                                                             |
| jobTitle                     | String                                                     | Cargo para este contato organizacional.                                                                                                                                                                                                                                                                                                                                      |
|email|String| O endereço SMTP do contato, por exemplo, "jeff@contoso.onmicrosoft.com". |
| mailNickname                 | String                                                     | Alias de email (parte do endereço de email, esperando o símbolo @) desse contato organizacional.                                                                                                                                                                                                                                                                                |
| onPremisesLastSyncDateTime   | DateTimeOffset                                             | Data e hora da última sincronização do contato organizacional do AD local. Essas informações de data e hora usam o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.   |
| onPremisesProvisioningErrors |coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md)       | Lista de erros de provisionamento de sincronização para este contato organizacional.                                                                                                                                                                                                                                                                                                |
|onPremisesSyncEnabled|Booliano|**true** se esse objeto for sincronizado a partir de um diretório local; **false** se esse objeto foi originalmente sincronizado a partir de um diretório local, mas não é mais sincronizado e agora é Mastered no Exchange; **NULL** se esse objeto nunca tiver sido sincronizado a partir de um diretório local (padrão).|
| telefones                       | Coleção [phone](phone.md)                            | Lista de telefones para este contato organizacional. Os tipos de telefone podem ser móveis, de negócios e de businessFax. Somente um de cada tipo pode estar presente na coleção.                                                                                                                       |
| proxyAddresses               | Coleção de cadeias de caracteres                                         | Por exemplo: "SMTP: bob@contoso.com", "SMTP: bob@sales.contoso.com". O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. Oferece \$suporte a filtro.                                                                                                                                                                               |
| surname                      | String                                                     | Sobrenome para este contato organizacional.                          |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|directReports|Coleção [directoryObject](directoryobject.md)| Os subordinados diretos do contato. (Os usuários e contatos que têm a propriedade do gerente definidas para este contato.)  Somente leitura. Anulável.|
|manager|[directoryObject](directoryobject.md)| O usuário ou contato que é o gerente do contato. Apenas leitura.|
|memberOf|Coleção [directoryObject](directoryobject.md)| Grupos dos quais este contato é membro. Somente leitura. Anulável.|
|transitiveMemberOf|Coleção [directoryObject](directoryobject.md)| Grupos dos quais este contato é membro, incluindo grupos nos quais o contato está aninhado.|. Somente leitura. Anulável.|

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
