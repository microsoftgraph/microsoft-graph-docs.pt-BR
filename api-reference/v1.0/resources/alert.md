# <a name="alert-resource-type"></a>tipo de recurso de alerta

Representa os possíveis problemas de segurança dentro do locatário do cliente que identificaram as soluções de segurança da Microsoft ou parceiro. Use alertas para unificar e simplificar o gerenciamento de problemas de segurança em todas as soluções integradas. Para saber mais, consulte os exemplos de consultas no [Explorer do gráfico](https://developer.microsoft.com/graph/graph-explorer).

Alertas podem ser recuperadas de provedores de segurança diferentes listados na [Visão geral de segurança do Microsoft Graph](security-api-overview.md).

## <a name="methods"></a>Métodos

| Método   | Tipo de retorno|Descrição|
|:---------------|:--------|:----------|
|[Obter alerta](../api/alert_get.md) | [alerta](alert.md) |Leia as propriedades e os relacionamentos de um objeto de alerta.|
|[Atualizar alertas](../api/alert_update.md) | [alerta](alert.md) |Atualize um objeto de alerta. |
|[Listar alertas](../api/alert_list.md) | coleção de [alerta](alert.md) |Obtenha uma coleção de objetos de alerta.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|activityGroupName|String|Nome ou alias do grupo de atividade (invasor) esse alerta é atribuído à.|
|assignedTo|String|Nome do analista de alerta é atribuída a triagem, investigação ou correção (oferece suporte a [atualização](../api/alert_update.md)).|
|azureSubscriptionId|String|ID de assinatura do Windows Azure, presente se esse alerta está relacionado a um recurso do Windows Azure.|
|azureTenantId |String|ID do locatário Azure Active Directory. Obrigatório.|
|Ferramentas para desenvolvedores|Cadeia de caracteres|Categoria do alerta (por exemplo, credentialTheft, ransomware, etc.).|
|closedDateTime|DateTimeOffset|Hora em que o alerta foi fechado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de Jan de 2014 ficaria assim: `'2014-01-01T00:00:00Z'` (oferece suporte a [atualização](../api/alert_update.md)).|
|cloudAppStates|coleção [cloudAppSecurityState](cloudappsecuritystate.md)|Informações de estado relacionadas à segurança geradas pelo provedor sobre o aplicativo/s de nuvem relacionado a este alerta.|
|comentários|String collection|Enviar comentários fornecido pelo cliente alerta (para gerenciamento de alerta do cliente) (oferece suporte a [atualização](../api/alert_update.md)).|
|confidence|Int32|Confiança da lógica de detecção (percentual entre 1-100).|
|createdDateTime |DateTimeOffset|Hora em que o alerta foi criado pelo provedor de alerta. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Obrigatório.|
|description|String|Descrição do alerta.|
|detectionIds|String collection|Conjunto de alertas relacionados a essa entidade alerta (todos os alertas são enviados para o SIEM como um registro separado).|
|eventDateTime |DateTimeOffset|Hora em que o evento (s) que servia como o entrarão para gerar o alerta ocorreu. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Obrigatório.|
|comentários|alertFeedback|Comentários analista no alerta. Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`. (oferece suporte a [atualização](../api/alert_update.md))|
|fileStates|coleção [fileSecurityState](filesecuritystate.md)|Informações de com informações de estado relacionadas à segurança geradas pelo provedor sobre os arquivos relacionados a este alerta.|
|hostStates|coleção [hostSecurityState](hostsecuritystate.md)|Informações de estado relacionadas à segurança geradas pelo provedor sobre o (s) relacionadas a este alerta.|
|id |String|Identificador GUID/exclusivo gerado pelo provedor. Somente leitura. Obrigatório.|
|lastModifiedDateTime|DateTimeOffset|Hora em que a entidade de alerta foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|malwareStates|coleção [malwareState](malwarestate.md)|Inteligência de ameaça referentes ao relacionadas a este alerta de malware.|
|networkConnections|coleção [networkConnection](networkconnection.md)|Informações de estado relacionadas à segurança geradas pelo provedor sobre as conexões de rede relacionadas a este alerta.|
|processos|coleção de [processo](process.md)|Informações de estado relacionadas à segurança geradas pelo provedor sobre o processo ou processos relacionados a este alerta.|
|recommendedActions|String collection|Fornecedor/provedor recomendado as ações assuma como resultado de alerta (por exemplo, isolar máquina, enforce2FA, host nova imagem).|
|registryKeyStates|coleção [registryKeyState](registrykeystate.md)|Informações de registro de estado relacionadas à segurança geradas pelo provedor sobre as chaves do registro relacionadas a este alerta.|
|severidade |alertSeverity|Alerta gravidade - definida pelo fornecedor/provedor. Os valores possíveis são: `unknown`, `informational`, `low`, `medium`, `high`. Obrigatório.|
|sourceMaterials|String collection|Hiperlinks (URIs) para o material de origem relacionado ao alerta, por exemplo, interface do usuário do provedor de alertas ou de pesquisa de log, etc.|
|status |alertStatus|Status do ciclo de vida de alerta (estágio). Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`. (oferece suporte a [atualização](../api/alert_update.md)). Obrigatório.|
|marcas|String collection|Rótulos podem ser definidos pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo "HVA", "SERRA", etc.) (oferece suporte a [atualização](../api/alert_update.md)).|
|title |String|Título do alerta. Obrigatório.|
|gatilhos|coleção [alertTrigger](alerttrigger.md)|Informações relacionadas a segurança sobre as propriedades específicas que disparou o alerta (que aparecem no alerta de propriedades). Alertas deve conter informações sobre vários usuários, hosts, arquivos, endereços ip. Este campo indica quais propriedades disparou a geração de alerta.|
|userStates|coleção [userSecurityState](usersecuritystate.md)|Informações de registro de estado relacionadas à segurança geradas pelo provedor sobre as contas de usuário relacionadas a este alerta.|
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|Tipo complexo que contém detalhes sobre o fornecedor de serviço do produto de segurança, o provedor e subprovider (por exemplo, o fornecedor = Microsoft; provider = ATP do Windows Defender; subProvider = AppLocker). Obrigatório.|
|vulnerabilityStates|coleção [vulnerabilityState](vulnerabilitystate.md)|Inteligência de ameaça referentes a um ou mais vulnerabilidades relacionadas a este alerta.|

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