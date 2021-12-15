---
title: Atualizar bookingservice
description: Atualize as propriedades de um objeto bookingService no bookingbusiness especificado.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e226e77717c048cc0e8001506a4b5b3a497aeccf
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525677"
---
# <a name="update-bookingservice"></a>Atualizar bookingservice

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto bookingService](../resources/bookingservice.md) no [bookingBusiness especificado.](../resources/bookingbusiness.md)

Veja a seguir alguns exemplos que você pode personalizar para um serviço:
- Price
- Tamanho típico de um compromisso
- Reminders
- Qualquer buffer de tempo para configurar antes ou concluir após o serviço
- [Os parâmetros de política](../resources/bookingschedulingpolicy.md) de agendamento, como aviso mínimo para reservar ou cancelar, e se os clientes podem selecionar membros específicos da equipe para um compromisso.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegada (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais
| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | {code} do portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|defaultDuration|Duração|O comprimento padrão do serviço, representado em números de dias, horas, minutos e segundos. Por exemplo, P11D23H59M59.99999999999S. |
|defaultLocation|[location](../resources/location.md)|O local físico padrão do serviço.|
|defaultPrice|Duplo|O preço monetário padrão do serviço.|
|defaultPriceType|bookingPriceType|A maneira padrão como o serviço é cobrado. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|defaultReminders|[Coleção bookingReminder](../resources/bookingreminder.md)|O conjunto padrão de lembretes para um compromisso desse serviço. O valor dessa propriedade está disponível somente ao ler este **bookingService** por sua ID.|
|description|Cadeia de caracteres|Uma descrição de texto para o serviço.|
|displayName|Cadeia de caracteres|Um nome de serviço.|
|id|String| Somente leitura.|
|isHiddenFromCustomers|Booliano|True significa que esse serviço não está disponível para os clientes para reserva.|
|isLocationOnline|Booliano|True indica que os compromissos do serviço serão mantidos online. O valor padrão é falso.|
|notes|String|Informações adicionais sobre esse serviço.|
|postBuffer|Duração|O tempo para buffer após o fim de um compromisso para esse serviço e antes que o próximo compromisso do cliente possa ser reservado.|
|preBuffer|Duração|O tempo para buffer antes que um compromisso para esse serviço possa começar.|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|O conjunto de políticas que determinam como os compromissos para esse tipo de serviço devem ser criados e gerenciados.|
|smsNotificationsEnabled|Booliano|True indica que as notificações de SMS podem ser enviadas aos clientes para o compromisso do serviço. O valor padrão é falso.|
|staffMemberIds|Coleção de cadeias de caracteres|Representa os [membros da equipe](../resources/bookingstaffmember.md) que fornecem esse serviço. |
|customQuestions|[coleção bookingQuestionAssignment](../resources/bookingquestionassignment.md)|Isso contém o conjunto de perguntas personalizadas associadas a um serviço específico. Opcional.|
|maximumAttendeesCount|Int32|O número máximo de clientes permitidos em um serviço.  |

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.
## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
O exemplo a seguir atualiza a duração do serviço especificado.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookingservice-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


