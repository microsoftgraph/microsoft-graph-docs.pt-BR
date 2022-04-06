---
title: tipo de recurso de domínio
doc_type: resourcePageType
description: Fornece detalhes sobre a atividade de login de usuário ou de aplicativo em seu diretório.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
ms.openlocfilehash: 2f5b27d0b0a128896f4c575796514373b506bc55
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672179"
---
# <a name="signin-resource-type"></a>tipo de recurso de domínio

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece detalhes sobre a atividade de login de usuário ou de aplicativo em seu diretório. Você deve ter uma licença Azure AD Premium P1 ou P2 para baixar logs de login usando a API Graph Microsoft.

A disponibilidade de logs de login é governada pelas políticas de retenção de dados do [Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar entrar](../api/signin-list.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de objetos de domínio.|
|[Obter entrar](../api/signin-get.md) | [signIn](signin.md) |Ler propriedades e relações de um objeto signIn.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appDisplayName|String|O nome do aplicativo exibido no Portal do Azure. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|appId|String|O identificador de aplicativo no Azure Active Directory. Suporta `$filter` (`eq` somente operador).|
|appliedConditionalAccessPolicies|[coleção appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)|Uma lista de políticas de acesso condicional que são disparadas pela atividade de entrada correspondente.|
|authenticationContextClassReferences|[Coleção authenticationContext](authenticationcontext.md)|Contém uma coleção de valores que representam os contextos de autenticação de acesso condicional aplicados à entrada.|
|authenticationDetails|[Coleção authenticationDetail](authenticationdetail.md)|O resultado da tentativa de autenticação e detalhes adicionais sobre o método de autenticação.|
|authenticationMethodsUsed|Coleção de cadeias de caracteres|Os métodos de autenticação usados. Valores possíveis: `SMS`, `Authenticator App`, `App Verification code`, `Password`, `FIDO`, `PTA`, ou `PHS`.|
|authenticationProcessingDetails|Coleção [KeyValue](keyvalue.md)|Detalhes adicionais de processamento de autenticação, como o nome do agente em caso de PTA/PHS ou nome de servidor/farm em caso de autenticação federada.|
|authenticationProtocol|protocolType|Lista o tipo de protocolo ou tipo de concessão usado na autenticação. Os valores possíveis são `none`, `oAuth2`, `ropc`, `wsFederation`, `saml20`, `deviceCode`, `unknownFutureValue`. Para autenticações que usam protocolos diferentes dos valores possíveis listados, o tipo de protocolo é listado como `none`. |
|authenticationRequirement | String | Isso mantém o nível mais alto de autenticação necessário por meio de todas as etapas de login, para que a assinatura seja bem-sucedida. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|authenticationRequirementPolicies|[Coleção authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md)|Fontes de requisitos de autenticação, como acesso condicional, MFA por usuário, proteção de identidade e padrões de segurança.|
|autonomousSystemNumber|Int32|O Número do Sistema Autônomo (ASN) da rede usada pelo ator.|
|azureResourceId|String|Contém uma ID do Gerenciador de Recursos do Azure totalmente qualificado de um recurso do Azure acessado durante a assinatura.|
|clientAppUsed|Cadeia de caracteres|O cliente herddo usado para atividades de entrada. Por exemplo: `Browser`, `Exchange ActiveSync`, `Modern clients`, , `MAPI``IMAP`, `SMTP`, ou `POP`. Suporta `$filter` (`eq` somente operador). |
|conditionalAccessStatus|conditionalAccessStatus| O status da política de acesso condicional disparada. Valores possíveis: `success`, `failure`, `notApplied`ou `unknownFutureValue`. Suporta `$filter` (`eq` somente operador).|
|correlationId|Cadeia de caracteres|O identificador enviado do cliente quando a entrada é iniciada. Isso é usado para solucionar problemas da atividade de login correspondente ao chamar o suporte. Suporta `$filter` (`eq` somente operador).|
|createdDateTime|DateTimeOffset|A data e a hora em que a assinatura foi iniciada. O tipo de Timestamp é sempre UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Suporta `$orderby` e `$filter` (`eq`, `le`e somente `ge` operadores).|
|crossTenantAccessType|signInAccessType|Descreve o tipo de acesso entre locatários usado pelo ator para acessar o recurso. Os possíveis valores são: `none`, `b2bCollaboration`, `b2bDirectConnect`, `microsoftSupport`, `serviceProvider`, `unknownFutureValue`. Se a assinatura não cruzar os limites do locatário, o valor será `none`.|
|deviceDetail|[deviceDetail](devicedetail.md)|As informações do dispositivo de onde ocorreu a entrada. Inclui informações como deviceId, so e navegador. Oferece `$filter` suporte (`eq` e `startsWith` somente operadores) nas **propriedades browser** e **operatingSystem** .|
|federatedCredentialId|String|Contém o identificador da credencial de identidade federada de um aplicativo, se uma credencial de identidade federada foi usada para entrar.|
|flaggedForReview|Booliano|Durante uma falha na entrada, um usuário pode clicar em um botão no portal do Azure para marcar o evento com falha para administradores de locatários. Se um usuário clicou no botão para sinalizar a falha de login, esse valor será `true`.|
|homeTenantId|String|O identificador de locatário do usuário que inicia a login. Não aplicável em Identidades Gerenciadas ou em logins da entidade de serviço.|
|homeTenantName|String|Para entrar no usuário, o identificador do locatário de que o usuário é membro. Somente populado em casos em que o locatário da residência forneceu consentimento afirmativo ao Azure AD para mostrar o conteúdo do locatário.|
|id|String|O identificador que representa a atividade de login. Herdado da [entidade](entity.md). Suporta `$filter` (`eq` somente operador).|
|incomingTokenType|incomingTokenType|Indica os tipos de token que foram apresentados ao Azure AD para autenticar o ator na assinatura. Os valores possíveis são: `none`, `primaryRefreshToken`, `saml11`, `saml20`, `unknownFutureValue`. <br><br> **OBSERVAÇÃO** O Azure AD também pode ter usado tipos de token não listados neste tipo de Enumeração para autenticar o ator. Não infera a falta de um token se não for um dos tipos listados. |
|ipAddress|Cadeia de caracteres|O endereço IP do cliente de onde ocorreu a entrada. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|ipAddressFromResourceProvider|String|O endereço IP usado por um usuário para alcançar um provedor de recursos, usado para determinar a conformidade de Acesso Condicional para algumas políticas. Por exemplo, quando um usuário interage com Exchange Online, o endereço IP Exchange recebe do usuário pode ser gravado aqui. Esse valor costuma ser `null`.|
|isInteractive|Booliano|Indica se um usuário entrar é interativo. No login interativo, o usuário fornece um fator de autenticação para o Azure AD. Esses fatores incluem senhas, respostas a desafios de MFA, fatores biométricos ou códigos de QR que um usuário fornece ao Azure AD ou a um aplicativo associado. No login não interativo, o usuário não fornece um fator de autenticação. Em vez disso, o aplicativo cliente usa um token ou código para autenticar ou acessar um recurso em nome de um usuário. As entrada não interativas são comumente usadas para um cliente entrar em nome de um usuário em um processo transparente para o usuário.|
|isTenantRestricted|Booliano|Mostra se o evento de entrar estava sujeito a uma política de restrição de locatário do Azure AD.|
|location|[signInLocation](signinlocation.md)|A cidade, o estado e o código de país de duas letras de onde ocorreu a login. Oferece `$filter` suporte (`eq` e `startsWith` somente operadores) em **propriedades city**, **state** e **countryOrRegion** .|
|networkLocationDetails|coleção [networkLocationDetail](networklocationdetail.md)|Os detalhes do local da rede, incluindo o tipo de rede usada e seus nomes.|
|originalRequestId|Cadeia de caracteres|O identificador de solicitação da primeira solicitação na sequência de autenticação. Suporta `$filter` (`eq` somente operador).|
|privateLinkDetails|[privateLinkDetails](../resources/privatelinkdetails.md)|Contém informações sobre a política de Link Privado do Azure AD associada ao evento de login.|
|processingTimeInMilliseconds|Int|O tempo de processamento da solicitação em milissegundos no AD STS.|
|resourceDisplayName|String|O nome do recurso ao que o usuário se inscreveu. Suporta `$filter` (`eq` somente operador).|
|resourceId|Cadeia de caracteres|O identificador do recurso ao que o usuário se inscreveu. Suporta `$filter` (`eq` somente operador).|
|resourceServicePrincipalId|String|O identificador da entidade de serviço que representa o recurso de destino no evento de entrada.|
|resourceTenantId|String|O identificador de locatário do recurso referenciado na assinatura.|
|riskDetail|riskDetail|O motivo por trás de um estado específico de um usuário arriscado, de entrar ou de um evento de risco. Valores possíveis: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, , `adminConfirmedSigninCompromised`ou `unknownFutureValue`. O valor `none` significa que nenhuma ação foi realizada pelo usuário ou entrar até o momento. Suporta `$filter` (`eq` somente operador).<br> **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden`.|
|riskEventTypes_v2|Coleção de cadeias de caracteres|A lista de tipos de eventos de risco associados à assinatura. Valores possíveis: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, ,  `generic`ou `unknownFutureValue`. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|riskLevelAggregated|riskLevel|O nível de risco agregado. Valores possíveis: `none`, `low`, `medium`, `high`, `hidden`ou `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. Suporta `$filter` (`eq` somente operador). <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden`.|
|riskLevelDuringSignIn|riskLevel|O nível de risco durante a assinatura. Valores possíveis: `none`, `low`, `medium`, `high`, `hidden`ou `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. Suporta `$filter` (`eq` somente operador). <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden`.|
|riskState|riskState|O estado de risco de um usuário arriscado, de entrar ou de um evento de risco. Valores possíveis: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, ou `unknownFutureValue`. Suporta `$filter` (`eq` somente operador).|
|servicePrincipalCredentialKeyId|String|O identificador exclusivo da credencial de chave usada pela entidade de serviço para autenticar.|
|servicePrincipalCredentialThumbprint|String|A impressão digital do certificado usado pela entidade de serviço para autenticação.|
|servicePrincipalId|String|O identificador de aplicativo usado para entrar. Esse campo é preenchido quando você está fazendo o registro usando um aplicativo. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|servicePrincipalName|Cadeia de caracteres|O nome do aplicativo usado para entrar. Esse campo é preenchido quando você está fazendo o registro usando um aplicativo. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|sessionLifetimePolicies|[Coleção sessionLifetimePolicy](sessionlifetimepolicy.md)|Quaisquer políticas de gerenciamento de sessão de acesso condicional que foram aplicadas durante o evento de entrada.|
|signInEventTypes|Coleção de cadeias de caracteres|Indica a categoria de sign in que o evento representa. Para entrar no usuário, a categoria pode ser `interactiveUser` `nonInteractiveUser` ou corresponde ao valor da **propriedade isInteractive** no recurso de signin. Para as insições de identidade gerenciada, a categoria é `managedIdentity`. Para as insições da entidade de serviço, a categoria **é servicePrincipal**. Os valores possíveis são: `interactiveUser`, `nonInteractiveUser`, `servicePrincipal`, `managedIdentity`, `unknownFutureValue`. Suporta `$filter` (`eq`, `ne`).|
|signInIdentifier|String|A identificação que o usuário forneceu para entrar. Pode ser o userPrincipalName, mas também é preenchido quando um usuário entra usando outros identificadores.|
|signInIdentifierType|signInIdentifierType|O tipo de identificador de login. Os possíveis valores são: `userPrincipalName`, `phoneNumber`, `proxyAddress`, `qrCode`, `onPremisesUserPrincipalName`, `unknownFutureValue`.|
|status|[signInStatus](signinstatus.md)|O status de login. Inclui o código de erro e a descrição do erro (no caso de uma falha de login). Suporta `$filter` (`eq` somente operador) na **propriedade errorCode** .|
|tokenIssuerName|Cadeia de caracteres|O nome do provedor de identidade. Por exemplo, `sts.microsoft.com`. Suporta `$filter` (`eq` somente operador).|
|tokenIssuerType|tokenIssuerType|O tipo de provedor de identidade. Os valores possíveis são: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`, `AzureADBackupAuth`, `ADFederationServicesMFAAdapter`, `NPSExtension`. Observe que você deve usar o `Prefer: include-unknown-enum-members` header de solicitação para obter os seguintes valores nesta [enum evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `AzureADBackupAuth` , `ADFederationServicesMFAAdapter` , `NPSExtension`.|
|uniqueTokenIdentifier|String|Um identificador de solicitação codificado de base64 exclusivo usado para rastrear tokens emitidos pelo Azure AD à medida que são resgatados em provedores de recursos. |
|userAgent|String|As informações do agente do usuário relacionadas à login. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|userDisplayName|Cadeia de caracteres|O nome de exibição do usuário. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|userId|Cadeia de caracteres|O identificador do usuário. Suporta `$filter` (`eq` somente operador).|
|userPrincipalName|String|O UPN do usuário. Oferece suporte `$filter` (`eq` e `startsWith` somente operadores).|
|userType|signInUserType|Identifica se o usuário é membro ou convidado no locatário. Os valores possíveis são: `member`, `guest`, `unknownFutureValue`.|
|mfaDetail (preterido)|String|Essa propriedade é preterida.|


## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.signIn",
  "openType": false
}
-->
```json
{
  "@odata.type": "#microsoft.graph.signIn",
  "appDisplayName": "String",
  "appId": "String",
  "authenticationContextClassReferences": [{"@odata.type": "microsoft.graph.authenticationContext"}],
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "microsoft.graph.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "authenticationRequirement": "String",
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
    }
  ],
  "autonomousSystemNumber": "Integer",
  "azureResourceId": "String",
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "crossTenantAccessType": "String",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "federatedCredentialId": "String",
  "flaggedForReview": "Boolean",
  "id": "String (identifier)",
  "homeTenantId": "String",
  "homeTenantName": "String",
  "isInteractive": "Boolean",
  "isTenantRestricted": "Boolean",
  "ipAddress": "String",
  "ipAddressFromResourceProvider": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail"
    }
  ],
  "originalRequestId": "String",
  "privateLinkDetails": {
    "@odata.type": "microsoft.graph.privateLinkDetails"
  },
  "processingTimeInMilliseconds": "Integer",
  "riskDetail": "String",
  "riskEventTypes": [
    "String"
  ],
  "riskEventTypes_v2": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "String",
  "resourceId": "String",
  "resourceTenantId": "String",
  "servicePrincipalCredentialKeyId": "String",
  "servicePrincipalCredentialThumbprint": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "sessionLifetimePolicies": [{"@odata.type": "microsoft.graph.sessionLifetimePolicy"}],
  "signInEventTypes": [
    "String"
  ],
  "signInIdentifier": "String",
  "signInIdentifierType": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
