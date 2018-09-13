# <a name="alert-resource-type"></a>tipo de recurso alert

Representa possíveis problemas de segurança no locatário de um cliente identificado pela Microsoft ou por soluções de segurança de parceiros. Use alertas para unificar e simplificar o gerenciamento de problemas de segurança em todas as soluções integradas. |||UNTRANSLATED_CONTENT_START|||To learn more, see the sample queries in [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer).|||UNTRANSLATED_CONTENT_END|||

Alertas podem ser recuperados dos seguintes provedores: Central de Segurança do Azure e Azure Active Directory Identity Protection. Outros provedores de alertas se integrarão nos próximos meses.

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Get alert](../api/alert_get.md) | [alerta](alert.md) |Ler propriedades e relações de um objeto de alerta.|
|[Atualizar alertas](../api/alert_update.md) | [alerta](alert.md) |Atualize um objeto de alerta. |
|[Listar alertas](../api/alert_list.md) | coleção [alert](alert.md) |Obtém uma coleção de objetos alert.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|activityGroupName|Cadeia de caracteres|Nome ou alias do grupo ativista (atacante) a que este alerta é atribuído.|
|assignedTo|Cadeia de caracteres|Nome do analista ao qual o alerta está atribuído para triagem, investigação ou correção (oferece suporte a [atualização](../api/alert_update.md)).|
|azureSubscriptionId|Cadeia de caracteres|ID de assinatura do Azure, presente se esse alerta estiver relacionado a um recurso do Azure.|
|azureTenantId *|Cadeia de caracteres|ID do locatário do Active Directory do Azure.|
|Ferramentas para desenvolvedores|Cadeia de caracteres|Categoria do alerta (por exemplo, credentialTheft, ransomware, etc.).|
|closedDateTime|DateTimeOffset|Hora em que o alerta foi fechado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de Jan de 2014 ficaria assim: `'2014-01-01T00:00:00Z'` (oferece suporte a [atualização](../api/alert_update.md)).|
|cloudAppStates|coleção [cloudAppSecurityState](cloudappsecuritystate.md)|Informações com estado relacionadas à segurança geradas pelo provedor sobre os aplicativos de nuvem relacionados a esse alerta.|
|comentários|Coleção de cadeias de caracteres|Comentários fornecidos pelo cliente sobre o alerta (para gerenciamento de alerta ao cliente) (oferece suporte a [atualização](../api/alert_update.md)).|
|confidence|Int32|Confiança da lógica de detecção (percentual entre 1-100).|
|createdDateTime *|DateTimeOffset|Hora em que o alerta foi criado pelo provedor de alerta. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de Jan de 2014 ficaria assim: `'2014-01-01T00:00:00Z'`.|
|descrição|Cadeia de caracteres|Descrição do alerta.|
|detectionIds|Coleção de cadeias de caracteres|Conjunto de alertas relacionados a essa entidade de alerta (cada alerta é enviado ao SIEM como um registro separado).|
|eventDateTime *|DateTimeOffset|Hora na qual os eventos que serviram como o gatilho para gerar o alerta ocorreram. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|feedback|alertFeedback|Feedback do analista no alerta. Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`. (oferece suporte a [atualização](../api/alert_update.md))|
|fileStates|coleção [fileSecurityState](filesecuritystate.md)|Informações de estado relacionadas à segurança geradas pelo provedor sobre os arquivos relacionados a este alerta.|
|hostStates|coleção [hostSecurityState](hostsecuritystate.md)|Informações com estado relacionadas à segurança geradas pelo provedor sobre os hosts relacionadas a este alerta.|
|id *|Cadeia de caracteres|GUID/identificador exclusivo gerado pelo provedor. (Somente leitura)|
|lastModifiedDateTime|DateTimeOffset|Hora em que a entidade de alerta foi modificada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|malwareStates|coleção [malwareState](malwarestate.md)|Inteligência de ameaças referente a malware relacionado a esse alerta.|
|networkConnections|coleção [networkConnection](networkconnection.md)|Informações de estado relacionadas à segurança geradas pelo provedor sobre as conexões de rede relacionadas a esse alerta.|
|processos|coleção [process](process.md)|Informações atualizadas relacionadas à segurança geradas pelo provedor sobre o processo ou processos relacionados a esse alerta.|
|recommendedActions|Coleção de cadeias de caracteres|Ações recomendadas do fornecedor/provedor a serem tomadas como resultado do alerta (por exemplo, isolar máquina, enforce2FA, reparar a imagem do host).|
|registryKeyStates|coleção [registryKeyState](registrykeystate.md)|Informações de estado relacionadas à segurança geradas pelo provedor sobre as chaves de registro relacionadas a esse alerta.|
|severity *|alertSeverity|Severidade de alerta - definida pelo fornecedor/provedor. Os valores possíveis são: `unknown`, `informational`, `low`, `medium`, `high`.|
|sourceMaterials|Coleção de cadeias de caracteres|Hiperlinks (URIs) para o material de origem relacionado ao alerta, por exemplo, a interface do usuário do provedor para alertas ou pesquisa de log, etc.|
|status *|alertStatus|Status do ciclo de vida do alerta (estágio). Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`. (oferece suporte a [atualização](../api/alert_update.md))|
|marcas|Coleção de cadeias de caracteres|Rótulos definidos pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "SAW", etc.) (oferece suporte a [atualização](../api/alert_update.md)).|
|title *|Cadeia de caracteres|Título do alerta.|
|triggers|coleção [alertTrigger](alerttrigger.md)|Informações relacionadas à segurança sobre as propriedades específicas que acionaram o alerta (propriedades que aparecem no alerta). Os alertas podem conter informações sobre vários usuários, hosts, arquivos, endereços IP. Este campo indica quais propriedades dispararam a geração de alerta.|
|userStates|coleção [userSecurityState](usersecuritystate.md)|Informações de estado relacionadas à segurança geradas pelo provedor sobre as chaves de registro relacionadas a esse alerta.|
|vendorInformation *|[securityVendorInformation](securityvendorinformation.md)|Contém detalhes sobre o fornecedor, provedor e subprovedor de produtos/serviços de segurança (por exemplo,  vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).|
|vulnerabilityStates|coleção [vulnerabilityState](vulnerabilitystate.md)|Inteligência de ameaças referente a uma ou mais vulnerabilidades relacionadas a esse alerta.|
(\* Indica um campo obrigatório.)

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alert"
}-->

```json
{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [{"@odata.type": "microsoft.graph.cloudAppSecurityState"}],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [{"@odata.type": "microsoft.graph.fileSecurityState"}],
  "hostStates": [{"@odata.type": "microsoft.graph.hostSecurityState"}],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [{"@odata.type": "microsoft.graph.malwareState"}],
  "networkConnections": [{"@odata.type": "microsoft.graph.networkConnection"}],
  "processes": [{"@odata.type": "microsoft.graph.process"}],
  "recommendedActions": ["String"],
  "registryKeyStates": [{"@odata.type": "microsoft.graph.registryKeyState"}],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [{"@odata.type": "microsoft.graph.alertTrigger"}],
  "userStates": [{"@odata.type": "microsoft.graph.userSecurityState"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "vulnerabilityStates": [{"@odata.type": "microsoft.graph.vulnerabilityState"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->