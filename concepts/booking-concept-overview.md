---
title: Visão geral da API do Microsoft Bookings (versão prévia)
description: O Microsoft Bookings fornece aplicativos online e móveis que tornam simples e eficiente o agendamento de compromissos para a organização, seus usuários e clientes.
author: arvindmicrosoft
localization_priority: Priority
ms.prod: bookings
ms.custom: scenarios:getting-started
ms.openlocfilehash: 2da9393f7c374e96f540efad3ed7e2aeb1ce6cd077b44e0beb6495a12148daad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237576"
---
# <a name="microsoft-bookings-api-overview-preview"></a>Visão geral da API do Microsoft Bookings (versão prévia)

O Microsoft Bookings fornece aplicativos móveis e online que tornam simples e eficiente o agendamento de compromissos para pequenas empresas e seus clientes. Qualquer organização que forneça serviços mediante agendamento, como empresas de grande porte, oficinas de automóveis, salões de beleza e escritórios de advocacia, pode se beneficiar com o gerenciamento de seus agendamentos, e assim liberar tempo para a tarefa mais importante de expandir os negócios. O Microsoft Bookings está disponível para organizações empresariais e empresas que possuem uma assinatura do Microsoft 365 Business Premium.

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>Por que se integrar ao Microsoft Bookings usando o Microsoft Graph?

### <a name="streamline-appointment-booking"></a>Simplificar o agendamento de compromissos
Um operador de negócios nunca perderá um compromisso com um cliente mesmo estando longe do telefone ou com a empresa fechada. Os clientes poderão [ver os serviços disponíveis](/graph/api/bookingbusiness-list-services?view=graph-rest-beta) e [agendar compromissos](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta) diretamente na página de agendamento, no site da empresa ou pelo Facebook. 

Os operadores de negócios podem realizar agendamentos em qualquer lugar, pela Web ou em um aplicativo móvel, pessoalmente ou pelo telefone. Eles podem [reagendar](/graph/api/bookingappointment-update?view=graph-rest-beta), [cancelar](/graph/api/bookingappointment-cancel?view=graph-rest-beta) ou [reatribuir](/graph/api/bookingappointment-update?view=graph-rest-beta) um agendamento existente para outro membro da equipe disponível. 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>Reduzir não comparecimentos e aumentar a produtividade da equipe
Os operadores de negócios podem especificar [políticas de agendamento](/graph/api/resources/bookingschedulingpolicy?view=graph-rest-beta) que incluem um aviso prévio mínimo para agendamentos e cancelamentos, e os clientes podem agendar ou reagendar compromissos por conta própria. As confirmações e lembretes automatizados para agendamentos reduzem os não comparecimentos e permitem que a equipe faça um uso melhor de suas horas de trabalho. 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>Gerenciar informações e relações de clientes em qualquer lugar
A realização automática de agendamentos verifica se o cliente já se encontra na [lista de clientes](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta) e [adiciona](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta) seu nome e endereço de email à lista se necessário. Isso permite que os operadores de negócios mantenham contato com seus clientes e enviem boletins informativos periódicos ou outros materiais promocionais com facilidade.

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>Integrar-se com os serviços de colaboração em equipe e produtividade do Microsoft Graph
Ao usar o mesmo ponto de extremidade REST unificado do Microsoft Graph, você pode acessar a API do Bookings e [integrar-se com o melhor do Microsoft 365](overview-major-services.md) para permitir cenários mais amplos. Por exemplo, você pode usar o [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) para acompanhar e analisar dados financeiros da empresa e gerar relatórios profissionais ou usar o [SharePoint](sharepoint-concept-overview.md) ou o [Microsoft Teams](teams-concept-overview.md) para aprimorar colaboração em equipe.

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

Confira [API do Microsoft Bookings no Microsoft Graph beta](/graph/api/resources/booking-api-overview?view=graph-rest-beta).


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Microsoft Bookings](https://support.office.com/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) e outros [aplicativos para empresas do Microsoft 365](https://support.office.com/article/manage-your-business-apps-in-the-business-center-47eca808-cf96-42ba-83e8-55daf18e49dc?ui=en-US&rs=en-US&ad=US).
- [Usar a API do Bookings](/graph/api/resources/booking-api-overview?view=graph-rest-beta) do Microsoft Graph.

