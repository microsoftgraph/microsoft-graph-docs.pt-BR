---
title: Tipo de recurso bookingBusiness
description: Representa uma empresa no Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: ccafc23fc8a1276ec7ffa9df4b0b2c8769142e32
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856292"
---
# <a name="bookingbusiness-resource-type"></a>Tipo de recurso bookingBusiness

Namespace: microsoft.graph

Representa uma empresa no Microsoft Bookings. Esse é o objeto de nível superior na API de Microsoft Bookings. Ele contém informações comerciais e objetos de negócios relacionados, como compromissos, clientes, serviços e membros da equipe.

## <a name="methods"></a>Métodos

| Método  | Tipo de retorno |Descrição|
|:---------------|:--------|:----------|
|[Listar bookingBusinesses](../api/bookingbusiness-list.md) | [coleção bookingBusiness](bookingbusiness.md) |Obtenha uma coleção de **objetos bookingBusiness** no locatário. |
|[Criar bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | Crie um novo Microsoft Bookings negócios. |
|[Obter bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |Ler propriedades e relações de um **objeto bookingBusiness** .|
|[Atualização](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |Atualize as propriedades em **um objeto bookingBusiness** . |
|[Delete](../api/bookingbusiness-delete.md) | Nenhum |Exclua **um objeto bookingBusiness** . |
|[Criar bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| Crie um novo **bookingAppointment** postando na coleção de compromissos.|
|[Listar compromissos](../api/bookingbusiness-list-appointments.md) |[coleção bookingAppointment](bookingappointment.md)| Obtenha uma coleção **de objetos bookingAppointment** .|
|[Criar bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| Crie um **novo bookingCustomer** postando na coleção de clientes.|
|[Listar clientes](../api/bookingbusiness-list-customers.md) |[coleção bookingCustomer](bookingcustomer.md)| Obtenha uma **coleção de objetos bookingCustomer** .|
|[Criar bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| Crie um novo **bookingService** postando na coleção de serviços.|
|[Listar serviços](../api/bookingbusiness-list-services.md) |[coleção bookingService](bookingservice.md)| Obtenha uma coleção **de objetos bookingService** .|
|[Criar bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| Crie um **novo bookingStaffMember** postando na coleção staffMembers.|
|[Listar staffMembers](../api/bookingbusiness-list-staffmembers.md) |[coleção bookingStaffMember](bookingstaffmember.md)| Obtenha uma **coleção de objetos bookingStaffMember** .|
|[Listar customQuestions](../api/bookingbusiness-list-customquestions.md)|[coleção bookingCustomQuestion](../resources/bookingcustomquestion.md)|Obtenha os **recursos bookingCustomQuestion** da **propriedade de navegação customQuestions** .|
|[Criar bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md)|[bookingCustomQuestion](../resources/bookingcustomquestion.md)|Crie um novo **objeto bookingCustomQuestion** .|
|[Listar calendarView](../api/bookingbusiness-list-calendarview.md)|[coleção bookingAppointment](bookingappointment.md)|Obtenha a coleção de **objetos bookingAppointment** que ocorre no intervalo de datas especificado.|
|[Publish](../api/bookingbusiness-publish.md)|Nenhum|Dispobilize a página de agendamento dessa empresa para clientes externos. Defina **a propriedade isPublished** como `true`, e **a propriedade publicUrl** como a URL da página de agendamento.|
|[Unpublish](../api/bookingbusiness-unpublish.md)|Nenhum| Torne a página de agendamento dessa empresa não disponível para clientes externos. Defina **a propriedade isPublished** como `false`, e **a propriedade publicUrl** como `null`.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|O endereço da empresa. A **propriedade** de endereço, juntamente **com telefone** **e webSiteUrl**, aparece no rodapé de uma página de agendamento de negócios. Não há **suporte** para o tipo de atributo physicalAddress na v1.0. Internamente, mapearemos os endereços para o tipo `others`.|
|businessHours|[coleção bookingWorkHours](bookingworkhours.md)|As horas de operação para os negócios.|
|businessType|Cadeia de caracteres|O tipo de negócio.|
|defaultCurrencyIso|Cadeia de caracteres|O código para a moeda na qual a empresa opera Microsoft Bookings.|
|displayName|Cadeia de caracteres|O nome da empresa, que se interface com os clientes. Esse nome aparece na parte superior da página de agendamento de negócios.|
|email|Cadeia de caracteres|O endereço de email da empresa.|
|id|Cadeia de caracteres|Um identificador programático exclusivo para a empresa. Somente leitura.|
|isPublished|Booliano|A página de agendamento foi disponibilizada para clientes externos. Use as **ações publicar** **e cancelar a publicação** para definir essa propriedade. Somente leitura.|
|phone|Cadeia de caracteres|O número de telefone da empresa. A **propriedade** de telefone, **juntamente com o endereço** e **WebSiteUrl**, aparece no rodapé de uma página de agendamento de negócios.|
|publicUrl|Cadeia de caracteres|A URL da página de agendamento, que é definida depois que você [publica ou cancela a publicação](../api/bookingbusiness-unpublish.md) da página.[](../api/bookingbusiness-publish.md) Somente leitura.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Especifica como as reservas podem ser criadas para essa empresa.|
|webSiteUrl|Cadeia de caracteres|A URL do site de negócios. A **propriedade webSiteUrl** , juntamente com **endereço**, **telefone**, aparece no rodapé de uma página de agendamento de negócios.|

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appointments|[coleção bookingAppointment](bookingappointment.md)| Todos os compromissos deste negócio. Somente leitura. Anulável.|
|calendarView|[coleção bookingAppointment](bookingappointment.md)| O conjunto de compromissos dessa empresa em um intervalo de datas especificado. Somente leitura. Anulável.|
|Clientes|[coleção bookingCustomer](bookingcustomer.md)| Todos os clientes deste negócio. Somente leitura. Anulável.|
|customQuestions|[coleção bookingCustomQuestion](../resources/bookingcustomquestion.md)| Todas as perguntas personalizadas deste negócio. Somente leitura. Anulável.|
|Serviços|[coleção bookingService](bookingservice.md)| Todos os serviços oferecidos por essa empresa. Somente leitura. Anulável.|
|staffMembers|[coleção bookingStaffMember](bookingstaffmember.md)| Todos os membros da equipe que fornecem serviços neste negócio. Somente leitura. Anulável.|

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


