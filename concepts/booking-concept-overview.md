---
title: Visão geral da API do Microsoft Bookings
description: O Microsoft Bookings fornece aplicativos online e móveis que tornam o agendamento de compromissos simples e eficiente para organizações e seus usuários e clientes.
author: arvindmicrosoft
ms.localizationpriority: high
ms.prod: bookings
ms.custom: scenarios:getting-started
ms.openlocfilehash: 3b143969faf7dcc67d4fc07a0ac117d9b020d09e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442159"
---
# <a name="microsoft-bookings-api-overview"></a>Visão geral da API do Microsoft Bookings

O Microsoft Bookings fornece aplicativos online e móveis que tornam o agendamento de compromissos simples e eficiente para empresas e seus clientes. Qualquer organização que forneça serviços mediante agendamento, como empresas de grande porte, oficinas de automóveis, salões de beleza e escritórios de advocacia, pode se beneficiar com o gerenciamento de seus agendamentos, e assim liberar tempo para a tarefa mais importante de expandir os negócios. O Microsoft Bookings está disponível para organizações empresariais e empresas que possuem uma assinatura do Microsoft 365 Business Premium.

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>Por que se integrar ao Microsoft Bookings usando o Microsoft Graph?

### <a name="streamline-appointment-booking"></a>Simplificar o agendamento de compromissos
Um operador de negócios nunca perderá um compromisso com um cliente mesmo estando longe do telefone ou com a empresa fechada. Os clientes poderão [ver os serviços disponíveis](/graph/api/bookingbusiness-list-services) e [agendar compromissos](/graph/api/bookingbusiness-post-appointments) diretamente na página de agendamento, no site da empresa ou pelo Facebook. 

Os operadores de negócios podem realizar agendamentos em qualquer lugar, pela Web ou em um aplicativo móvel, pessoalmente ou pelo telefone. Eles podem [reagendar](/graph/api/bookingappointment-update), [cancelar](/graph/api/bookingappointment-cancel) ou [reatribuir](/graph/api/bookingappointment-update) um agendamento existente para outro membro da equipe disponível. 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>Reduzir não comparecimentos e aumentar a produtividade da equipe
Os operadores de negócios podem especificar [políticas de agendamento](/graph/api/resources/bookingschedulingpolicy) que incluem um aviso prévio mínimo para agendamentos e cancelamentos, e os clientes podem agendar ou reagendar compromissos por conta própria. As confirmações e lembretes automatizados para agendamentos reduzem os não comparecimentos e permitem que a equipe faça um uso melhor de suas horas de trabalho. 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>Gerenciar informações e relações de clientes em qualquer lugar
A realização automática de agendamentos verifica se o cliente já se encontra na [lista de clientes](/graph/api/bookingbusiness-list-customers) e [adiciona](/graph/api/bookingbusiness-post-customers) seu nome e endereço de email à lista se necessário. Isso permite que os operadores de negócios mantenham contato com seus clientes e enviem boletins informativos periódicos ou outros materiais promocionais com facilidade.

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>Integrar-se com os serviços de colaboração em equipe e produtividade do Microsoft Graph
Ao usar o mesmo ponto de extremidade REST unificado do Microsoft Graph, você pode acessar a API do Bookings e [integrar-se com o melhor do Microsoft 365](overview-major-services.md) para permitir cenários mais amplos. Por exemplo, você pode usar o [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) para acompanhar e analisar dados financeiros da empresa e gerar relatórios profissionais ou usar o [SharePoint](sharepoint-concept-overview.md) ou o [Microsoft Teams](teams-concept-overview.md) para aprimorar colaboração em equipe.

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço? Consulte [API da Microsoft Bookings no Microsoft Graph](/graph/api/resources/booking-api-overview).

## <a name="see-also"></a>Confira também

- [Microsoft Bookings para Microsoft 365](https://support.office.com/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d)
- Outros [aplicativos de negócios do Microsoft 365](https://www.microsoft.com/microsoft-365)