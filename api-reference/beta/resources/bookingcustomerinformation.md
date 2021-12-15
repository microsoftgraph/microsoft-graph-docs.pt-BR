---
title: tipo de recurso bookingCustomerInformation
description: Registra as propriedades do cliente para um compromisso. Um compromisso contém uma lista de informações do cliente e cada unidade indica as propriedades de um cliente que faz parte desse compromisso.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d72f54794cc637e7cb90a2f11b59cc2cb026d7ed
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525595"
---
# <a name="bookingcustomerinformation-resource-type"></a>tipo de recurso bookingCustomerInformation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Registra as propriedades do cliente para um compromisso. Um compromisso contém uma lista de informações do cliente e cada unidade indica as propriedades de um cliente que faz parte desse compromisso.

Herda de [bookingCustomerInformationBase](bookingcustomerinformationbase.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|customerId|Cadeia de caracteres|A ID do [bookingCustomer](../resources/bookingcustomer.md) para esse compromisso. Se nenhuma ID for especificada quando um compromisso for criado, um novo **objeto bookingCustomer** será criado. Depois de definido, você deve considerar o customerId imutável. |
|customQuestionAnswers|[coleção bookingQuestionAnswer](../resources/bookingquestionanswer.md)|Ele consiste na lista de perguntas e respostas personalizadas fornecidas pelo cliente como parte do compromisso. |
|emailAddress|String| O endereço SMTP do **bookingCustomer** que está reservando o compromisso. |
|location|[location](../resources/location.md)| Representa informações de local para **o bookingCustomer** que está reservando o compromisso. |
|nome|Cadeia de caracteres|O nome do cliente. |
|notes|String|Observações do cliente associado a esse compromisso. Você só pode obter o valor ao ler **esse bookingAppointment** por sua ID. Você só pode definir essa propriedade ao criar um compromisso com um novo cliente inicialmente. Após esse ponto, o valor é calculado do cliente representado pelo **customerId**. |
|phone|Cadeia de caracteres|O número de telefone do cliente. |
|timeZone|Cadeia de caracteres|O fuso horário do cliente. Para uma lista de valores possíveis, consulte [dateTimeTimeZone](../resources/datetimetimezone.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingCustomerInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingCustomerInformation",
  "customerId": "String",
  "name": "String",
  "emailAddress": "String",
  "phone": "String",
  "notes": "String",
  "location": {
    "@odata.type": "microsoft.graph.location"
  },
  "timeZone": "String",
  "customQuestionAnswers": [
    {
      "@odata.type": "microsoft.graph.bookingQuestionAnswer"
    }
  ]
}
```

