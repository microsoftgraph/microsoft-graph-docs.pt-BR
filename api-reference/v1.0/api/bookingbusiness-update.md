---
title: Atualizar bookingbusiness
description: Atualize as propriedades de um objeto bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 2ff072b07a3d1812f9fc80954507020d5be4eef1
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526456"
---
# <a name="update-bookingbusiness"></a>Atualizar bookingbusiness

Namespace: microsoft.graph

Atualize as propriedades de um [objeto bookingBusiness.](../resources/bookingbusiness.md)
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
PATCH /bookingBusinesses/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:-----------|
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|[physicalAddress](../resources/physicaladdress.md)|O endereço da rua do negócio. O tipo **de** atributo physicalAddress não é suportado em v1.0. Internamente, mapeemos os endereços para o tipo `others` .|
|businessHours|[Coleção bookingWorkHours](../resources/bookingworkhours.md)|Os horários de operação para os negócios.|
|businessType|Cadeia de caracteres|O tipo de negócio.|
|defaultCurrencyIso|Cadeia de caracteres|O código da moeda em que a empresa opera no Microsoft Bookings.|
|displayName|Cadeia de caracteres|Um nome para a empresa que faz interface com os clientes.|
|email|Cadeia de caracteres|O endereço de email da empresa.|
|phone|Cadeia de caracteres|O número de telefone da empresa.|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|Especifica como as reservas podem ser criadas para essa empresa.|
|webSiteUrl|Cadeia de caracteres|A URL do site comercial.|

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.
## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
O exemplo a seguir atualiza o endereço de email comercial e a política de agendamento, para alterar o intervalo de tempo de reserva padrão da empresa para uma hora e avançar a reserva até 30 dias.

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/fabrikam@contoso.onmicrosoft.com
Content-type: application/json

{
  "email": "admin@fabrikam.com",
  "schedulingPolicy": {
      "timeSlotInterval": "PT60M",
      "minimumLeadTime": "P1D",
      "maximumAdvance": "P30D",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
  }
}
```

### <a name="response"></a>Resposta
Eis um exemplo da resposta. Observação: o objeto de resposta exibido aqui pode ser reduzido para facilitar a leitura.
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
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


