---
title: Atualizar bookingbusiness
description: Atualize as propriedades de um objeto bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 32c4901237c17429d3908607dffd186fc3919199
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160654"
---
# <a name="update-bookingbusiness"></a>Atualizar bookingbusiness

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto bookingBusiness](../resources/bookingbusiness.md) .
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}
```
## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais
| Nome       | Descrição|
|:-----------|:-----------|
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|[physicalAddress](../resources/physicaladdress.md)|O endereço da empresa.|
|businessHours|[coleção bookingWorkHours](../resources/bookingworkhours.md)|As horas de operação para os negócios.|
|businessType|Cadeia de Caracteres|O tipo de negócio.|
|defaultCurrencyIso|Cadeia de Caracteres|O código para a moeda na qual a empresa opera Microsoft Bookings.|
|displayName|Cadeia de caracteres|Um nome para a empresa que se interface com os clientes.|
|email|Cadeia de caracteres|O endereço de email da empresa.|
|languageTag|Cadeia de Caracteres|O idioma da página de reserva de autoatendimento.
|phone|Cadeia de caracteres|O número de telefone da empresa.|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|Especifica como as reservas podem ser criadas para essa empresa.|
|webSiteUrl|Cadeia de Caracteres|A URL do site de negócios.|

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O exemplo a seguir atualiza o endereço de email comercial e a política de agendamento, para alterar o intervalo de tempo de reserva padrão da empresa para uma hora e avançar a reserva de até 30 dias.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingbusiness"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@contoso.onmicrosoft.com
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookingbusiness-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-bookingbusiness-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
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


