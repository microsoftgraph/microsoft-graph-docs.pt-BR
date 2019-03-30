---
title: tipo de recurso tiIndicator
description: Os indicadores de inteligência da ameaça (TI) representam dados usados para identificar atividades mal-intencionadas. Se sua organização trabalha com indicadores de ameaça, gerando sua própria, obtendo de feeds de origem aberta, compartilhando com organizações de parceiros ou comunidades, ou comprando feeds de dados, você geralmente deseja usar esses indicadores em várias segurança ferramentas de correspondência com dados de log. A entidade de segurança do gráfico tiIndicators permite que você carregue seus indicadores de ameaça para as ferramentas de segurança da Microsoft para as ações de permitir, bloquear ou alertar.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fd86dc4da572c17e35afe939977b65ff99bd30be
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988858"
---
# <a name="tiindicator-resource-type"></a>tipo de recurso tiIndicator

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os indicadores de inteligência da ameaça (TI) representam dados usados para identificar atividades mal-intencionadas. Se sua organização trabalha com indicadores de ameaça, gerando sua própria, obtendo seus próprios feeds de fontes abertas, compartilhando com organizações ou comunidades parceiras ou comprando feeds de dados, talvez você queira usar esses indicadores em várias segurança ferramentas de correspondência com dados de log. A entidade **TIINDICATORS** API de segurança do Microsoft Graph permite que você carregue seus indicadores de ameaça para as ferramentas de segurança da Microsoft para as ações de permitir, bloquear ou alertar.

