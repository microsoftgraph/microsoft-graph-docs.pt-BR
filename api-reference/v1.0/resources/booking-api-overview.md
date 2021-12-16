---
title: Usar a API do Microsoft Bookings no Microsoft Graph
description: O Microsoft Bookings permite que proprietários de pequenas empresas gerenciem reservas e informações de clientes com configuração mínima.
ms.localizationpriority: high
author: arvindmicrosoft
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: dcf56949743c4442409eb6f7345410967e0db2c0
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526447"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a>Usar a API do Microsoft Bookings no Microsoft Graph

O Microsoft Bookings permite que proprietários de pequenas empresas gerenciem reservas e informações de clientes com configuração mínima. Um proprietário de empresa pode criar um ou mais negócios e cada empresa oferece um conjunto de serviços. O proprietário pode definir membros da equipe e especificar os serviços que cada membro da equipe executará. Um cliente pode agendar um horário para um serviço específico nesse negócio em um aplicativo online ou móvel. O Bookings garante que o horário do compromisso seja mantido atualizado para a empresa, funcionários e clientes envolvidos.

Programaticamente, um [bookingBusiness](bookingbusiness.md) na API do Bookings envolve os seguintes objetos:

- Uma ou mais objetos [bookingStaffMember](bookingstaffmember.md)
- Uma ou mais objetos [bookingService](bookingservice.md)
- Um conjunto de instâncias [bookingAppointment](bookingappointment.md)
- Um conjunto de objetos [bookingCustomer](bookingcustomer.md)

## <a name="using-the-bookings-rest-api"></a>Como usar a API REST do Bookings

Siga as etapas a seguir antes de agendar os compromissos do cliente para uma empresa pela primeira vez. Certifique-se de fornecer os [tokens de acesso](/graph/auth-overview) apropriados para as operações correspondentes.

1. Certifique-se que a empresa tenha um assinatura do [Microsoft 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium).
2. Crie um novo **bookingBusiness** enviando uma operação POST para o conjunto de entidades. No mínimo, você deve especificar um nome para a nova empresa que os clientes verão:
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
Use a propriedade **id** do novo **bookingBusiness** retornado na resposta do POST para continuar a [personalizar](../api/bookingbusiness-update.md) configurações de negócios e adicionar funcionários e serviços para a empresa.

3. Adicione membros individuais da equipe para a empresa:
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. Defina cada serviço oferecido pela empresa:
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. Publique a página de agendamento para a empresa, para permitir que clientes e operadores de negócios comecem a agendar compromissos:
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

Em geral, para listar todas as empresas de agendamento no locatário do Microsoft 365:
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a>Casos de uso comuns

A tabela a seguir lista as operações comuns para uma empresa na API do Bookings.

| Casos de uso        | Recursos REST | Confira também |
|:---------------|:--------|:----------|
| Criar, acessar, atualizar ou excluir uma empresa | [bookingBusiness](bookingbusiness.md) | [Métodos de bookingBusiness](bookingbusiness.md#methods) |
| Atualizar a política de agendamento | [bookingSchedulingPolicy](bookingschedulingpolicy.md) | [Atualizar um bookingBusiness](../api/bookingbusiness-update.md) |
| Adicionar, obter, atualizar ou excluir membros da equipe | [bookingStaffMember](bookingstaffmember.md) | [Métodos de bookingStaffMember](bookingstaffmember.md#methods)  |
| Adicionar, obter, atualizar ou excluir serviços | [bookingService](bookingservice.md) | [Métodos de bookingService](bookingservice.md#methods)  |
| Adicionar, obter, atualizar ou excluir perguntas personalizadas | [bookingCustomQuestion](bookingcustomquestion.md) | [Métodos de bookingCustomQuestion](bookingcustomquestion.md#methods)  |
| Adicionar, obter, atualizar ou excluir clientes | [bookingCustomer](bookingcustomer.md) | [Métodos de bookingCustomer](bookingcustomer.md#methods)  |
| Publicar ou cancelar a publicação da página de agendamento | [bookingBusiness](bookingbusiness.md) | [publish](../api/bookingbusiness-publish.md) <br> [unpublish](../api/bookingbusiness-unpublish.md) |
| Criar, obter, atualizar, excluir ou cancelar um compromisso | [bookingAppointment](bookingappointment.md) | [Métodos de bookingAppointment](bookingappointment.md#methods)  |
| Obter compromissos em um intervalo de datas | [bookingBusiness](bookingbusiness.md) | [Listar o calendarView do Bookings](../api/bookingbusiness-list-calendarview.md) |
| Obter moeda | [bookingCurrency](bookingcurrency.md) | [Métodos de bookingCurrency](bookingcurrency.md#methods) |

## <a name="whats-new"></a>O que há de novo
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="see-also"></a>Confira também

- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/partners).
- Saiba como escolher [permissões](/graph/permissions-reference) no Microsoft Graph.


