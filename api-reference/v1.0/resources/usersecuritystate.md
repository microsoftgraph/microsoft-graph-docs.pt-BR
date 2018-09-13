# <a name="usersecuritystate-resource-type"></a>tipo de recurso de userSecurityState

Contém informações com estado sobre a conta de usuário.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|aadUserId|Cadeia de caracteres|Identificador de Objeto do Usuário AAD (GUID) - representa a entidade de usuário física/de várias contas.|
|accountName|Cadeia de caracteres|Nome da conta de usuário (sem o domínio do Active Directory ou domínio DNS) - conta (também chamado de `mailNickName`).|
|domainName|Cadeia de caracteres|Domínio NetBIOS/Active Directory da conta de usuário (ou seja, no formato domínio\conta).|
|emailRole|emailRole|Para alertas relacionados a e-mail - 'função' do e-mail da conta do usuário. Os valores possíveis são: `unknown`, `sender`, `recipient`.|
|isVpn|Booleano|Indica se o usuário efetuou logon por meio de uma VPN.|
|logonDateTime|DateTimeOffset|Hora em que o login ocorreu. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|identificação de logon|Cadeia de caracteres|ID de login do usuário.|
|logonIp|Cadeia de caracteres|Endereço IP onde foi originada a solicitação de login.|
|logonLocation|Cadeia de caracteres|Local (por um mapeamento de endereço IP) associado a um evento de entrada do usuário por esse usuário.|
|logonType|logonType|Método de login do usuário. Os valores possíveis são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|
|onPremisesSecurityIdentifier|Sequência de caracteres|Identificador de segurança (SID) do Active Directory (no local) do usuário.|
|riskScore|Cadeia de caracteres|Pontuação de risco calculada/gerada pelo provedor da conta do usuário. Intervalo de valor recomendado de 0-1, que equivale a um percentual.|
|userAccountType|userAccountSecurityType|Tipo de conta de usuário (membros do grupo), por definição do Windows. Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.|
|userPrincipalName|Cadeia de caracteres|Nome de login do usuário - formato da internet: (nome da conta de usuário)@(nome de domínio DNS da conta de usuário).|

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
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