Os indicadores de ameaça carregados por meio do **tiIndicators** serão usados em conjunto com o Microsoft Threat Intelligence para fornecer uma solução de segurança personalizada para sua organização. Ao usar a entidade **tiIndicators** , você especifica a solução de segurança da Microsoft para a qual deseja utilizar os indicadores por meio da propriedade **targetProduct** e especifica a ação (permitir, bloquear ou alerta) à qual a solução de segurança deve Aplique os indicadores por meio da propriedade **Action** .

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter tiIndicator](../api/tiindicator-get.md) | [tiIndicator](tiindicator.md) | Leia as propriedades e os relacionamentos do objeto tiIndicator. |
| [Criar tiIndicator](../api/tiindicators-post.md) | [tiIndicator](tiindicator.md) | Crie um novo tiIndicator postando na coleção tiIndicators. |
| [Lista tiIndicators](../api/tiindicators-list.md) | coleção [tiIndicator](tiindicator.md) | Obtenha uma coleção de objetos tiIndicator. |
| [Update](../api/tiindicator-update.md) | [tiIndicator](tiindicator.md) | Atualize o objeto tiIndicator. |
| [Excluir](../api/tiindicator-delete.md) | Nenhum | Exclua o objeto tiIndicator. |
|[deleteTiIndicators](../api/tiindicator-deletetiindicators.md)|Nenhum| Excluir vários objetos tiIndicator.|
|[deleteTiIndicatorsByExternalId](../api/tiindicator-deletetiindicatorsbyexternalid.md)|Nenhum| Excluir vários objetos tiIndicator pela `externalId` propriedade.|
|[submitTiIndicators](../api/tiindicator-submittiindicators.md)|coleção [tiIndicator](tiindicator.md)|Criar novo tiIndicators postando uma coleção tiIndicators.|
|[updateTiIndicators](../api/tiindicator-updatetiindicators.md)|coleção [tiIndicator](tiindicator.md)| Atualizar vários objetos tiIndicator.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|action|string| A ação a ser aplicada se o indicador for correspondido de dentro da ferramenta de segurança do targetProduct. Os valores possíveis são: `unknown`, `allow`, `block`, `alert`. **Obrigatório.**|
|activityGroupNames|Coleção String|O nome do Cyber Threat Intelligence (s) para as partes responsáveis pela atividade mal-intencionada coberta pelo indicador de ameaças.|
|additionalInformation|String|Uma área catchall na qual os dados extras do indicador não cobertos pelas outras propriedades de tiIndicator podem ser colocados. Os dados colocados no additionalInformation normalmente não serão utilizados pela ferramenta de segurança do targetProduct.|
|azureTenantId|String| Marcado pelo sistema quando o indicador está ingerido. A ID de locatário do Azure Active Directory do cliente remetente. **Obrigatório.**|
|confidence|Int32|Um inteiro representando a confiança dos dados dentro do indicador identifica precisamente o comportamento mal-intencionado. Os valores aceitáveis são 0 – 100 com 100 sendo os mais altos.|
|description|String| Breve descrição (100 caracteres ou menos) da ameaça representada pelo indicador. **Obrigatório.**|
|diamondModel|[diamondModel](#diamondmodel-values)|A área do modelo em losango em que esse indicador existe. Os valores possíveis são: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| Cadeia de caracteres DateTime indicando quando o indicador expira. Todos os indicadores devem ter uma data de vencimento para evitar indicadores obsoletos persistentes no sistema. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. **Obrigatório.**|
|externalId|Cadeia de caracteres| Um número de identificação que liga o indicador de volta para o sistema do provedor de indicadores (por exemplo, uma chave externa). |
|id|String|Criado pelo sistema quando o indicador é ingerido. GUID gerado/identificador exclusivo. Somente leitura.|
|ingestedDateTime|DateTimeOffset| Marcado pelo sistema quando o indicador está ingerido. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|isActive|Booliano| Usado para desativar indicadores no sistema. Por padrão, qualquer indicador enviado é definido como ativo. No enTanto, os provedores podem enviar indicadores existentes com este conjunto como ' false ' para desativar indicadores no sistema.|
|killChain|coleção [killChain](#killchain-values)|Uma matriz JSON de cadeias de caracteres que descreve o ponto ou os pontos na cadeia de Kill que este indicador aponta. Consulte ' valores killChain ' abaixo para ver os valores exatos. |
|knownFalsePositives|String|Cenários nos quais o indicador pode causar falsos positivos. Isso deve ser um texto legível por pessoas.|
|lastReportedDateTime|DateTimeOffset|A última vez que o indicador foi visto. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|malwareFamilyNames|Coleção String|O nome da família de malware associado a um indicador, se existir. A Microsoft prefere o nome da família de malware da Microsoft, se possível, que possa ser encontrado por meio da [enciclopédia de ameaças](https://www.microsoft.com/wdsi/threats)de inteligência de segurança do Windows Defender.|
|passiveOnly|Booliano |Determina se o indicador deve acionar um evento que é visível para um usuário final. Quando definido como ' true ', as ferramentas de segurança não notificarão o usuário final de que um ' hit ' ocorreu. Isso geralmente é tratado como um modo de auditoria ou silencioso por produtos de segurança onde eles simplesmente farão o registro de que uma correspondência ocorreu, mas não executará a ação. O valor padrão é falso. |
|severity|Int32| Um inteiro que representa a gravidade do comportamento mal-intencionado identificado pelos dados dentro do indicador. Os valores aceitáveis são 0 – 5, onde 5 é o mais grave e zero não é grave. O valor padrão é 3. |
|tags|String collection|Uma matriz JSON de cadeias de caracteres que armazena marcas arbitrárias/palavras-chave. |
|targetProduct|String|Um valor String que representa um único produto de segurança ao qual o indicador deve ser aplicado. Os valores aceitáveis `Azure Sentinel`são:. **Required**|
|threattype|[threattype](#threattype-values)| Cada indicador deve ter um tipo de ameaça de indicador válido. Os valores possíveis são: `Botnet`, `C2`, `CryptoMining`, `Darknet`, `DDoS`, `MaliciousUrl`, `Malware`, `Phishing`, `Proxy`, `PUA`, `WatchList`. **Obrigatório.** |
|tlpLevel|[tlpLevel](#tlplevel-values)| Valor do protocolo de luz de tráfego para o indicador. Os valores possíveis são: `unknown`, `white`, `green`, `amber`, `red`. **Obrigatório.**|

### <a name="indicator-observables---email"></a>Indicador observáveis-email

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|emailEncoding|String|O tipo de codificação de texto usado no email.|
|emailLanguage|String|O idioma do email.|
|emailRecipient|String|Endereço de email do destinatário.|
|emailSenderAddress|String|Endereço de email do attacker& # 124; vítima.|
|emailSenderName|String|Nome exibido da attacker& # 124; vítima.|
|emailSourceDomain|String|Domínio usado no email.|
|emailSourceIpAddress|String|Endereço IP de origem do email.|
|emailSubject|String|Linha de assunto do email.|
|emailXMailer|String|Valor do X-Mailer usado no email.|

### <a name="indicator-observables---file"></a>Indicador observáveis-arquivo

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|fileCompileDateTime|DateTimeOffset|DateTime quando o arquivo foi compilado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|fileCreatedDateTime|DateTimeOffset| DateTime quando o arquivo foi criado. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|fileHashType|string| O tipo de hash armazenado em fileHashvalue. Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`.|
|fileHashvalue|String| O valor de hash do arquivo.|
|fileMutexname|String| Nome mutex usado em detecções baseadas em arquivo.|
|fileName|String|Nome do arquivo se o indicador for baseado em arquivo. Vários nomes de arquivo podem ser delimitados por vírgulas. |
|filePackr|String|O empacotador usado para criar o arquivo em questão.|
|filePath|String|Caminho do arquivo que indica o compromisso. Pode ser um caminho de estilo Windows ou * Nix.|
|Tamanho|Int64|Tamanho do arquivo em bytes.|
|fileType|String| Descrição de texto do tipo de arquivo. Por exemplo, "documento do Word" ou "binário".|

### <a name="indicator-observables---network"></a>Indicador observáveis-rede

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|domainName|Cadeia de caracteres|Nome de domínio associado a esse indicador. Deve ser do formato subdomain. domain. TopLevelDomain (por exemplo, baddomain.domain.net)|
|networkCidrBlock|String| Representação de notação de bloqueio CIDR da rede referenciada neste indicador. Use somente se a origem e o destino não puderem ser identificados. |
|networkDestinationAsn|Int32|O identificador de sistema autônomo de destino da rede referenciada no indicador.|
|networkDestinationCidrBlock|String|Representação de notação de bloqueio CIDR da rede de destino neste indicador.|
|networkDestinationIPv4|String|Destino do endereço IP IPv4.|
|networkDestinationIPv6|String|Destino do endereço IP IPv6.|
|networkDestinationPort|Int32|Destino da porta TCP.|
|networkIPv4|String| Endereço IP IPv4. Use somente se a origem e o destino não puderem ser identificados. |
|networkIPv6|String| Endereço IP IPv6. Use somente se a origem e o destino não puderem ser identificados. |
|networkPort|Int32| Porta TCP. Use somente se a origem e o destino não puderem ser identificados. |
|networkProtocol|Int32|Representação decimal do campo de protocolo no cabeçalho IPv4.|
|networkSourceAsn|Int32|O identificador de sistema autônomo de origem da rede referenciada no indicador.|
|networkSourceCidrBlock|String|Representação de notação de bloqueio CIDR da rede de origem neste indicador|
|networkSourceIPv4|String|Origem do endereço IP IPv4.|
|networkSourceIPv6|String|Origem do endereço IP IPv6.|
|networkSourcePort|Int32|Origem da porta TCP.|
|url|String|Localizador de recursos uniforme. Esta URL deve estar em conformidade com a RFC 1738.|
|userAgent|String|Cadeia de caracteres do agente de usuário de uma solicitação da Web que pode indicar comprometimento.|

### <a name="diamondmodel-values"></a>valores de diamondModel

Para obter informações sobre esse modelo, consulte [o modelo de losango](http://diamondmodel.org).

| Valores | Descrição |
|:-------|:------------|
|adversário|O indicador descreve o adversário.|
|função|O indicador é uma capacidade do adversário.|
|ti|O indicador descreve a infraestrutura do adversário.|
|vítima|O indicador descreve a vítima do adversário.|

### <a name="killchain-values"></a>valores de killChain

| Valores | Descrição |
|:-------|:------------|
|Ações|Indcates que o atacante está aproveitando o sistema comprometido para realizar ações como um ataque de negação de serviço distribuído.|
|C2|Representa o canal de controle pelo qual um sistema comprometido é manipulado.|
|Delivery|O processo de distribuição do código de exploração para vítimas (por exemplo, USB, email, sites).|
|Invasão|O código de exploração que aproveita as vulnerabilidades (por exemplo, execução de código).|
|Instalação|Instalação de malware após uma vulnerabilidade ter sido explorada.|
|Reconhecimento|O indicador é uma evidência de um grupo de atividades que coleta informações a serem usadas em um ataque futuro.|
|Armas|Transformar uma vulnerabilidade em código de exploração (por exemplo, malware).|

### <a name="threattype-values"></a>valores de threattype

| Valores | Descrição |
|:-------|:------------|
|Botnet| O indicador é detalhando um nó/membro de botnet.|
|C2|O indicador é detalhando o nó de controle & de um comando de um botnet.|
|CryptoMining|O tráfego que envolve esse endereço de rede/URL é uma indicação de abuso de CyrptoMining/recurso.|
|Darknet|O indicador é o de um nó/rede do Darknet.
|DDoS|Indicadores relacionados a uma campanha de DDoS ativa ou futura.|
|MaliciousUrl|URL que serve de malware.|
|Malware|Indicador que descreve um arquivo ou arquivos mal-intencionados.|
|Phishing|Indicadores relacionados a uma campanha de phishing.|
|Acionista|O indicador é o de um serviço de proxy.|
|PUA|Aplicativo potencialmente inDesejado.|
|Watchlist|Este é o Bucket genérico no qual os indicadores são colocados quando não é possível determinar exatamente qual é a ameaça ou será necessária a interpretação manual. Normalmente, isso não deve ser usado pelos parceiros que enviam dados para o sistema.|

### <a name="tlplevel-values"></a>valores de tlpLevel

Cada indicador também deve ter um valor de protocolo de luz de tráfego quando ele é enviado. Esse valor representa a sensibilidade e o escopo de compartilhamento de um determinado indicador.

| Valores | Descrição |
|:-------|:------------|
|Branco| Escopo de compartilhamento: ilimitado. Os indicadores podem ser compartilhados livremente, sem restrição.|
|Verde| Escopo de compartilhamento: Comunidade. Os indicadores podem ser compartilhados com a comunidade de segurança.|
|Âmbar| Escopo de compartilhamento: limitado. Essa é a configuração padrão para indicadores e restringe o compartilhamento apenas àqueles com os serviços e operadores de serviço "necessário para saber", que implementam a inteligência da ameaça 2) clientes cujos sistemas de exposição de sistema (es) são consistentes com o indicador.|
|Vermelho| Escopo de compartilhamento: pessoal. Esses indicadores devem ser compartilhados apenas diretamente e, preferencialmente, em pessoa. Normalmente, os indicadores vermelhos do TLP não são incluídos devido às restrições predefinidas. Se TLP indicadores vermelhos forem enviados, a propriedade "PassiveOnly" também deverá ser definida `True` . |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tiIndicator",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "action": "string",
  "activityGroupNames": ["String"],
  "additionalInformation": "String",
  "azureTenantId": "String",
  "confidence": 1024,
  "description": "String",
  "diamondModel": "string",
  "domainName": "String",
  "emailEncoding": "String",
  "emailLanguage": "String",
  "emailRecipient": "String",
  "emailSenderAddress": "String",
  "emailSenderName": "String",
  "emailSourceDomain": "String",
  "emailSourceIpAddress": "String",
  "emailSubject": "String",
  "emailXMailer": "String",
  "expirationDateTime": "String (timestamp)",
  "externalId": "String",
  "fileCompileDateTime": "String (timestamp)",
  "fileCreatedDateTime": "String (timestamp)",
  "fileHashType": "string",
  "fileHashValue": "String",
  "fileMutexName": "String",
  "fileName": "String",
  "filePacker": "String",
  "filePath": "String",
  "fileSize": 1024,
  "fileType": "String",
  "id": "String (identifier)",
  "ingestedDateTime": "String (timestamp)",
  "isActive": true,
  "killChain": ["String"],
  "knownFalsePositives": "String",
  "lastReportedDateTime": "String (timestamp)",
  "malwareFamilyNames": ["String"],
  "networkCidrBlock": "String",
  "networkDestinationAsn": 1024,
  "networkDestinationCidrBlock": "String",
  "networkDestinationIPv4": "String",
  "networkDestinationIPv6": "String",
  "networkDestinationPort": 1024,
  "networkIPv4": "String",
  "networkIPv6": "String",
  "networkPort": 1024,
  "networkProtocol": 1024,
  "networkSourceAsn": 1024,
  "networkSourceCidrBlock": "String",
  "networkSourceIPv4": "String",
  "networkSourceIPv6": "String",
  "networkSourcePort": 1024,
  "passiveOnly": true,
  "severity": 1024,
  "tags": ["String"],
  "targetProduct": "String",
  "threatType": "String",
  "tlpLevel": "string",
  "url": "String",
  "userAgent": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
