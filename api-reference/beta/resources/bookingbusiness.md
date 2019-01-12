---
title: tipo de recurso de bookingBusiness
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cf00239802cec9a705c24548649e38f3022383a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986212"
---
# <a name="bookingbusiness-resource-type"></a>tipo de recurso de bookingBusiness

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.
 
Representa uma empresa no Microsoft Bookings. Esse é o objeto de nível superior na API Microsoft reservas. Ele contém informações comerciais e objetos de negócios relacionados, como compromissos, os clientes, serviços e membros da equipe.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista bookingBusinesses](../api/bookingbusiness-list.md) | coleção [bookingBusiness](bookingbusiness.md) |Obtenha uma coleção de objetos bookingbusiness no inquilino. |
|[Criar bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | Crie um novo negócio Bookings Microsoft. |
|[Obter bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |Leia as propriedades e os relacionamentos do objeto bookingBusiness.|
|[Update](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |Atualize propriedades em um objeto **bookingBusiness** . |
|[Delete](../api/bookingbusiness-delete.md) | Nenhum |Exclua um objeto **bookingBusiness** . |
|[Criar bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| Crie um novo bookingAppointment pelo lançamento para o conjunto de compromissos.|
|[Lista de compromissos](../api/bookingbusiness-list-appointments.md) |coleção [bookingAppointment](bookingappointment.md)| Obtenha uma coleção de objetos bookingAppointment.|
|[Criar bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| Crie um novo bookingCustomer pelo lançamento à coleção de clientes.|
|[Clientes de lista](../api/bookingbusiness-list-customers.md) |coleção [bookingCustomer](bookingcustomer.md)| Obtenha uma coleção de objetos bookingCustomer.|
|[Criar bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| Crie um novo bookingService pelo lançamento para o conjunto de serviços.|
|[Lista de serviços](../api/bookingbusiness-list-services.md) |coleção [bookingService](bookingservice.md)| Obtenha uma coleção de objetos bookingService.|
|[Criar bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| Crie um novo bookingStaffMember pelo lançamento à coleção staffMembers.|
|[Lista staffMembers](../api/bookingbusiness-list-staffmembers.md) |coleção [bookingStaffMember](bookingstaffmember.md)| Obtenha uma coleção de objetos bookingStaffMember.|
|[Listar calendarView](../api/bookingbusiness-list-calendarview.md)|coleção [bookingAppointment](bookingappointment.md)|Obter a coleção de objetos **bookingAppointment** que ocorra no intervalo de datas especificado.|
|[Publicar](../api/bookingbusiness-publish.md)|Nenhum|Página de agendamento dessa empresa torne disponíveis para clientes externos. Defina a propriedade **isPublished** como true e a propriedade **publicUrl** para a URL da página de agendamento.|
|[cancelamento de publicação](../api/bookingbusiness-unpublish.md)|Nenhum| Verifique a página de agendamento dessa empresa não está disponível para clientes externos. Defina a propriedade **isPublished** como false e a propriedade **publicUrl** como nulo.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|O endereço da empresa. A propriedade **address** , juntamente com o **telefone** e **webSiteUrl**, aparecem no rodapé de um página de agendamento de negócios.|
|businessHours|coleção [bookingWorkHours](bookingworkhours.md)|Os horários de operação para a empresa.|
|businessType|Cadeia de caracteres|O tipo de negócio.|
|defaultCurrencyIso|Cadeia de caracteres|O código para a moeda que a empresa opera em Microsoft Bookings.|
|displayName|Cadeia de caracteres|O nome da empresa, interfaces com os clientes. Esse nome é exibido na parte superior do negócio o agendamento de página.|
|email|Cadeia de caracteres|O endereço de email para a empresa.|
|id|Cadeia de caracteres|Um identificador programático exclusivo para a empresa. Somente leitura.|
|isPublished|Booliano|A página de agendamento tenha sido disponibilizada para clientes externos. Use as ações de **Publicar** e **cancelamento de publicação** para definir essa propriedade. Somente leitura.|
|phone|Cadeia de caracteres|O número de telefone para a empresa. A propriedade de **telefone** , junto com o **endereço** e **webSiteUrl**, aparecem no rodapé de um página de agendamento de negócios.|
|publicUrl|Cadeia de caracteres|A URL para a página de agendamento, que é definida após você [Publicar](../api/bookingbusiness-publish.md) ou [Cancelar a publicação](../api/bookingbusiness-unpublish.md) de página. Somente leitura.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Especifica como reservas podem ser criadas para esta empresa.|
|webSiteUrl|Cadeia de caracteres|A URL do site da web de negócios. A propriedade de **webSiteUrl** , o **endereço**, **telefone**, aparecem no rodapé de uma página de agendamento de negócios.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appointments|coleção [bookingAppointment](bookingappointment.md)| Todos os compromissos essa empresa. Somente leitura. Anulável.|
|calendarView|coleção [bookingAppointment](bookingappointment.md)| O conjunto de compromissos deste negócio em um intervalo de datas especificado. Somente leitura. Anulável.|
|clientes|coleção [bookingCustomer](bookingcustomer.md)| Todos os clientes desse negócio. Somente leitura. Anulável.|
|serviços|coleção [bookingService](bookingservice.md)| Todos os serviços oferecidos por essa empresa. Somente leitura. Anulável.|
|staffMembers|coleção [bookingStaffMember](bookingstaffmember.md)| Todos os membros da equipe que fornecem serviços nesse negócio. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
