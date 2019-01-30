---
title: tipo de recurso de orgContact
description: Veja a seguir uma representação JSON do recurso
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01f606e8fb1f6ae51608853eed3bc39e0ec124df
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643528"
---
# <a name="orgcontact-resource-type"></a>tipo de recurso de orgContact

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| department                   | String                                                     | O nome para o departamento no qual o contato funciona.                                                                                                                                                                                                                                                                                                                                |
| displayName                  | String                                                     | Nome de exibição para esse contato organizacional.                                                                                                                                                                                                                                                                                                                                   |
| givenName                    | String                                                     | Nome para esse contato organizacional.                                                                                                                                                                                                                                                                                                                                     |
| id                           | String                                                     | Identificador exclusivo para esse contato organizacional.                                                                                                                                                                                                                                                                                                                             |
| imAddresses                  | Coleção de cadeias de caracteres                          | Lista de endereços de mensagens Instantâneas para esse contato organizacional. Por enquanto um contato só pode ter um endereço SIP.                                                                                                                                                                                                                        |
| jobTitle                     | String                                                     | Cargo para esse contato organizacional.                                                                                                                                                                                                                                                                                                                                      |
|email|String| O endereço SMTP do contato, por exemplo, "jeff@contoso.onmicrosoft.com". |
| mailNickname                 | String                                                     | Alias de email (parte do endereço de email previamente pendente o símbolo @) para esse contato organizacional.                                                                                                                                                                                                                                                                                |
| onPremisesLastSyncDateTime   | DateTimeOffset                                             | Data e hora quando este contato organizacional foi último sincronizados a partir do AD local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de Jan de 2014 ficaria assim: ' 2014-01-01T00:00:00Z'.   |
| onPremisesProvisioningErrors |coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md)       | Lista de sincronização de provisionamento de erros para esse contato organizacional.                                                                                                                                                                                                                                                                                                |
|onPremisesSyncEnabled|Booliano|**true** se este objeto é sincronizado a partir de um diretório local; **false** se este objeto foi originalmente sincronizados a partir de um diretório local, mas é não são mais sincronizados e agora são administrados no Exchange; **Nulo** se este objeto nunca foram sincronizado a partir de um diretório local (padrão).|
| telefones                       | Coleção [phone](phone.md)                            | Lista de telefones para esse contato organizacional. Tipos de telefone podem ser businessFax, comercial e celular. Somente um de cada tipo nunca pode estar presente na coleção.                                                                                                                       |
| proxyAddresses               | Coleção de cadeias de caracteres                                         | Por exemplo: ["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]. O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. Suporta \$filtro.                                                                                                                                                                               |
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
<!--
{
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/orgcontact.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
