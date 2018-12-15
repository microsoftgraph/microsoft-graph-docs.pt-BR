---
title: tipo de recurso de orgContact
description: Veja a seguir uma representação JSON do recurso
ms.openlocfilehash: 90d25d3ef7688372e4e961220bc454a2b5607344
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283665"
---
# <a name="orgcontact-resource-type"></a>tipo de recurso de orgContact

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter orgContact](../api/orgcontact-get.md) | [orgContact](orgcontact.md) |Leia as propriedades e os relacionamentos do objeto orgContact.|
|[Obtenha manager](../api/orgcontact-get-manager.md) |[directoryObject](directoryobject.md)| Obtenha o gerente do contato.|
|[Listar directReports](../api/orgcontact-list-directreports.md) |Coleção [directoryObject](directoryobject.md)| Liste relatórios de diretos do contato.|
|[Listar memberOf](../api/orgcontact-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Obtenha uma coleção de objetos do membro.|
|[Delete](../api/orgcontact-delete.md) | Nenhum |Exclua objeto orgContact. |
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|Coleção de cadeias de caracteres| Verifique se a associação ao grupo. |
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|Coleção de cadeias de caracteres| Retorne todos os grupos que o contato especificado é um membro de. |
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|Coleção de cadeias de caracteres| Retorna uma lista de directoryObjects de que o contato é um membro. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| endereços                    | [physicalOfficeAddress](physicalofficeaddress.md)            | Endereços postais para esse contato organizacional. Por enquanto um contato só pode ter um endereço físico. |
| companyName                  | String                                                    | Nome da empresa que este contato organizacional pertencem.                                                                                                                                                                                                                                                                                                                 |
| departamento                   | String                                                     | O nome para o departamento no qual o contato funciona.                                                                                                                                                                                                                                                                                                                                |
| displayName                  | String                                                     | Nome de exibição para esse contato organizacional.                                                                                                                                                                                                                                                                                                                                   |
| givenName                    | String                                                     | Nome para esse contato organizacional.                                                                                                                                                                                                                                                                                                                                     |
| id                           | String                                                     | Identificador exclusivo para esse contato organizacional.                                                                                                                                                                                                                                                                                                                             |
| imAddresses                  | String collection                          | Lista de endereços de mensagens Instantâneas para esse contato organizacional. Por enquanto um contato só pode ter um endereço SIP.                                                                                                                                                                                                                        |
| jobTitle                     | String                                                     | Cargo para esse contato organizacional.                                                                                                                                                                                                                                                                                                                                      |
|Email|String| O endereço SMTP do contato, por exemplo, "jeff@contoso.onmicrosoft.com". |
| mailNickname                 | String                                                     | Alias de email (parte do endereço de email previamente pendente o símbolo @) para esse contato organizacional.                                                                                                                                                                                                                                                                                |
| onPremisesLastSyncDateTime   | DateTimeOffset                                             | Data e hora quando este contato organizacional foi último sincronizados a partir do AD local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de Jan de 2014 ficaria assim: ' 2014-01-01T00:00:00Z'.   |
| onPremisesProvisioningErrors |coleção [onPremisesProvisioningError](onpremisesprovisioningerror.md)       | Lista de sincronização de provisionamento de erros para esse contato organizacional.                                                                                                                                                                                                                                                                                                |
|onPremisesSyncEnabled|Boolean|**true** se este objeto é sincronizado a partir de um diretório local; **false** se este objeto foi originalmente sincronizados a partir de um diretório local, mas é não são mais sincronizados e agora são administrados no Exchange; **Nulo** se este objeto nunca foram sincronizado a partir de um diretório local (padrão).|
| telefones                       | Coleção [phone](phone.md)                            | Lista de telefones para esse contato organizacional. Tipos de telefone podem ser businessFax, comercial e celular. Somente um de cada tipo nunca pode estar presente na coleção.                                                                                                                       |
| proxyAddresses               | Coleção de cadeias de caracteres                                         | Por exemplo: ["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]. Operador **any** é necessário para expressões de filtro propriedades de valores múltiplos. Suporta \$filtro.                                                                                                                                                                               |
| surname                      | String                                                     | Sobrenome para esse contato organizacional.                          |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|directReports|Coleção [directoryObject](directoryobject.md)| Relatórios de diretos do contato. (Os usuários e contatos que tenham sua propriedade manager definida para esse contato.)  Somente leitura. Anulável.|
|manager|[directoryObject](directoryobject.md)| O usuário ou contato que é gerente do contato. Somente leitura.|
|memberOf|Coleção [directoryObject](directoryobject.md)| Grupos que este contato é um membro de. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->