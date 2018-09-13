# <a name="microsoft-bookings-api-overview-preview"></a>Visão geral da API do Microsoft Bookings (versão prévia)

O Microsoft Bookings fornece aplicativos móveis e online que tornam simples e eficiente o agendamento de compromissos para pequenas empresas e seus clientes. Qualquer pequena empresa que forneça serviços com base em agendamentos, como oficinas mecânicas, salões de cabeleireiros e empresas de advocacia, podem beneficiar com o gerenciamento de seus agendamentos para liberar tempo para tarefas mais importantes para expandir seus negócios. O Microsoft Bookings está disponível para empresas que possuem uma assinatura do Office 365 Business Premium.

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>Por que se integrar ao Microsoft Bookings usando o Microsoft Graph?

### <a name="streamline-appointment-booking"></a>Simplificar o agendamento de compromissos
Um operador de negócios nunca perderá um compromisso com um cliente mesmo estando longe do telefone ou com a empresa fechada. Os clientes poderão [ver os serviços disponíveis](../api-reference/beta/api/bookingbusiness_list_services.md) e [agendar compromissos](../api-reference/beta/api/bookingbusiness_post_appointments.md) diretamente na página de agendamento, no site da empresa ou pelo Facebook. 

Os operadores de negócios podem realizar agendamentos em qualquer lugar, pela Web ou em um aplicativo móvel, pessoalmente ou pelo telefone. Eles podem [reagendar](../api-reference/beta//api/bookingappointment_update.md), [cancelar](../api-reference/beta/api/bookingappointment_cancel.md) ou [reatribuir](../api-reference/beta/api/bookingappointment_update.md) um agendamento existente para outro membro da equipe disponível. 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>Reduzir não comparecimentos e aumentar a produtividade da equipe
Os operadores de negócios podem especificar [políticas de agendamento](../api-reference/beta/resources/bookingschedulingpolicy.md) que incluem um aviso prévio mínimo para agendamentos e cancelamentos, e os clientes podem agendar ou reagendar compromissos por conta própria. As confirmações e lembretes automatizados para agendamentos reduzem os não comparecimentos e permitem que a equipe faça um uso melhor de suas horas de trabalho. 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>Gerenciar informações e relações de clientes em qualquer lugar
A realização automática de agendamentos verifica se o cliente já se encontra na [lista de clientes](../api-reference/beta/api/bookingbusiness_list_customers.md) e [adiciona](../api-reference/beta/api/bookingbusiness_post_customers.md) seu nome e endereço de email à lista se necessário. Isso permite que os operadores de negócios mantenham contato com seus clientes e enviem boletins informativos periódicos ou outros materiais promocionais com facilidade.

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>Integrar-se com os serviços de colaboração em equipe e produtividade do Microsoft Graph
Ao usar o mesmo ponto de extremidade REST unificado do Microsoft Graph, você pode acessar a API do Bookings e [integrar-se com o melhor do Microsoft 365](overview-major-services.md) para permitir cenários mais amplos. Por exemplo, você pode usar o [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) para acompanhar e analisar dados financeiros da empresa e gerar relatórios profissionais ou usar o [SharePoint](sharepoint-concept-overview.md) ou o [Microsoft Teams](teams-concept-overview.md) para aprimorar colaboração em equipe.

## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Microsoft Bookings](https://support.office.com/en-us/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) e outros [aplicativos do Office 365 business](https://support.office.com/en-us/article/manage-your-business-apps-in-the-business-center-47eca808-cf96-42ba-83e8-55daf18e49dc?ui=en-US&rs=en-US&ad=US).
- [Usar a API do Bookings](../api-reference/beta/resources/booking-api-overview.md) do Microsoft Graph.

