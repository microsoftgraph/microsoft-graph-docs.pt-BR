---
title: Tipo de recurso tiIndicator
description: Os indicadores de inteligência contra ameaças (TI) representam dados usados para identificar atividades mal-intencionadas.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 33c14b4bc60fe492c961445cb294200555e2cc9a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158741"
---
# <a name="tiindicator-resource-type"></a>Tipo de recurso tiIndicator

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os indicadores de inteligência contra ameaças (TI) representam dados usados para identificar atividades mal-intencionadas. Se sua organização trabalha com indicadores de ameaças, seja gerando seus próprios, obtendo-os de feeds de código aberto, compartilhando com organizações ou comunidades parceiras ou comprando feeds de dados, talvez você queira usar esses indicadores em várias ferramentas de segurança para corresponder aos dados de log. A entidade **tiIndicators** da API de Segurança do Microsoft Graph permite carregar seus indicadores de ameaça para as ferramentas de segurança da Microsoft para as ações de permitir, bloquear ou alerta.

Os indicadores de ameaças carregados por **meio de tiIndicators** serão usados em conjunto com a inteligência contra ameaças da Microsoft para fornecer uma solução de segurança personalizada para sua organização. Ao usar a entidade **tiIndicators,** você especifica a solução de segurança da Microsoft para a qual deseja utilizar os indicadores por meio da propriedade  **targetProduct** e especifica a ação (permitir, bloquear ou alerta) à qual a solução de segurança deve aplicar os indicadores por meio da propriedade de ação.

O **suporte a targetProduct** atual inclui o seguinte:

- **Azure Sentinel** – Oferece suporte a todos os **métodos tiIndicators** documentados listados na seção a seguir.
- **Microsoft Defender ATP (Proteção Avançada contra** Ameaças do Microsoft Defender) – oferece suporte aos seguintes métodos **tiIndicators:**
     - [Obter tiIndicator](../api/tiindicator-get.md)
     - [Criar tiIndicator](../api/tiindicators-post.md)
     - [Lista tiIndicators](../api/tiindicators-list.md)
     - [Update](../api/tiindicator-update.md)
     - [Delete](../api/tiindicator-delete.md)

     O suporte para os métodos em massa será em breve.

  > [!NOTE]
  >Os seguintes tipos de indicadores são suportados pelo Microsoft Defender ATP targetProduct:
  > - Arquivos
  > - Endereços IP: o Microsoft Defender ATP dá suporte somente a IPv4/IPv6 de destino – definir propriedade nas propriedades networkDestinationIPv4 ou networkDestinationIPv6 na API de Segurança do Microsoft Graph **tiIndicator**.
  > - URLs/domínios

   Há um limite de 15.000 indicadores por locatário do Microsoft Defender ATP.

Para mais detalhes sobre os tipos de indicadores com suporte e limites de contagens de indicadores por locatário, confira [Gerenciar indicadores](/windows/security/threat-protection/microsoft-defender-atp/manage-indicators).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter tiIndicator](../api/tiindicator-get.md) | [tiIndicator](tiindicator.md) | Leia as propriedades e os relacionamentos do objeto tiIndicator. |
| [Criar tiIndicator](../api/tiindicators-post.md) | [tiIndicator](tiindicator.md) | Crie um novo tiIndicator postando na coleção tiIndicators. |
| [Lista tiIndicators](../api/tiindicators-list.md) | [Coleção tiIndicator](tiindicator.md) | Obter uma coleção de objetos tiIndicator. |
| [Update](../api/tiindicator-update.md) | [tiIndicator](tiindicator.md) | Atualize o objeto tiIndicator. |
| [Delete](../api/tiindicator-delete.md) | Nenhum(a) | Exclua o objeto tiIndicator. |
|[deleteTiIndicators](../api/tiindicator-deletetiindicators.md)|Nenhum(a)| Exclua vários objetos tiIndicator.|
|[deleteTiIndicatorsByExternalId](../api/tiindicator-deletetiindicatorsbyexternalid.md)|Nenhum(a)| Exclua vários objetos tiIndicator pela `externalId` propriedade.|
|[submitTiIndicators](../api/tiindicator-submittiindicators.md)|[Coleção tiIndicator](tiindicator.md)|Crie novos tiIndicators postando uma coleção tiIndicators.|
|[updateTiIndicators](../api/tiindicator-updatetiindicators.md)|[Coleção tiIndicator](tiindicator.md)| Atualize vários objetos tiIndicator.|

### <a name="methods-supported-by-each-target-product"></a>Métodos suportados por cada produto de destino

