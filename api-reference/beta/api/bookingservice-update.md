---
title: Atualizar bookingservice
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: e39ad73b7f9acf2337db517e67895bc4601598a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035348"
---
# <a name="update-bookingservice"></a>Atualizar bookingservice

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.
 
Atualize as propriedades de um objeto de [bookingService](../resources/bookingservice.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).

Eis alguns exemplos que você pode personalizar para um serviço:
- Price
- Comprimento típico de um compromisso
- Reminders
- Buffer para definir antes ou término após o serviço a qualquer momento
- Parâmetros de [política de agendamento](../resources/bookingschedulingpolicy.md) , como mínimo de aviso do livro ou Cancelar, e se os clientes podem selecionar membros de equipe específico para um compromisso.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais
| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|defaultDuration|Duração|O comprimento padrão do serviço, representado em número de dias, horas, minutos e segundos. Por exemplo, P11D23H59M59.999999999999S. |
|defaultLocation|[location](../resources/location.md)|A localização física padrão para o serviço.|
|defaultPrice|Duplo|O preço monetários padrão para o serviço.|
|defaultPriceType|string|A maneira padrão de serviço é cobrada. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultReminders|coleção [bookingReminder](../resources/bookingreminder.md)|O padrão é definido de lembretes para um compromisso desse serviço. O valor dessa propriedade está disponível somente quando a ler este **bookingService** pela sua identificação.|
|description|String|Uma descrição de texto para o serviço.|
|displayName|String|Um nome de serviço.|
|emailAddress|String|Um endereço de email|
|id|String| Somente leitura.|
|isHiddenFromCustomers|Booliano|True significa que esse serviço não está disponível para os clientes de reserva.|
|Observações|String|Informações adicionais sobre esse serviço.|
|postBuffer|Duração|Encerra o tempo de buffer após um compromisso para este serviço e antes que a próxima compromisso do cliente pode ser agendado.|
|preBuffer|Duração|O tempo de buffer antes de um compromisso para esse serviço pode iniciar.|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|O conjunto de diretivas que determinam como compromissos para esse tipo de serviço devem ser criados e gerenciados.|
|staffMemberIds|String collection|Representa os [membros da equipe](../resources/bookingstaffmember.md) que forneça esse serviço. |

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O exemplo a seguir atualiza a duração do serviço especificado.
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a>Resposta
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
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->