---
title: Tipo de recurso bookingBusiness
description: Representa uma empresa no Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 76c08ab05575b1f0c52b7af21db787396e8dba63
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524823"
---
# <a name="bookingbusiness-resource-type"></a>Tipo de recurso bookingBusiness

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa uma empresa no Microsoft Bookings. Este é o objeto de nível superior na API do Microsoft Bookings. Ele contém informações comerciais e objetos de negócios relacionados, como compromissos, clientes, serviços e membros da equipe.

Herda de [bookingNamedEntity](bookingnamedentity.md)

## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar bookingBusinesses](../api/bookingbusiness-list.md) | [coleção bookingBusiness](bookingbusiness.md) |Obter uma coleção de objetos bookingbusiness no locatário. |
|[Criar bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | Crie uma nova empresa do Microsoft Bookings. |
|[Obter bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |Leia propriedades e relações do objeto bookingBusiness.|
|[Atualizar](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |Atualizar propriedades em um **objeto bookingBusiness.** |
|[Delete](../api/bookingbusiness-delete.md) | Nenhuma |**Exclua um objeto bookingBusiness.** |
|[Criar bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| Crie um novo bookingAppointment postando na coleção appointments.|
|[Listar compromissos](../api/bookingbusiness-list-appointments.md) |[coleção bookingAppointment](bookingappointment.md)| Obter uma coleção de objetos bookingAppointment.|
|[Criar bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| Crie um novo bookingCustomer postando na coleção customers.|
|[Listar clientes](../api/bookingbusiness-list-customers.md) |[coleção bookingCustomer](bookingcustomer.md)| Obter uma coleção de objetos bookingCustomer.|
|[Criar bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| Crie um novo bookingService postando na coleção de serviços.|
|[Listar serviços](../api/bookingbusiness-list-services.md) |[Coleção bookingService](bookingservice.md)| Obter uma coleção de objetos bookingService.|
|[Criar bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| Crie um novo bookingStaffMember postando na coleção staffMembers.|
|[Listar staffMembers](../api/bookingbusiness-list-staffmembers.md) |[coleção bookingStaffMember](bookingstaffmember.md)| Obter uma coleção de objetos bookingStaffMember.|
|[Listar customQuestions](../api/bookingbusiness-list-customquestions.md)|[coleção bookingCustomQuestion](../resources/bookingcustomquestion.md)|Obter os **recursos bookingCustomQuestion** da propriedade de navegação **customQuestions.**|
|[Criar bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md)|[bookingCustomQuestion](../resources/bookingcustomquestion.md)|Crie um novo **objeto bookingCustomQuestion.**|
|[Listar calendarView](../api/bookingbusiness-list-calendarview.md)|[coleção bookingAppointment](bookingappointment.md)|Obter a coleção **de objetos bookingAppointment** que ocorre no intervalo de datas especificado.|
|[publish](../api/bookingbusiness-publish.md)|Nenhuma|Disponibilizar a página de agendamento dessa empresa para clientes externos. Defina a **propriedade isPublished** como true e **a propriedade publicUrl** como a URL da página de agendamento.|
|[unpublish](../api/bookingbusiness-unpublish.md)|Nenhuma| Tornar a página de agendamento dessa empresa não disponível para clientes externos. Defina a **propriedade isPublished** como false e **a propriedade publicUrl** como null.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|O endereço da rua do negócio. A **propriedade** address, juntamente com **telefone** **e webSiteUrl**, aparece no rodapé de uma página de agendamento de negócios.|
|businessHours|[Coleção bookingWorkHours](bookingworkhours.md)|Os horários de operação para os negócios.|
|businessType|Cadeia de caracteres|O tipo de negócio.|
|defaultCurrencyIso|Cadeia de caracteres|O código da moeda em que a empresa opera no Microsoft Bookings.|
|displayName|Cadeia de caracteres|O nome da empresa, que faz interface com os clientes. Esse nome aparece na parte superior da página de agendamento de negócios.|
|email|Cadeia de caracteres|O endereço de email da empresa.|
|id|Cadeia de caracteres|Um identificador programático exclusivo para a empresa. Somente leitura.|
|isPublished|Booliano|A página de agendamento foi disponibilizada para clientes externos. Use as **ações publicar** e não **publicar para** definir essa propriedade. Somente leitura.|
|phone|Cadeia de caracteres|O número de telefone da empresa. A **propriedade** phone, juntamente **com endereço e** **webSiteUrl**, aparece no rodapé de uma página de agendamento de negócios.|
|publicUrl|Cadeia de caracteres|A URL da página de agendamento, que é definida após [publicar](../api/bookingbusiness-publish.md) ou [não publicar a](../api/bookingbusiness-unpublish.md) página. Somente leitura.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Especifica como as reservas podem ser criadas para essa empresa.|
|webSiteUrl|Cadeia de caracteres|A URL do site comercial. A **propriedade webSiteUrl,** juntamente com **endereço**, **telefone**, aparece no rodapé de uma página de agendamento de negócios.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appointments|[coleção bookingAppointment](bookingappointment.md)| Todos os compromissos dessa empresa. Somente leitura. Anulável.|
|calendarView|[coleção bookingAppointment](bookingappointment.md)| O conjunto de compromissos dessa empresa em um intervalo de datas especificado. Somente leitura. Anulável.|
|customers|[coleção bookingCustomer](bookingcustomer.md)| Todos os clientes dessa empresa. Somente leitura. Anulável.|
|customQuestions|[coleção bookingCustomQuestion](../resources/bookingcustomquestion.md)| Todas as perguntas personalizadas dessa empresa. Somente leitura. Anulável.|
|services|[Coleção bookingService](bookingservice.md)| Todos os serviços oferecidos por essa empresa. Somente leitura. Anulável.|
|staffMembers|[coleção bookingStaffMember](bookingstaffmember.md)| Todos os membros da equipe que fornecem serviços nesta empresa. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingBusiness"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}],
  "businessType": "String",
  "defaultCurrencyIso": "String",
  "displayName": "String",
  "email": "String",
  "id": "String (identifier)",
  "isPublished": true,
  "phone": "String",
  "publicUrl": "String",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "webSiteUrl": "String"
}
```

## <a name="see-also"></a>Confira também


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