| Método                                                          | Azure Sentinel                                                                                                                                                                                                                                                                                                                                                                      | O Microsoft Defender ATP                                                                                                                                                                                               |
|:----------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Criar tiIndicator](../api/tiindicators-post.md)               | Os campos obrigatórios são: , , , , , e pelo menos um `action` `azureTenantId` `description` `expirationDateTime` `targetProduct` `threatType` `tlpLevel` email, rede ou arquivo observável.                                                                                                                                                                                                | Os campos obrigatórios são: `action` e um destes valores: , `domainName` , , ( deve fornecer no caso de `url` `networkDestinationIPv4` `networkDestinationIPv6` `fileHashValue` `fileHashType` `fileHashValue` ). |
| [Enviar tiIndicators](../api/tiindicator-submittiindicators.md) | Consulte o método [Create tiIndicator](../api/tiindicators-post.md) para campos obrigatórios para cada tiIndicator. Há um limite de 100 tiIndicators por solicitação.                                                                                                                                                                                                                    | Consulte o método [Create tiIndicator](../api/tiindicators-post.md) para campos obrigatórios para cada tiIndicator. Há um limite de 100 tiIndicators por solicitação.                                                     |
| [Atualizar tiIndicator](../api/tiindicator-update.md)              | Os campos obrigatórios são: `id` , `expirationDateTime` . `targetProduct` <br> Os campos editáveis são:  `action` , , , , , , , , `activityGroupNames` , , , `additionalInformation` , , , `confidence` , `description` `diamondModel` , `expirationDateTime` `externalId` `isActive` `killChain` `knownFalsePositives` `lastReportedDateTime` `malwareFamilyNames` `passiveOnly` `severity` `tags` `tlpLevel` . | Os campos obrigatórios são: `id` , `expirationDateTime` . `targetProduct` <br> Os campos editáveis são: `expirationDateTime` , `severity` . `description`                                                                         |
| [Atualizar tiIndicators](../api/tiindicator-updatetiindicators.md) | Consulte o método [Update tiIndicator](../api/tiindicator-update.md) para campos obrigatórios e editáveis para cada tiIndicator.                                                                                                                                                                                                                                                       | <p align="center">[Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p>                                                                                                             |
| [Excluir tiIndicator](../api/tiindicator-delete.md)              | O campo obrigatório é: `id` .                                                                                                                                                                                                                                                                                                                                                            | O campo obrigatório é: `id` .                                                                                                                                                                                             |
| [Excluir tiIndicators](../api/tiindicator-deletetiindicators.md) | Consulte o [método Delete tiIndicator](../api/tiindicator-delete.md) acima para o campo necessário para cada tiIndicator.                                                                                                                                                                                                                                                               | <p align="center">[Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p>                                                                                                             |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ação|string| A ação a ser aplicada se o indicador for corresponder de dentro da ferramenta de segurança targetProduct. Os valores possíveis são: `unknown`, `allow`, `block`, `alert`. **Obrigatório.**|
|activityGroupNames|Coleção de cadeias de caracteres|Os nomes de inteligência contra ameaças cibernéticas para as partes responsáveis pelas atividades mal-intencionadas cobertas pelo indicador de ameaças.|
|additionalInformation|String|Uma área catchall na qual dados extras do indicador não cobertos pelas outras propriedades tiIndicator podem ser colocados. Os dados colocados em additionalInformation normalmente não serão utilizados pela ferramenta de segurança targetProduct.|
|azureTenantId|String| Carimbado pelo sistema quando o indicador é ingerido. A ID de locatário do Azure Active Directory do cliente de envio. **Obrigatório.**|
|confidence|Int32|Um inteiro que representa a confiança dos dados no indicador identifica com precisão o comportamento mal-intencionado. Os valores aceitáveis são de 0 a 100, sendo 100 o maior.|
|description|String| Breve descrição (100 caracteres ou menos) da ameaça representada pelo indicador. **Obrigatório.**|
|diamondModel|[diamondModel](#diamondmodel-values)|A área do Modelo de Losango na qual esse indicador existe. Os valores possíveis são: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| Cadeia de caracteres DateTime que indica quando o Indicador expira. Todos os indicadores devem ter uma data de expiração para evitar que os indicadores persistentes persistam no sistema. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. **Obrigatório.**|
|externalId|Cadeia de caracteres| Um número de identificação que vincula o indicador de volta ao sistema do provedor do indicador (por exemplo, uma chave estrangeira). |
|id|String|Criado pelo sistema quando o indicador é ingerido. Identificador GUID/exclusivo gerado. Somente leitura.|
|ingestedDateTime|DateTimeOffset| Carimbado pelo sistema quando o indicador é ingerido. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|isActive|Boolean| Usado para desativar indicadores no sistema. Por padrão, qualquer indicador enviado é definido como ativo. No entanto, os provedores podem enviar indicadores existentes com esse conjunto como "Falso" para desativar os indicadores no sistema.|
|killChain|[Coleção killChain](#killchain-values)|Uma matriz JSON de cadeias de caracteres que descreve qual ponto ou pontos no Kill Chain este indicador se direciona. Consulte 'valores killChain' abaixo para saber os valores exatos. |
|knownFalsePositives|String|Cenários em que o indicador pode causar falsos positivos. Deve ser um texto acessível para humanos.|
|lastReportedDateTime|DateTimeOffset|A última vez em que o indicador foi visto. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|malwareFamilyNames|Coleção de cadeias de caracteres|O nome da família de malware associado a um indicador, se ele existir. A Microsoft prefere o nome da família de malware da Microsoft, se possível, que pode ser encontrado por meio da ameaça de inteligência de segurança do Windows [Defender.](https://www.microsoft.com/wdsi/threats)|
|passiveOnly|Boolean |Determina se o indicador deve disparar um evento visível para um usuário final. Quando definido como "verdadeiro", as ferramentas de segurança não notificarão o usuário final de que ocorreu um 'acerto'. Isso é tratado com mais frequência como auditoria ou modo silencioso pelos produtos de segurança, onde eles simplesmente registram que uma combinação ocorreu, mas não executarão a ação. O valor padrão é falso. |
|severity|Int32| Um inteiro que representa a gravidade do comportamento mal-intencionado identificado pelos dados dentro do indicador. Os valores aceitáveis são de 0 a 5, onde 5 é o mais grave e zero não é grave. O valor padrão é 3. |
|tags|Coleção de cadeias de caracteres|Uma matriz JSON de cadeias de caracteres que armazena marcas/palavras-chave arbitrárias. |
|targetProduct|String|Um valor de cadeia de caracteres que representa um único produto de segurança ao qual o indicador deve ser aplicado. Os valores aceitáveis são: `Azure Sentinel` , `Microsoft Defender ATP` . **Required**|
|threatType|[threatType](#threattype-values)| Cada indicador deve ter um tipo de ameaça válido. Os valores possíveis são: `Botnet`, `C2`, `CryptoMining`, `Darknet`, `DDoS`, `MaliciousUrl`, `Malware`, `Phishing`, `Proxy`, `PUA`, `WatchList`. **Obrigatório.** |
|tlpLevel|[tlpLevel](#tlplevel-values)| Valor do Protocolo semáforo para o indicador. Os valores possíveis são: `unknown`, `white`, `green`, `amber`, `red`. **Obrigatório.**|

### <a name="indicator-observables---email"></a>Indicador observáveis - email

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|emailEncoding|String|O tipo de codificação de texto usado no email.|
|emailLanguage|String|O idioma do email.|
|emailRecipient|String|Endereço de email do destinatário.|
|emailSenderAddress|String|Endereço de email do invasor&#124;vítima.|
|emailSenderName|String|Nome exibido do invasor&#124;vítima.|
|emailSourceDomain|String|Domínio usado no email.|
|emailSourceIpAddress|String|Endereço IP de origem do email.|
|emailSubject|String|Linha de assunto do email.|
|emailXMailer|String|Valor X-Mailer usado no email.|

### <a name="indicator-observables---file"></a>Indicador observáveis - arquivo

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|fileCompileDateTime|DateTimeOffset|DateTime quando o arquivo foi compilado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|fileCreatedDateTime|DateTimeOffset| DateTime quando o arquivo foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|fileHashType|string| O tipo de hash armazenado em fileHashValue. Os valores possíveis são: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`.|
|fileHashValue|String| O valor de hash do arquivo.|
|fileMutexName|String| Nome mutex usado em detecções baseadas em arquivo.|
|fileName|String|Nome do arquivo se o indicador for baseado em arquivo. Vários nomes de arquivo podem ser delimitados por vírgulas. |
|filePacker|String|O filho usado para criar o arquivo em questão.|
|filePath|String|Caminho do arquivo indicando comprometimento. Pode ser um caminho de estilo windows ou *nix.|
|fileSize|Int64|Tamanho do arquivo em bytes.|
|fileType|String| Descrição do texto do tipo de arquivo. Por exemplo, "Documento do Word" ou "Binário".|

### <a name="indicator-observables---network"></a>Indicador observáveis - rede

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|domainName|Cadeia de caracteres|Nome de domínio associado a esse indicador. Deve ser do formato subdomínio.domínio.topleveldomain (por exemplo, baddomain.domain.net)|
|networkCidrBlock|String| Representação de notação de bloqueio CIDR da rede referenciada neste indicador. Use somente se a fonte e o destino não puderem ser identificados. |
|networkDestinationAsn|Int32|O identificador de sistema autônomo de destino da rede referenciada no indicador.|
|networkDestinationCidrBlock|String|Representação de notação de bloqueio CIDR da rede de destino neste indicador.|
|networkDestinationIPv4|String|Destino do endereço IP IPv4.|
|networkDestinationIPv6|String|Destino do endereço IP IPv6.|
|networkDestinationPort|Int32|Destino da porta TCP.|
|networkIPv4|String| Endereço IP IPv4. Use somente se a fonte e o destino não puderem ser identificados. |
|networkIPv6|String| Endereço IP IPv6. Use somente se a fonte e o destino não puderem ser identificados. |
|networkPort|Int32| Porta TCP. Use somente se a fonte e o destino não puderem ser identificados. |
|networkProtocol|Int32|Representação decimal do campo de protocolo no header IPv4.|
|networkSourceAsn|Int32|O identificador de sistema autônomo de origem da rede referenciado no indicador.|
|networkSourceCidrBlock|String|Representação de notação de bloqueio CIDR da rede de origem neste indicador|
|networkSourceIPv4|String|Origem do endereço IP IPv4.|
|networkSourceIPv6|String|Fonte de endereço IP IPv6.|
|networkSourcePort|Int32|Origem da porta TCP.|
|url|Cadeia de caracteres|Localizador de Recursos Uniforme. Essa URL deve estar em conformidade com a RFC 1738.|
|userAgent|String|User-Agent cadeia de caracteres de uma solicitação da Web que pode indicar comprometimento.|

### <a name="diamondmodel-values"></a>valores de diamondModel

Para obter informações sobre esse modelo, consulte [o modelo de losango.](http://diamondmodel.org)

| Membro | Valor | Descrição |
|:-------|:----- |:------------|
| desconhecido |  0    | |
| adversário |  1     |O indicador descreve o adversário.|
| capability |  2    |Indicador é um recurso do adversário.|
| infrastructure | 3  |O indicador descreve a infraestrutura do adversário.|
| vítima | 4  |O indicador descreve a vítima do adversário.|
| unknownFutureValue | 127 | |

### <a name="killchain-values"></a>Valores killChain

| Member | Descrição |
|:-------|:------------|
|Ações|Indcates that the attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.|
|C2|Representa o canal de controle pelo qual um sistema comprometido é manipulado.|
|Entrega|O processo de distribuir o código de exploração para as vítima (por exemplo, USB, email, sites).|
|Exploração|O código de exploração aproveitando as vulnerabilidades (por exemplo, execução de código).|
|Instalação|Instalação de malware após uma vulnerabilidade ser explorada.|
|Reconhecimento|Indicador é a evidência de um grupo de atividades coletando informações a serem usadas em um ataque futuro.|
|Desorganização|Transformar uma vulnerabilidade em código de exploração (por exemplo, malware).|

### <a name="threattype-values"></a>valores threatType

| Member | Descrição |
|:-------|:------------|
|Botnet| O indicador está detalhando um nó/membro de botnet.|
|C2|O indicador está detalhando um nó command & Control de uma botnet.|
|CryptoMining|O tráfego que envolve esse endereço de rede/URL é uma indicação de CyrptoMining /Abuso de recursos.|
|Darknet|Indicador é o de um nó/rede Darknet.
|DDos|Indicadores relacionados a uma campanha DDoS ativa ou futura.|
|MaliciousUrl|URL que está servindo malware.|
|Malware|Indicador que descreve um arquivo ou arquivos mal-intencionados.|
|Phishing|Indicadores relacionados a uma campanha de phishing.|
|Proxy|Indicador é o de um serviço de proxy.|
|PUA|Aplicativo potencialmente indesejado.|
|WatchList|Esse é o bucket genérico no qual os indicadores são colocados quando não podem ser determinados exatamente qual é a ameaça ou exigirão interpretação manual. Isso normalmente não deve ser usado por parceiros que estão enviando dados para o sistema.|

### <a name="tlplevel-values"></a>Valores tlpLevel

Cada indicador também deve ter um valor do Protocolo semáforo quando enviado. Esse valor representa o escopo de sensibilidade e compartilhamento de um determinado indicador.

| Member | Descrição |
|:-------|:------------|
|Branco| Escopo de compartilhamento: Ilimitado. Os indicadores podem ser compartilhados livremente, sem restrições.|
|Verde| Escopo de compartilhamento: Comunidade. Os indicadores podem ser compartilhados com a comunidade de segurança.|
|Colore| Escopo de compartilhamento: Limitado. Essa é a configuração padrão para indicadores e restringe o compartilhamento apenas àqueles com um "precisa-saber" sendo 1) Serviços e operadores de serviço que implementam inteligência de ameaça 2) Clientes cujo(s) sistema(s) exibem comportamento consistente com o indicador.|
|Vermelho| Escopo de compartilhamento: Pessoal. Esses indicadores devem ser compartilhados apenas diretamente e, preferencialmente, pessoalmente. Normalmente, os indicadores TLP Red não são ingeridos devido às restrições pré-definidas. Se os indicadores TLP Red são enviados, a propriedade "PassiveOnly" deve ser definida `True` como também. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tiIndicator",
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