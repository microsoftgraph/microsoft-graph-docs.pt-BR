---
title: Use a API do reservas Microsoft no Microsoft Graph
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Priority
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 494b13016c20124e1a81f996d332c97c15e46852
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915729"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a>Use a API do reservas Microsoft no Microsoft Graph

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.
 
Microsoft Bookings permite que os proprietários de pequenas empresas gerencie informações com uma configuração mínima e reservas de cliente. Um proprietário de negócios pode criar uma ou mais empresas, com cada empresa que oferece um conjunto de serviços. O proprietário pode configurar membros da equipe e especifique os serviços que cada membro da equipe realiza. Um cliente pode agendar um compromisso para um serviço específico em que os negócios em um aplicativo online ou móvel. Reservas garante que a hora do compromisso é mantida atualizada para os negócios, os membros da equipe e clientes envolvido.

Programaticamente, um [bookingBusiness](bookingbusiness.md) na API reservas envolve os seguintes objetos:
 
- Um ou mais objetos [bookingStaffMember](bookingstaffmember.md)
- Um ou mais objetos [bookingService](bookingservice.md)
- Um conjunto de instâncias de [bookingAppointment](bookingappointment.md)
- Um conjunto de objetos [bookingCustomer](bookingcustomer.md)

## <a name="using-the-bookings-rest-api"></a>Usando as API REST reservas

Explore as etapas a seguir antes de compromissos do cliente para uma empresa de reserva na primeira vez. Verifique se que você fornecer [tokens de acesso](/graph/auth-overview) apropriado para as operações correspondentes.

1. Verifique se que a empresa tem uma assinatura do [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) .
2. Crie um novo **bookingBusiness** enviando uma operação POST no conjunto de entidade. No mínimo, você deve especificar um nome para o novo negócio que os clientes verão:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
Use a propriedade **id** do novo **bookingBusiness** retornados na resposta POST para continuar para [Personalizar](../api/bookingbusiness-update.md) configurações de negócios e adicionar membros da equipe e serviços para a empresa.

3. Adicione membros da equipe individuais para os negócios:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. Defina cada serviço oferecido pela empresa:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. Publica a página de agendamento para os negócios, para permitir que os clientes e iniciar o agendamento de compromissos de operadores de negócios:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

Em geral, para listar todas as empresas de reserva em inquilino do Office 365:<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a>Casos comuns de uso 

A tabela a seguir lista as operações comuns para uma empresa na API reservas.

| Casos de uso        | Recursos REST | Confira também |
|:---------------|:--------|:----------|
| Criar, obter, atualizar ou excluir uma empresa | [bookingBusiness](bookingbusiness.md) | [Métodos de bookingBusiness](bookingbusiness.md#methods) |
| Atualizar a política de agendamento | [bookingSchedulingPolicy](bookingschedulingpolicy.md) | [Atualizar um bookingBusiness](../api/bookingbusiness-update.md) |
| Adicionar, obter, atualizar ou excluir membros da equipe | [bookingStaffMember](bookingstaffmember.md) | [Métodos de bookingStaffMember](bookingstaffmember.md#methods)  |
| Adicionar, obter, atualizar ou excluir serviços | [bookingService](bookingservice.md) | [Métodos de bookingService](bookingservice.md#methods)  |
| Publicar ou cancelar a publicação de página de agendamento | [bookingBusiness](bookingbusiness.md) | [Publicar](../api/bookingbusiness-publish.md) <br> [cancelamento de publicação](../api/bookingbusiness-unpublish.md) |
| Criar, obter, atualizar, excluir ou cancelar um compromisso | [bookingAppointment](bookingappointment.md) | [Métodos de bookingAppointment](bookingappointment.md#methods)  |
| Obter compromissos em um intervalo de datas | [bookingBusiness](bookingbusiness.md) | [Lista reservas calendarView](../api/bookingbusiness-list-calendarview.md) |
| Obtenha a moeda | [bookingCurrency](bookingcurrency.md) | [Métodos de bookingCurrency](bookingcurrency.md#methods) |


## <a name="see-also"></a>Confira também

- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Consulte [como alguns dos nossos parceiros estão usando o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).
- Saiba como escolher as [permissões](/graph/permissions-reference) no Microsoft Graph.
