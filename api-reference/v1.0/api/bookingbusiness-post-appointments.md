---
title: Criar bookingAppointment
description: Crie um novo bookingAppointment para o bookingBusiness especificado.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 84a91ac1e3bb289e085d8bc07a5094e41512eb4a
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856341"
---
# <a name="create-bookingappointment"></a>Criar bookingAppointment

Namespace: microsoft.graph

Crie um [novo bookingAppointment](../resources/bookingappointment.md) para o [bookingBusiness especificado](../resources/bookingbusiness.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | BookingsAppointment.ReadWrite.All, Bookings.Read.All  |

> [!NOTE]
> Se você criar um aplicativo personalizado usando permissões de aplicativo, deverá seguir a validação [de regras de negócios](/graph/bookingsbusiness-business-rules).

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /solutions/bookingBusinesses/{id}/appointments

```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {code} do portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um [objeto bookingAppointment](../resources/bookingappointment.md) .

Se o número máximo de clientes (**maximumAttedeesCount**) permitido no [serviço](../resources/bookingservice.md) for maior que 1:

- Verifique se os clientes existem no Calendário de Reserva. Caso contrário, crie usando a [operação Criar bookingCustomer](bookingbusiness-post-customers.md) .

- Passe as IDs de cliente válidas ao criar ou atualizar o compromisso. Se a ID do cliente não for válida, esse cliente não será incluído no objeto de compromisso.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `201 Created` de resposta e um [objeto bookingAppointment](../resources/bookingappointment.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Esse compromisso não envolve a reserva de membros específicos da equipe.

<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.bookingAppointment",
    "customerTimeZone": "America/Chicago",
    "smsNotificationsEnabled": true,
    "endDateTime": {
        "@odata.type": "#microsoft.graph.dateTimeTimeZone",
        "dateTime": "2018-05-01T12:30:00.0000000+00:00",
        "timeZone": "UTC"
    },
    "isLocationOnline": true,
    "optOutOfCustomerEmail": false,
    "postBuffer": "PT10M",
    "preBuffer": "PT5M",
    "price": 10.0,
    "priceType@odata.type": "#microsoft.graph.bookingPriceType",
    "priceType": "fixedPrice",
    "reminders@odata.type": "#Collection(microsoft.graph.bookingReminder)",
    "reminders": [
        {
            "@odata.type": "#microsoft.graph.bookingReminder",
            "message": "This service is tomorrow",
            "offset": "P1D",
            "recipients@odata.type": "#microsoft.graph.bookingReminderRecipients",
            "recipients": "allAttendees"
        },
        {
            "@odata.type": "#microsoft.graph.bookingReminder",
            "message": "Please be available to enjoy your lunch service.",
            "offset": "PT1H",
            "recipients@odata.type": "#microsoft.graph.bookingReminderRecipients",
            "recipients": "customer"
        },
        {
            "@odata.type": "#microsoft.graph.bookingReminder",
            "message": "Please check traffic for next cater.",
            "offset": "PT2H",
            "recipients@odata.type": "#microsoft.graph.bookingReminderRecipients",
            "recipients": "staff"
        }
    ],
    "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceLocation": {
        "@odata.type": "#microsoft.graph.location",
        "address": {
            "@odata.type": "#microsoft.graph.physicalAddress",
            "city": "Buffalo",
            "countryOrRegion": "USA",
            "postalCode": "98052",
            "postOfficeBox": null,
            "state": "NY",
            "street": "123 First Avenue",
            "type@odata.type": "#microsoft.graph.physicalAddressType",
            "type": null
        },
        "coordinates": null,
        "displayName": "Customer location",
        "locationEmailAddress": null,
        "locationType@odata.type": "#microsoft.graph.locationType",
        "locationType": null,
        "locationUri": null,
        "uniqueId": null,
        "uniqueIdType@odata.type": "#microsoft.graph.locationUniqueIdType",
        "uniqueIdType": null
    },
    "serviceName": "Catered bento",
    "serviceNotes": "Customer requires punctual service.",
    "startDateTime": {
        "@odata.type": "#microsoft.graph.dateTimeTimeZone",
        "dateTime": "2018-05-01T12:00:00.0000000+00:00",
        "timeZone": "UTC"
    },
    "maximumAttendeesCount": 5,
    "filledAttendeesCount": 1,
    "customers@odata.type": "#Collection(microsoft.graph.bookingCustomerInformation)",
    "customers": [
        {
            "@odata.type": "#microsoft.graph.bookingCustomerInformation",
            "customerId": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "name": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com",
            "phone": "213-555-0199",
            "notes": null,
            "location": {
                "@odata.type": "#microsoft.graph.location",
                "displayName": "Customer",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "@odata.type": "#microsoft.graph.physicalAddress",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "timeZone":"America/Chicago",
            "customQuestionAnswers": [
                {
                    "questionId": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
                    "question": "What is your age?",
                    "answerInputType": "text",
                    "answerOptions": [],
                    "isRequired": true,
                    "answer": "25",
                    "selectedOptions": []
                }
            ]
        }
    ]
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses('Contosolunchdelivery%40contoso.onmicrosoft.com')/appointments/$entity",
    "id": "AAMkADc7zF4J0AAA8v_KnAAA=",
    "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
    "isLocationOnline": true,
    "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MTlhZTE3MDUtODk0Yy00MGZkLTlhNzktN2FmYTk3MDUxNmE2%40thread.v2/0?context=%7b%22Tid%22%3a%22995fa18c-b557-4694-8d07-b89779d6dc77%22%2c%22Oid%22%3a%22d4d260ab-989d-490e-b121-e2066391807a%22%7d",
    "smsNotificationsEnabled": true,
    "customerTimeZone": "America/Chicago",
    "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceName": "Catered bento",
    "duration": "PT30M",
    "preBuffer": "PT5M",
    "postBuffer": "PT10M",
    "priceType": "fixedPrice",
    "price": 10,
    "serviceNotes": "Customer requires punctual service.",
    "optOutOfCustomerEmail": false,
    "staffMemberIds": [],
    "startDateTime": {
        "dateTime": "2018-05-01T12:00:00.0000000Z",
        "timeZone": "UTC"
    },
    "endDateTime": {
        "dateTime": "2018-05-01T12:30:00.0000000Z",
        "timeZone": "UTC"
    },
    "serviceLocation": {
        "displayName": "Customer location (123 First Avenue, Buffalo, NY 98052, USA)",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "street": "",
            "city": "",
            "state": "",
            "countryOrRegion": "",
            "postalCode": ""
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "reminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "This service is tomorrow"
        },
        {
            "offset": "PT1H",
            "recipients": "customer",
            "message": "Please be available to enjoy your lunch service."
        },
        {
            "offset": "PT2H",
            "recipients": "staff",
            "message": "Please check traffic for next cater."
        }
    ],
    "maximumAttendeesCount": 5,
    "filledAttendeesCount": 1,
    "customers": [
        {
            "@odata.type": "#microsoft.graph.bookingCustomerInformation",
            "customerId": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "name": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com",
            "phone": "213-555-0199",
            "notes": null,
            "location": {
                "@odata.type": "#microsoft.graph.location",
                "displayName": "Customer",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "@odata.type": "#microsoft.graph.physicalAddress",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "timeZone": "America/Chicago",
            "customQuestionAnswers": [
                {
                    "questionId": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
                    "question": "What is your age?",
                    "answerInputType": "text",
                    "answerOptions": [],
                    "isRequired": true,
                    "answer": "25",
                    "selectedOptions": []
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->