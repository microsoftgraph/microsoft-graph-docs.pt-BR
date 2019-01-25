---
title: tipo de recurso de userSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62a54a996d7fe9c892da797cee352a57d0782035
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517236"
---
# <a name="usersecuritystate-resource-type"></a>tipo de recurso de userSecurityState

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações com informações de estado sobre a conta de usuário.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|aadUserId|String|Usuário AAD objeto GUID (identificador) - representa a entidade de usuário físicos/multi-account.|
|accountName|String|Nome da conta de usuário (sem o domínio do Active Directory ou domínio DNS) - conta (também chamado de `mailNickName`).|
|domainName|Cadeia de caracteres|Domínio NetBIOS/Active Directory da conta de usuário (ou seja, o formato domínio \ conta).|
|emailRole|emailRole|Para alertas relacionados a email - o email de uma conta de usuário 'função'. Os valores possíveis são: `unknown`, `sender`, `recipient`.|
|isVpn|Booliano|Indica se o usuário conectado por meio da VPN.|
|logonDateTime|DateTimeOffset|Hora em que a entrar ocorreu. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|identificação de logon|String|ID de usuário entrar.|
|logonIp|String|Endereço IP que a solicitação de entrada se originou.|
|logonLocation|String|Local (por um mapeamento de endereço IP) associado a um evento de entrada do usuário por esse usuário.|
|logonType|logonType|Método do usuário entrar. Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|
|onPremisesSecurityIdentifier|String|Active Directory (no local) identificador de segurança (SID) do usuário.|
|riskScore|String|Pontuação de provedor gerado/calculado em risco da conta de usuário. Valor recomendado o intervalo de 0-1, que é igual a um percentual.|
|userAccountType|userAccountSecurityType|Tipo de conta de usuário (membros do grupo), por definição do Windows. Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.|
|userPrincipalName|String|Entrar nome de usuário - formato da internet: (nome de conta de usuário) @(nome de domínio do DNS de conta de usuário).|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/usersecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
