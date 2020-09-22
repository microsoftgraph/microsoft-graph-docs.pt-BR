---
title: tipo de recurso bookingBusiness
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3d33c182fb2456137193f01bb1d2b9a310184160
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071798"
---
# <a name="bookingbusiness-resource-type"></a>tipo de recurso bookingBusiness

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa uma empresa em Microsoft bookings. Este é o objeto de nível superior na API do Microsoft bookings. Ele contém informações comerciais e objetos corporativos relacionados, como compromissos, clientes, serviços e membros da equipe.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar bookingBusinesses](../api/bookingbusiness-list.md) | coleção [bookingBusiness](bookingbusiness.md) |Obtenha uma coleção de objetos bookingbusiness no locatário. |
|[Criar bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | Crie uma nova empresa de livros da Microsoft. |
|[Obter bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |Leia as propriedades e os relacionamentos do objeto bookingBusiness.|
|[Update](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |Atualize as propriedades em um objeto **bookingBusiness** . |
|[Delete](../api/bookingbusiness-delete.md) | Nenhum |Excluir um objeto **bookingBusiness** . |
|[Criar bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| Crie um novo bookingAppointment postando na coleção de compromissos.|
|[Listar compromissos](../api/bookingbusiness-list-appointments.md) |coleção [bookingAppointment](bookingappointment.md)| Obtenha uma coleção de objetos bookingAppointment.|
|[Criar bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| Crie um novo bookingCustomer postando na coleção Customers.|
|[Listar clientes](../api/bookingbusiness-list-customers.md) |coleção [bookingCustomer](bookingcustomer.md)| Obtenha uma coleção de objetos bookingCustomer.|
|[Criar bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| Crie um novo bookingService postando na coleção de serviços.|
|[Listar serviços](../api/bookingbusiness-list-services.md) |coleção [bookingService](bookingservice.md)| Obtenha uma coleção de objetos bookingService.|
|[Criar bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| Crie um novo bookingStaffMember postando na coleção staffMembers.|
|[Listar staffMembers](../api/bookingbusiness-list-staffmembers.md) |coleção [bookingStaffMember](bookingstaffmember.md)| Obtenha uma coleção de objetos bookingStaffMember.|
|[Listar calendarView](../api/bookingbusiness-list-calendarview.md)|coleção [bookingAppointment](bookingappointment.md)|Obtenha a coleção de objetos **bookingAppointment** que ocorre no intervalo de datas especificado.|
|[publish](../api/bookingbusiness-publish.md)|Nenhum|Tornar a página de agendamento dessa empresa disponível para clientes externos. Defina a propriedade **IsPublished** como true e a propriedade **PUBLICURL** para a URL da página de agendamento.|
|[unpublish](../api/bookingbusiness-unpublish.md)|Nenhum| Tornar a página de agendamento dessa empresa não disponível para clientes externos. Defina a propriedade **IsPublished** como false e a propriedade **publicUrl** como NULL.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|O endereço da empresa. A propriedade **Address** , junto com **Phone** e **webSiteUrl**, aparecem no rodapé de uma página de agendamento de negócios.|
|businessHours|coleção [bookingWorkHours](bookingworkhours.md)|As horas de operação da empresa.|
|businesstype|Cadeia de caracteres|O tipo de negócio.|
|defaultCurrencyIso|Cadeia de caracteres|O código da moeda na qual a empresa opera em reservas da Microsoft.|
|displayName|Cadeia de caracteres|O nome da empresa, que é a interface com os clientes. Esse nome aparece na parte superior da página agendamento de negócios.|
|email|Cadeia de caracteres|O endereço de email da empresa.|
|id|Cadeia de caracteres|Um identificador de programação exclusivo para a empresa. Somente leitura.|
|isPublished|Booliano|A página de agendamento foi disponibilizada para clientes externos. Use as ações **publicar** e cancelar **publicação** para definir essa propriedade. Somente leitura.|
|phone|Cadeia de caracteres|O número de telefone da empresa. A propriedade **Phone** , junto com **endereço** e **webSiteUrl**, aparecem no rodapé de uma página de agendamento de negócios.|
|publicUrl|Cadeia de caracteres|A URL da página de agendamento, que é definida depois que você [publica](../api/bookingbusiness-publish.md) ou cancela a [publicação](../api/bookingbusiness-unpublish.md) da página. Somente leitura.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Especifica como as reservas podem ser criadas para essa empresa.|
|webSiteUrl|Cadeia de caracteres|A URL do site da empresa. A propriedade **webSiteUrl** , junto com **endereço**, **telefone**, aparece no rodapé de uma página de agendamento de negócios.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appointments|coleção [bookingAppointment](bookingappointment.md)| Todos os compromissos dessa empresa. Somente leitura. Anulável.|
|calendarView|coleção [bookingAppointment](bookingappointment.md)| O conjunto de compromissos dessa empresa em um intervalo de datas especificado. Somente leitura. Anulável.|
|Eles|coleção [bookingCustomer](bookingcustomer.md)| Todos os clientes desse negócio. Somente leitura. Anulável.|
|serviço|coleção [bookingService](bookingservice.md)| Todos os serviços oferecidos por essa empresa. Somente leitura. Anulável.|
|staffMembers|coleção [bookingStaffMember](bookingstaffmember.md)| Todos os membros da equipe que fornecem serviços neste negócio. Somente leitura. Anulável.|

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


