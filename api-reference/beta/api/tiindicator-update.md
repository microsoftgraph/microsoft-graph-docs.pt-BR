---
title: Atualizar tiIndicator
description: Atualiza as propriedades de um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 0efdf8309d2e277c473c099f869ee35b463004f9
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409286"
---
# <a name="update-tiindicator"></a>Atualizar tiIndicator

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades de um objeto [tiIndicator](../resources/tiindicator.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | ThreatIndicators.ReadWrite.OwnedBy |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | ThreatIndicators.ReadWrite.OwnedBy |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | Portador {código} **obrigatório** |
|Preferir | Return = representação |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ação|string| A ação a ser aplicada se o indicador for correspondido de dentro da ferramenta de segurança do targetProduct. Os valores possíveis são: `unknown`, `allow`, `block`, `alert`.|
|activityGroupNames|Coleção de cadeias de caracteres|O nome do Cyber Threat Intelligence (s) para as partes responsáveis pela atividade mal-intencionada coberta pelo indicador de ameaças.|
|additionalInformation|String|Uma área catchall na qual os dados extras do indicador não cobertos pelas outras propriedades de tiIndicator podem ser colocados. Os dados colocados no additionalInformation normalmente não serão utilizados pela ferramenta de segurança do targetProduct.|
|confidence|Int32|Um inteiro representando a confiança dos dados dentro do indicador identifica precisamente o comportamento mal-intencionado. Os valores aceitáveis são 0 – 100 com 100 sendo os mais altos.|
|descrição|String|Breve descrição (100 caracteres ou menos) da ameaça representada pelo indicador.|
|diamondModel|[diamondModel](#diamondmodel-values)|A área do modelo em losango em que esse indicador existe. Os valores possíveis são: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| Cadeia de caracteres DateTime indicando quando o indicador expira. Todos os indicadores devem ter uma data de vencimento para evitar indicadores obsoletos persistentes no sistema. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.|
|externalId|Cadeia de caracteres|Um número de identificação que liga o indicador de volta para o sistema do provedor de indicadores (por exemplo, uma chave externa).|
|isActive|Booliano|Usado para desativar indicadores no sistema. Por padrão, qualquer indicador enviado é definido como ativo. No entanto, os provedores podem enviar indicadores existentes com este conjunto como ' false ' para desativar indicadores no sistema.|
|killChain|coleção [killChain](#killchain-values)|Uma matriz JSON de cadeias de caracteres que descreve o ponto ou os pontos na cadeia de Kill que este indicador aponta. Consulte "valores de killChain" abaixo para ver os valores exatos.|
|knownFalsePositives|String|Cenários nos quais o indicador pode causar falsos positivos. Isso deve ser um texto legível por pessoas.|
|lastReportedDateTime|DateTimeOffset|A última vez que o indicador foi visto. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`|
|malwareFamilyNames|Coleção de cadeias de caracteres|O nome da família de malware associado a um indicador, se existir. A Microsoft prefere o nome da família de malware da Microsoft, se possível, que possa ser encontrado por meio da [enciclopédia de ameaças](https://www.microsoft.com/wdsi/threats)de inteligência de segurança do Windows Defender.|
|passiveOnly|Booliano|Determina se o indicador deve acionar um evento que é visível para um usuário final. Quando definido como ' true ', as ferramentas de segurança não notificarão o usuário final de que um ' hit ' ocorreu. Isso geralmente é tratado como um modo de auditoria ou silencioso por produtos de segurança onde eles simplesmente farão o registro de que uma correspondência ocorreu, mas não executará a ação. O valor padrão é falso.|
|severity|Int32|Um inteiro que representa a gravidade do comportamento mal-intencionado identificado pelos dados dentro do indicador. Os valores aceitáveis são 0 – 5, onde 5 é o mais grave e zero não é grave. O valor padrão é 3.|
|marcações|String collection|Uma matriz JSON de cadeias de caracteres que armazena marcas arbitrárias/palavras-chave.|
|tlpLevel|[tlpLevel](#tlplevel-values)| Valor do protocolo de luz de tráfego para o indicador. Os valores possíveis são: `unknown`, `white`, `green`, `amber`, `red`.|

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
|Ações|Representa "ações nos objetivos". O invasor está aproveitando o sistema comprometido para realizar ações como um ataque de negação de serviço distribuído.|
|C2|Representa o canal de controle pelo qual um sistema comprometido é manipulado.|
|Entrega|O processo de distribuição do código de exploração para vítimas (por exemplo, USB, email, sites).|
|Invasão|O código de exploração que aproveita as vulnerabilidades (por exemplo, execução de código).|
|Instalação|Instalação de malware após uma vulnerabilidade ter sido explorada.|
|Reconhecimento|O indicador é uma evidência de um grupo de atividades que coleta informações a serem usadas em um ataque futuro.|
|Armas|Transformar uma vulnerabilidade em código de exploração (por exemplo, malware).|

### <a name="tlplevel-values"></a>valores de tlpLevel

Todos os indicadores devem ter um valor de protocolo de semáforo (TLP) quando ele é enviado. Esse valor representa a sensibilidade e o escopo de compartilhamento de um determinado indicador.

| Valores | Descrição |
|:-------|:------------|
|Branco| Escopo de compartilhamento: ilimitado. Os indicadores podem ser compartilhados livremente, sem restrição.|
|Verde| Escopo de compartilhamento: Comunidade. Os indicadores podem ser compartilhados com a comunidade de segurança.|
|Âmbar| Escopo de compartilhamento: limitado. Essa é a configuração padrão para indicadores e restringe o compartilhamento apenas àqueles que têm de ser conhecidos: 1) serviços e operadores de serviço que implementam inteligência de ameaças; 2) clientes cujos sistemas apresentam comportamento consistente com o indicador.|
|Vermelho| Escopo de compartilhamento: pessoal. Esses indicadores devem ser compartilhados apenas diretamente e, preferencialmente, em pessoa. Normalmente, os indicadores vermelhos do TLP não são incluídos devido às restrições predefinidas. Se TLP indicadores vermelhos forem enviados, a propriedade **passiveOnly** também deverá ser definida `True` como. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [tiIndicator](../resources/tiindicator.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-request-without-prefer-header"></a>Exemplo 1: solicitação sem cabeçalho de preferência

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo da solicitação sem `Prefer` cabeçalho.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>Exemplo 2: solicitação com cabeçalho preferencial

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo da solicitação que inclui o `Prefer` cabeçalho.

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> [!NOTE]
> O objeto de resposta mostrado aqui pode ser reduzido para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
