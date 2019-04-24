---
title: Atualizar alerta
description: Atualize uma propriedade de alerta editável em qualquer solução integrada para manter o status e as atribuições de alerta em sincronia entre soluções.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b1fec6bfca2ce116bc35c4a7c8a115418b15012
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459217"
---
# <a name="update-alert"></a>Atualizar alerta

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize uma propriedade de **alerta** editável em qualquer solução integrada para manter o status e as atribuições de alerta em sincronia entre soluções. Este método atualiza qualquer solução que tenha um registro da ID de alerta referenciada.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |   SecurityEvents.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

> **Observação:** Você deve incluir a ID do **alerta** como um parâmetro e vendorInformation contendo `provider` o `vendor` e com esse método.
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Authorization  | Portador {código}. Obrigatório.|
|Preferir | Return = representação |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON dos valores de campos relevantes que devem ser atualizados. O corpo **deve** conter a `vendorInformation` Propriedade com os `provider` campos `vendor` válidos e. A tabela a seguir lista os campos que podem ser atualizados para um alerta. Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|assignedTo|String|Nome do analista ao qual o alerta é atribuído para a triagem, investigação ou correção.|
|closedDateTime|DateTimeOffset|Tempo em que o alerta foi fechado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|comentários|Coleção de cadeias de caracteres|Comentários de analista sobre o alerta (para o gerenciamento de alerta do cliente).|
|comentários|Enumeração alertFeedback|Comentários do analista no alerta. Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|Enumeração alertStatus|Status do ciclo de vida de alerta (estágio). Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.|
|tags|String collection|Rótulos definíveis pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "vimos).|
|vendorInformation |[securityVendorInformation](../resources/securityvendorinformation.md)|Tipo complexo que contém detalhes sobre o fornecedor, provedor e subprovedor de produtos / serviços de segurança (por exemplo, fornecedor = Microsoft; provedor = Windows Defender ATP; subProvedor = AppLocker). **Os campos Provider e Vendor são necessários.**|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [Alert](../resources/alert.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-request-without-prefer-header"></a>Exemplo 1: solicitação sem cabeçalho de preferência

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo da solicitação sem `Prefer` cabeçalho.
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Resposta

Veja a seguir o exemplo de uma resposta bem-sucedida.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>Exemplo 2: solicitação com cabeçalho preferencial

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação que inclui `Prefer` o cabeçalho da solicitação.

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta quando o cabeçalho de `Prefer: return=representation` solicitação opcional é usado.

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
