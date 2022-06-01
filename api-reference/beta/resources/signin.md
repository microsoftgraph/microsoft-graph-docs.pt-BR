---
title: tipo de recurso de domínio
doc_type: resourcePageType
description: Fornece detalhes sobre a atividade de login de usuário ou de aplicativo em seu diretório.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
ms.openlocfilehash: ba1100b738c2904c6661e52df62171a11aa4dda3
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819346"
---
# <a name="signin-resource-type"></a>tipo de recurso de domínio

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece detalhes sobre a atividade de login de usuário ou de aplicativo em seu diretório. Você deve ter uma Azure AD Premium P1 ou P2 para baixar os logs de entrada usando o Microsoft API do Graph.

A disponibilidade de logs de entrada é regida pelas políticas [de retenção Azure AD dados.](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar entrar](../api/signin-list.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de objetos de domínio.|
|[Obter entrar](../api/signin-get.md) | [signIn](signin.md) |Ler propriedades e relações de um objeto signIn.|
|[Confirmar comprometimento](../api/signin-confirmcompromised.md)|Nenhum|Marque um evento no Azure AD logs de entrada como arriscados.|
|[Confirmar seguro](../api/signin-confirmsafe.md)|Nenhum|marcar um evento em Azure AD logs de entrada como seguros.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appDisplayName|Cadeia de caracteres|O nome do aplicativo exibido no Portal do Azure. Dá `$filter` suporte (`eq` e somente `startsWith` operadores).|
|appId|String|O identificador do aplicativo Azure Active Directory. Dá suporte `$filter` (`eq` somente operador).|
|appliedConditionalAccessPolicies|[Coleção appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)|Uma lista de políticas de acesso condicional que são disparadas pela atividade de entrada correspondente.|
|authenticationContextClassReferences|[coleção authenticationContext](authenticationcontext.md)|Contém uma coleção de valores que representam os contextos de autenticação de acesso condicional aplicados à entrada.|
|authenticationDetails|[coleção authenticationDetail](authenticationdetail.md)|O resultado da tentativa de autenticação e detalhes adicionais sobre o método de autenticação.|
|authenticationMethodsUsed|Coleção de cadeias de caracteres|Os métodos de autenticação usados. Valores possíveis: `SMS`, `Authenticator App`, `App Verification code`, `Password`, `FIDO`, `PTA`ou `PHS`.|
|authenticationProcessingDetails|Coleção [KeyValue](keyvalue.md)|Detalhes adicionais de processamento de autenticação, como o nome do agente no caso de PTA/PHS ou nome de servidor/farm no caso de autenticação federada.|
|authenticationProtocol|Protocoltype|Lista o tipo de protocolo ou tipo de concessão usado na autenticação. Os valores possíveis são `none`, `oAuth2`, `ropc`, `wsFederation`, `saml20`, `deviceCode`, `unknownFutureValue`. Para autenticações que usam protocolos diferentes dos valores possíveis listados, o tipo de protocolo é listado como `none`. |
|authenticationRequirement | Cadeia de caracteres | Isso mantém o nível mais alto de autenticação necessário por meio de todas as etapas de entrada para que a entrada seja bem-sucedida. Dá `$filter` suporte (`eq` e somente `startsWith` operadores).|
|authenticationRequirementPolicies|[coleção authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md)|Fontes de requisito de autenticação, como acesso condicional, MFA por usuário, proteção de identidade e padrões de segurança.|
|autonomousSystemNumber|Int32|O ASN (Número do Sistema Autônomo) da rede usada pelo ator.|
|azureResourceId|Cadeia de caracteres|Contém uma ID totalmente qualificada do Azure Resource Manager de um recurso do Azure acessado durante a entrada.|
|clientAppUsed|Cadeia de caracteres|O cliente herdado usado para a atividade de entrada. Por exemplo: `Browser`, `Exchange ActiveSync`, `Modern clients`, , `IMAP`, `MAPI`, `SMTP`ou `POP`. Dá suporte `$filter` (`eq` somente operador). |
|Clientcredentialtype|Clientcredentialtype|Descreve o tipo de credencial que um cliente de usuário ou entidade de serviço forneceu para Azure AD autenticar a si mesmo. Talvez você queira examinar clientCredentialType para controlar e eliminar tipos de credenciais menos seguros ou observar clientes e entidades de serviço usando tipos de credenciais anômalos. Os valores possíveis são `none`, `clientSecret`, `clientAssertion`, `federatedIdentityCredential`, `managedIdentity`, `certificate`, `unknownFutureValue`.|
|conditionalAccessStatus|conditionalAccessStatus| O status da política de acesso condicional disparada. Valores possíveis: `success`, `failure`, `notApplied`ou `unknownFutureValue`. Dá suporte `$filter` (`eq` somente operador).|
|correlationId|Cadeia de caracteres|O identificador que é enviado do cliente quando a entrada é iniciada. Isso é usado para solucionar problemas da atividade de entrada correspondente ao chamar o suporte. Dá suporte `$filter` (`eq` somente operador).|
|createdDateTime|DateTimeOffset|A data e a hora em que a entrada foi iniciada. O tipo de Timestamp é sempre UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Dá `$orderby` suporte `$filter` e (`eq`, `le`e somente operadores `ge` ).|
|crossTenantAccessType|signInAccessType|Descreve o tipo de acesso entre locatários usado pelo ator para acessar o recurso. Os possíveis valores são: `none`, `b2bCollaboration`, `b2bDirectConnect`, `microsoftSupport`, `serviceProvider`, `unknownFutureValue`. Se a entrada não cruzar os limites do locatário, o valor será `none`.|
|deviceDetail|[deviceDetail](devicedetail.md)|As informações do dispositivo de onde ocorreu a entrada. Inclui informações como deviceId, so e navegador. Dá `$filter` suporte (`eq` e `startsWith` somente operadores) nas **propriedades do navegador** **e do operatingSystem** .|
|federatedCredentialId|Cadeia de caracteres|Contém o identificador da credencial de identidade federada de um aplicativo, se uma credencial de identidade federada foi usada para entrar.|
|flaggedForReview|Booliano|Durante uma entrada com falha, um usuário pode clicar em um botão no portal do Azure para marcar o evento com falha para administradores de locatários. Se um usuário clicou no botão para sinalizar a entrada com falha, esse valor será `true`.|
|homeTenantId|Cadeia de caracteres|O identificador de locatário do usuário que inicia a entrada. Não aplicável em identidades gerenciadas ou entradas de entidade de serviço.|
|homeTenantName|String|Para entradas de usuário, o identificador do locatário do qual o usuário é membro. Populado somente em casos em que o locatário inicial forneceu consentimento afirmativo Azure AD mostrar o conteúdo do locatário.|
|id|Cadeia de caracteres|O identificador que representa a atividade de entrada. Herdado da [entidade](entity.md). Dá suporte `$filter` (`eq` somente operador).|
|incomingTokenType|incomingTokenType|Indica os tipos de token que foram apresentados Azure AD autenticar o ator na entrada. Os valores possíveis são: `none`, `primaryRefreshToken`, `saml11`, `saml20`, `unknownFutureValue`, `remoteDesktopToken`. <br><br> **OBSERVE** Azure AD também pode ter usado tipos de token não listados neste tipo Enum para autenticar o ator. Não infera a falta de um token se ele não for um dos tipos listados. Além disso, observe que você deve usar `Prefer: include-unknown-enum-members` o cabeçalho da solicitação para obter os seguintes valores nesta [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `remoteDesktopToken`.|
|ipAddress|Cadeia de caracteres|O endereço IP do cliente de onde ocorreu a entrada. Dá `$filter` suporte (`eq` e somente `startsWith` operadores).|
|ipAddressFromResourceProvider|Cadeia de caracteres|O endereço IP que um usuário usou para acessar um provedor de recursos, usado para determinar a conformidade de Acesso Condicional para algumas políticas. Por exemplo, quando um usuário interage com Exchange Online, o endereço IP Exchange recebe do usuário pode ser registrado aqui. Esse valor geralmente é `null`.|
|isInteractive|Booliano|Indica se uma entrada do usuário é interativa. Na entrada interativa, o usuário fornece um fator de autenticação para Azure AD. Esses fatores incluem senhas, respostas a desafios de MFA, fatores biométricos ou códigos QR que um usuário fornece para Azure AD ou um aplicativo associado. Na entrada não interativa, o usuário não fornece um fator de autenticação. Em vez disso, o aplicativo cliente usa um token ou código para autenticar ou acessar um recurso em nome de um usuário. As entradas não interativas são comumente usadas para um cliente entrar em nome de um usuário em um processo transparente para o usuário.|
|isTenantRestricted|Booliano|Mostra se o evento de entrada estava sujeito a uma política Azure AD restrição de locatário.|
|location|[signInLocation](signinlocation.md)|A cidade, o estado e o código do país de duas letras de onde a entrada ocorreu. Dá `$filter` suporte (`eq` e `startsWith` somente operadores) **nas propriedades city**, **state** e **countryOrRegion** .|
|networkLocationDetails|coleção [networkLocationDetail](networklocationdetail.md)|Os detalhes do local de rede, incluindo o tipo de rede usada e seus nomes.|
|originalRequestId|Cadeia de caracteres|O identificador de solicitação da primeira solicitação na sequência de autenticação. Dá suporte `$filter` (`eq` somente operador).|
|privateLinkDetails|[privateLinkDetails](../resources/privatelinkdetails.md)|Contém informações sobre a Azure AD Link Privado que está associada ao evento de entrada.|
|processingTimeInMilliseconds|Int|O tempo de processamento da solicitação em milissegundos no AD STS.|
|resourceDisplayName|Cadeia de caracteres|O nome do recurso ao qual o usuário entrou. Dá suporte `$filter` (`eq` somente operador).|
|resourceId|Cadeia de caracteres|O identificador do recurso ao qual o usuário entrou. Dá suporte `$filter` (`eq` somente operador).|
|resourceServicePrincipalId|Cadeia de caracteres|O identificador da entidade de serviço que representa o recurso de destino no evento de entrada.|
|resourceTenantId|Cadeia de caracteres|O identificador de locatário do recurso referenciado na entrada.|
|riskDetail|riskDetail|O motivo por trás de um estado específico de um usuário arriscado, entrada ou um evento de risco. Valores possíveis: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, , `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`ou `unknownFutureValue`. O valor `none` significa que nenhuma ação foi realizada pelo usuário ou entrar até o momento. Dá suporte `$filter` (`eq` somente operador).<br> **Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden`.|
|riskEventTypes_v2|Coleção de cadeias de caracteres|A lista de tipos de evento de risco associados à entrada. Valores possíveis: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, , `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`ou `unknownFutureValue`. Dá `$filter` suporte (`eq` e somente `startsWith` operadores).|
|riskLevelAggregated|riskLevel|O nível de risco agregado. Valores possíveis: `none`, `low`, `medium`, `high`, `hidden`ou `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. Dá suporte `$filter` (`eq` somente operador). <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden`.|
|riskLevelDuringSignIn|riskLevel|O nível de risco durante a entrada. Valores possíveis: `none`, `low`, `medium`, `high`, `hidden`ou `unknownFutureValue`. O valor `hidden` significa que o usuário ou entrada não foi habilitado para proteção de identidade do Azure AD. Dá suporte `$filter` (`eq` somente operador). <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Todos os outros clientes são retornados `hidden`.|
|riskState|riskState|O estado de risco de um usuário arriscado, entrada ou evento de risco. Valores possíveis: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`ou `unknownFutureValue`. Dá suporte `$filter` (`eq` somente operador).|
|servicePrincipalCredentialKeyId|Cadeia de caracteres|O identificador exclusivo da credencial de chave usada pela entidade de serviço a ser autenticada.|
|servicePrincipalCredentialThumbprint|Cadeia de caracteres|A impressão digital do certificado usado pela entidade de serviço para autenticar.|
|servicePrincipalId|Cadeia de caracteres|O identificador de aplicativo usado para entrar. Esse campo é preenchido quando você está entrando usando um aplicativo. Dá `$filter` suporte (`eq` e somente `startsWith` operadores).|
|servicePrincipalName|Cadeia de caracteres|O nome do aplicativo usado para entrar. Esse campo é preenchido quando você está entrando usando um aplicativo. Dá `$filter` suporte (`eq` e somente `startsWith` operadores).|
|sessionLifetimePolicies|[coleção sessionLifetimePolicy](sessionlifetimepolicy.md)|Todas as políticas de gerenciamento de sessão de acesso condicional que foram aplicadas durante o evento de entrada.|
|signInEventTypes|Coleção de cadeias de caracteres|Indica a categoria de entrada que o evento representa. Para entradas de usuário, a categoria pode ser `interactiveUser` `nonInteractiveUser` ou corresponde ao valor da propriedade **isInteractive** no recurso de entrada. Para entradas de identidade gerenciada, a categoria é `managedIdentity`. Para entradas da entidade de serviço, a categoria é **servicePrincipal**. Os valores possíveis são: `interactiveUser`, `nonInteractiveUser`, `servicePrincipal`, `managedIdentity`, `unknownFutureValue`. Suporta `$filter` (`eq`, `ne`).|
|signInIdentifier|String|A identificação que o usuário forneceu para entrar. Pode ser o userPrincipalName, mas também é preenchido quando um usuário entra usando outros identificadores.|
|signInIdentifierType|signInIdentifierType|O tipo de identificador de entrada. Os possíveis valores são: `userPrincipalName`, `phoneNumber`, `proxyAddress`, `qrCode`, `onPremisesUserPrincipalName`, `unknownFutureValue`.|
|status|[signInStatus](signinstatus.md)|O status de entrada. Inclui o código de erro e a descrição do erro (no caso de uma falha de entrada). Dá `$filter` suporte (`eq` somente operador) à **propriedade errorCode** .|
|tokenIssuerName|Cadeia de caracteres|O nome do provedor de identidade. Por exemplo, `sts.microsoft.com`. Dá suporte `$filter` (`eq` somente operador).|
|tokenIssuerType|tokenIssuerType|O tipo de provedor de identidade. Os valores possíveis são: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`, `AzureADBackupAuth`, `ADFederationServicesMFAAdapter`, `NPSExtension`. Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores nesta [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `AzureADBackupAuth` , `ADFederationServicesMFAAdapter` , `NPSExtension`.|
|uniqueTokenIdentifier|Cadeia de caracteres|Um identificador de solicitação codificado em base64 exclusivo usado para rastrear tokens emitidos pelo Azure AD à medida que eles são resgatados em provedores de recursos. |
|Useragent|String|As informações do agente do usuário relacionadas à entrada. Dá `$filter` suporte (`eq` e somente `startsWith` operadores).|
|userDisplayName|Cadeia de caracteres|O nome de exibição do usuário. Dá `$filter` suporte (`eq` e somente `startsWith` operadores).|
|userId|Cadeia de caracteres|O identificador do usuário. Dá suporte `$filter` (`eq` somente operador).|
|userPrincipalName|Cadeia de caracteres|O UPN do usuário. Dá `$filter` suporte (`eq` e somente `startsWith` operadores).|
|userType|signInUserType|Identifica se o usuário é membro ou convidado no locatário. Os valores possíveis são: `member`, `guest`, `unknownFutureValue`.|
|mfaDetail (preterido)|String|Essa propriedade foi preterida.|


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
