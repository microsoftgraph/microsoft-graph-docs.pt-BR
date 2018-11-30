---
title: tipo de recurso de orgContact
description: Veja a seguir uma representação JSON do recurso
ms.openlocfilehash: fb0970b2eb973e516761ba1145d66b3af7fdef5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038652"
---
# <a name="orgcontact-resource-type"></a>tipo de recurso de orgContact

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "officeLocation": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "proxyAddresses": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|city|String| A cidade na qual o contato está localizado. |
|country|String| O país/região no qual o contato está localizado. |
|departamento|String| O nome para o departamento no qual o contato funciona. |
|onPremisesSyncEnabled|Booliano|**True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão).|
|displayName|String| O nome de exibição do contato. |
|givenName|String| O nome fornecido (primeiro nome) do contato. |
|jobTitle|String| Cargo do contato. |
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o objeto foi sincronizado com o diretório local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|onPremisesProvisioningErrors|coleção [onPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante o provisionamento. |
|Email|String| O endereço SMTP do contato, por exemplo, "jeff@contoso.onmicrosoft.com". |
|mailNickname|String| O alias de email do contato. |
|mobilePhone|String| O número de telefone principal de celular do contato. |
|id|String| O identificador exclusivo para o contato. Somente leitura.|
|officeLocation|String| O local do escritório no lugar do contato de negócios. |
|postalCode|String| O código postal do endereço postal do contato. O código postal é específico país/região do contato. Nos Estados Unidos, este atributo contém o CEP. |
|proxyAddresses|Coleção de cadeias de caracteres| Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` o operador **any** é necessário para expressões de filtro propriedades de valores múltiplos. Somente leitura. Não anulável. Oferece suporte a $filter. |
|state|String| O estado ou província no endereço do contato. |
|streetAddress|String| O endereço do local do contato de negócios. |
|surname|String| O sobrenome do contato (família nome ou sobrenome). |
|businessPhones|String| O número de telefone principal do local do contato de negócios. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|directReports|Coleção [directoryObject](directoryobject.md)| Relatórios de diretos do contato. (Os usuários e contatos que tenham sua propriedade manager definida para esse contato.)  Somente leitura. Anulável.|
|manager|[directoryObject](directoryobject.md)| O usuário ou contato que é gerente do contato. Somente leitura.|
|memberOf|Coleção [directoryObject](directoryobject.md)| Grupos que este contato é um membro de. Somente leitura. Anulável.|

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->