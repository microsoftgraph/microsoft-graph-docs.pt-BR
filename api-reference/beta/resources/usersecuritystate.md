---
title: Tipo de recurso userSecurityState
description: Contém informações de estado sobre a conta de usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c95f898a729138a7af88eaf25fa4cbc0c5fc9bb9
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761776"
---
# <a name="usersecuritystate-resource-type"></a>Tipo de recurso userSecurityState

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações de estado sobre a conta de usuário.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|aadUserId|Cadeia de Caracteres|Identificador de objeto do usuário AAD (GUID) - representa a entidade de usuário físico/de várias contas.|
|accountName|Cadeia de Caracteres|Nome da conta de usuário (sem domínio do Active Directory ou domínio DNS) - (também chamado `mailNickName` ).|
|domainName|Cadeia de caracteres|Domínio NetBIOS/Active Directory da conta de usuário (ou seja, formato de domínio\conta).|
|emailRole|emailRole|Para alertas relacionados a email - 'função' de email da conta de usuário. Os valores possíveis são: `unknown`, `sender`, `recipient`.|
|isVpn|Boolean|Indica se o usuário fez logons por meio de uma VPN.|
|logonDateTime|DateTimeOffset|Hora em que ocorreu a login. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|logonId|Cadeia de Caracteres|ID de login do usuário.|
|logonIp|Cadeia de Caracteres|Endereço IP da solicitação de login originada.|
|logonLocation|Cadeia de Caracteres|Local (por mapeamento de endereço IP) associado a um evento de login do usuário por esse usuário.|
|logonType|logonType|Método de login do usuário. Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|
|onPremisesSecurityIdentifier|String|Identificador de Segurança (SID) do Active Directory (local) do usuário.|
|riskScore|Cadeia de Caracteres|Pontuação de risco gerada/calculada pelo provedor da conta de usuário. Intervalo de valores recomendado de 0 a 1, que equivale a uma porcentagem.|
|userAccountType|userAccountSecurityType|Tipo de conta de usuário (associação ao grupo), por definição do Windows. Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.|
|userPrincipalName|Cadeia de caracteres|Nome de login do usuário - formato da Internet: (nome da conta de usuário)@(nome de domínio DNS da conta de usuário).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


