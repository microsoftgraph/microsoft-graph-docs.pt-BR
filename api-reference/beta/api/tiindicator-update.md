---
title: Atualizar tiIndicator
description: Atualize as propriedades de um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: f10370177565a1cbd92fad29bc1547bc042cc7b6
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786303"
---
# <a name="update-tiindicator"></a>Atualizar tiIndicator

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto tiIndicator.](../resources/tiindicator.md)

## <a name="permissions"></a>Permissions

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

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados. Os campos necessários são: `id` , `expirationDateTime` , `targetProduct` .

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ação|cadeia de caracteres| A ação a ser aplicada se o indicador for matched de dentro da ferramenta de segurança targetProduct. Os valores possíveis são: `unknown`, `allow`, `block`, `alert`.|
|activityGroupNames|Coleção de cadeias de caracteres|Os nomes(s) de inteligência de ameaças cibernéticas para as partes responsáveis pela atividade mal-intencionada coberta pelo indicador de ameaça.|
|additionalInformation|String|Uma área de catchall na qual os dados extras do indicador não cobertos pelas outras propriedades tiIndicator podem ser colocados. Os dados colocados em additionalInformation normalmente não serão usados pela ferramenta de segurança targetProduct.|
|confidence|Int32|Um inteiro que representa a confiança dos dados no indicador identifica com precisão comportamento mal-intencionado. Os valores aceitáveis são 0 – 100 com 100 sendo os mais altos.|
|description|String|Breve descrição (100 caracteres ou menos) da ameaça representada pelo indicador.|
|diamondModel|[diamondModel](../resources/tiindicator.md#diamondmodel-values)|A área do Modelo de Diamante na qual esse indicador existe. Os valores possíveis são: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| Cadeia de caracteres DateTime indicando quando o Indicador expira. Todos os indicadores devem ter uma data de expiração para evitar que os indicadores de stale persistam no sistema. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.|
|externalId|Cadeia de caracteres|Um número de identificação que vincula o indicador ao sistema do provedor de indicadores (por exemplo, uma chave estrangeira).|
|isActive|Booliano|Usado para desativar indicadores dentro do sistema. Por padrão, qualquer indicador enviado é definido como ativo. No entanto, os provedores podem enviar indicadores existentes com esse conjunto como "False" para desativar indicadores no sistema.|
|killChain|[Coleção killChain](../resources/tiindicator.md#killchain-values)|Uma matriz JSON de cadeias de caracteres que descreve qual ponto ou pontos na Cadeia de Kill esse indicador tem como destino. Consulte "valores killChain" abaixo para saber os valores exatos.|
|knownFalsePositives|String|Cenários em que o indicador pode causar falsos positivos. Este deve ser um texto aceitável para humanos.|
|lastReportedDateTime|DateTimeOffset|A última vez que o indicador foi visto. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`|
|malwareFamilyNames|Coleção de cadeias de caracteres|O nome da família de malware associado a um indicador se ele existir. A Microsoft prefere o nome da família de malware da Microsoft, se possível, o que pode ser encontrado por meio da Windows Defender de ameaças [do](https://www.microsoft.com/wdsi/threats)Security Intelligence.|
|passiveOnly|Booliano|Determina se o indicador deve disparar um evento visível para um usuário final. Quando definida como "true", as ferramentas de segurança não notificarão o usuário final de que ocorreu um "acerto". Isso é tratado com mais frequência como modo de auditoria ou silencioso pelos produtos de segurança, onde eles simplesmente registrarão que ocorreu uma combinação, mas não executarão a ação. O valor padrão é falso.|
|severity|Int32|Um inteiro que representa a gravidade do comportamento mal-intencionado identificado pelos dados dentro do indicador. Os valores aceitáveis são 0 – 5, onde 5 é o mais grave e zero não é grave. O valor padrão é 3.|
|categorias|Coleção de cadeias de caracteres|Uma matriz JSON de cadeias de caracteres que armazena marcas/palavras-chave arbitrárias.|
|tlpLevel|[tlpLevel](../resources/tiindicator.md#tlplevel-values)| Valor do Protocolo de Semáforo para o indicador. Os valores possíveis são: `unknown`, `white`, `green`, `amber`, `red`.|


## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`.

Se o header de solicitação opcional for usado, o método retornará um código de resposta e o objeto `200 OK` [tiIndicator](../resources/tiindicator.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-request-without-prefer-header"></a>Exemplo 1: Solicitar sem o header Prefer

#### <a name="request"></a>Solicitação

A seguir, um exemplo da solicitação sem `Prefer` o header.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>Exemplo 2: Solicitar com o header Prefer

#### <a name="request"></a>Solicitação

A seguir, um exemplo da solicitação que inclui o `Prefer` header.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator_2"
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> [!NOTE]
> O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.

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


