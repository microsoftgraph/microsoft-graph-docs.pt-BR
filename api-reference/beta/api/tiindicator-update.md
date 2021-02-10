---
title: Atualizar tiIndicator
description: Atualizar as propriedades de um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 3ded1ad2ac77cfd08320c54480de5dd24d319b91
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176952"
---
# <a name="update-tiindicator"></a>Atualizar tiIndicator

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar as propriedades de um [objeto tiIndicator.](../resources/tiindicator.md)

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
| Autorização | Portador {code} **Obrigatório** |
|Preferir | return=representation |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados. Os campos obrigatórios são: `id` , `expirationDateTime` . `targetProduct`

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ação|string| A ação a ser aplicada se o indicador for corresponder de dentro da ferramenta de segurança targetProduct. Os valores possíveis são: `unknown`, `allow`, `block`, `alert`.|
|activityGroupNames|Coleção de cadeias de caracteres|Os nomes de inteligência contra ameaças cibernéticas para as partes responsáveis pelas atividades mal-intencionadas cobertas pelo indicador de ameaças.|
|additionalInformation|Cadeia de caracteres|Uma área catchall na qual dados extras do indicador não cobertos pelas outras propriedades tiIndicator podem ser colocados. Os dados colocados em additionalInformation normalmente não serão utilizados pela ferramenta de segurança targetProduct.|
|confidence|Int32|Um inteiro que representa a confiança dos dados no indicador identifica com precisão o comportamento mal-intencionado. Os valores aceitáveis são de 0 a 100, sendo 100 o maior.|
|description|Cadeia de caracteres|Breve descrição (100 caracteres ou menos) da ameaça representada pelo indicador.|
|diamondModel|[diamondModel](../resources/tiindicator.md#diamondmodel-values)|A área do Modelo de Losango na qual esse indicador existe. Os valores possíveis são: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| Cadeia de caracteres DateTime que indica quando o Indicador expira. Todos os indicadores devem ter uma data de expiração para evitar que os indicadores persistentes persistam no sistema. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.|
|externalId|Cadeia de caracteres|Um número de identificação que vincula o indicador de volta ao sistema do provedor do indicador (por exemplo, uma chave estrangeira).|
|isActive|Booliano|Usado para desativar indicadores no sistema. Por padrão, qualquer indicador enviado é definido como ativo. No entanto, os provedores podem enviar indicadores existentes com esse conjunto como "Falso" para desativar os indicadores no sistema.|
|killChain|[Coleção killChain](../resources/tiindicator.md#killchain-values)|Uma matriz JSON de cadeias de caracteres que descreve qual ponto ou pontos no Kill Chain esse indicador se direciona. Consulte "valores killChain" abaixo para saber os valores exatos.|
|knownFalsePositives|Cadeia de caracteres|Cenários em que o indicador pode causar falsos positivos. Deve ser um texto acessível para humanos.|
|lastReportedDateTime|DateTimeOffset|A última vez em que o indicador foi visto. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`|
|malwareFamilyNames|Coleção de cadeias de caracteres|O nome da família de malware associado a um indicador, se ele existir. A Microsoft prefere o nome da família de malware da Microsoft, [](https://www.microsoft.com/wdsi/threats)se possível, que pode ser encontrado por meio da ameaça de inteligência de segurança do Windows Defender.|
|passiveOnly|Booliano|Determina se o indicador deve disparar um evento visível para um usuário final. Quando definido como "verdadeiro", as ferramentas de segurança não notificarão o usuário final de que ocorreu um 'acerto'. Isso é tratado com mais frequência como modo de auditoria ou silencioso por produtos de segurança, onde eles simplesmente registram que uma combinação ocorreu, mas não executarão a ação. O valor padrão é falso.|
|severity|Int32|Um inteiro que representa a gravidade do comportamento mal-intencionado identificado pelos dados dentro do indicador. Os valores aceitáveis são de 0 a 5, onde 5 é o mais grave e zero não é grave. O valor padrão é 3.|
|tags|Coleção de cadeias de caracteres|Uma matriz JSON de cadeias de caracteres que armazena marcas/palavras-chave arbitrárias.|
|tlpLevel|[tlpLevel](../resources/tiindicator.md#tlplevel-values)| Valor do Protocolo semáforo para o indicador. Os valores possíveis são: `unknown`, `white`, `green`, `amber`, `red`.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Se o header de solicitação opcional for usado, o método retornará um código de resposta e o objeto `200 OK` [tiIndicator](../resources/tiindicator.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-request-without-prefer-header"></a>Exemplo 1: Solicitação sem o header Prefer

#### <a name="request"></a>Solicitação

A seguir está um exemplo da solicitação sem `Prefer` o header.

# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-java-snippets.md)]
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

### <a name="example-2-request-with-prefer-header"></a>Exemplo 2: Solicitação com o header Prefer

#### <a name="request"></a>Solicitação

A seguir está um exemplo da solicitação que inclui `Prefer` o header.

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
> O objeto response mostrado aqui pode ser encurtado para maior leitura. Todas as propriedades serão retornadas de uma chamada real.

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


