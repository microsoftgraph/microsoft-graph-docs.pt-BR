---
title: Principais serviços e recursos do Microsoft Graph
description: 'O Microsoft Graph permite a integração com os melhores serviços do Microsoft 365, Windows 10 e Enterprise Mobility + Security no Microsoft 365, usando a APIs REST e as bibliotecas de clientes. Além disso, ele oferece segurança e inteligência social que podem aumentar a produtividade do usuário, a criatividade e a colaboração em equipe, além de proteger os recursos de negócios e os dados dos usuários. '
author: angelgolfer-ms
ms.localizationpriority: high
ms.custom: scenarios:getting-started
ms.openlocfilehash: 7d2a3df6af87d9e3b9802e112bc429682a42d989
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424599"
---
# <a name="major-services-and-features-in-microsoft-graph"></a>Principais serviços e recursos do Microsoft Graph

O Microsoft Graph permite a integração com os melhores serviços do Microsoft 365, Windows 10 e Enterprise Mobility + Security no Microsoft 365, usando a APIs REST e as bibliotecas de clientes. Além disso, oferece segurança e inteligência que podem aumentar a produtividade do usuário, bem como a criatividade e a colaboração em equipe, além de proteger os recursos de negócios e os dados dos usuários. 

## <a name="users-and-groups"></a>Usuários e grupos

Na parte central do Microsoft Graph estão os conceitos de usuário e de grupo. 

Um _usuário_ do Microsoft Graph é uma pessoa entre milhões que usam serviços em nuvem do Microsoft 365. Ele é o foco principal, aquele que é protegido e cujo acesso é bem gerenciado. Os dados do usuário é que orientam os negócios. Os serviços do Microsoft Graph disponibilizam esses dados para empresas em contextos sofisticados, atualizações em tempo real e insights profundos e, sempre, apenas com as permissões apropriadas.

O grupo no _Microsoft 365_ é a entidade fundamental que permite que os usuários colaborem. Ele integra-se a outros serviços possibilitando cenários mais sofisticados no planejamento de tarefas, trabalho em equipe, educação e muito mais. 

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Usuários | O Azure AD e a maioria dos serviços de produtividade, colaboração, inteligência e educação | O usuário é um dos pontos centrais do Microsoft Graph, em torno do qual muitos serviços do Microsoft Graph criam uma funcionalidade centrada no usuário. | [Visão geral de usuários do Microsoft Graph](azuread-users-concept-overview.md)|
|Grupos | Azure AD, OneDrive, OneNote, Outlook, Planner | Um grupo no Microsoft 365 fornece a unidade colaborativa fundamental para os usuários compartilharem conversas, arquivos, notas, calendário, planos e muito mais. | [Visão geral dos grupos do Microsoft 365 no Microsoft Graph](office365-groups-concept-overview.md) |

## <a name="connecting-users-data-microsoft-365-services-and-your-apps"></a>Como conectar dados de usuários, serviços do Microsoft 365 e seus aplicativos

Começando com usuários e grupos no núcleo, o Microsoft Graph forma uma rede de serviços e recursos do Microsoft 365 que gerencia, protege e extrai dados para oferecer suporte a uma ampla gama de cenários. O Microsoft Graph permite que você acesse essa riqueza de dados do usuário, sempre respeitando a autorização adequada.

![O Microsoft Graph conecta você aos dados dos usuários](images/microsoft-graph-connects-users-data.png)

### <a name="services-and-features"></a>Serviços e recursos

Alguns serviços do Microsoft Graph iniciam-se no próprio Microsoft Graph, outros são bem conhecidos como serviços autônomos, mas já estão convergindo no Microsoft Graph. Seus conjuntos de APIs seguem um design simplificado, conforme detalhado nas [diretrizes da API REST da Microsoft](https://github.com/Microsoft/api-guidelines), e agora estão acessíveis por meio do único ponto de extremidade REST do Microsoft Graph `https://graph.microsoft.com`. O restante deste artigo lista os principais serviços e recursos por categoria. 


## <a name="identity-and-access-management"></a>Gerenciamento de identidades e acesso

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Gerenciamento de identidades e acesso | Azure AD | Cria e gerencia recursos de diretório, como usuários, grupos e aplicativos. Gerencie o acesso a recursos e dados. Oferece acesso aos clientes a dados de entrada e de risco da conta no Azure AD.| [Visão geral do gerenciamento de identidade e acesso do Azure AD](azuread-identity-access-management-concept-overview.md)  |


## <a name="productivity"></a>Produtividade

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Calendário | Outlook  | Permite que os usuários configurem compromissos e reuniões na Web, dispositivos móveis e computadores. Faz parte do hub de comunicação de mensagens do Outlook no Microsoft 365 que também permite que os usuários gerenciem emails e contatos. | [Visão geral do calendário do Outlook](outlook-calendar-concept-overview.md)  |
| Arquivos | OneDrive e SharePoint | Gerencia e compartilha arquivos de usuários no OneDrive e no SharePoint. | [Visão geral do armazenamento de arquivos do OneDrive](onedrive-concept-overview.md) |
| Email | Outlook | Permite que os usuários se comuniquem, organizem mensagens e gerenciem prioridades em seus fluxos de trabalho na Web, em dispositivos móveis e de desktop. Faz parte do hub de comunicação do Outlook no Microsoft 365, que também permite que os usuários gerenciem contatos e agendem reuniões. | [Visão geral do email do Outlook](outlook-mail-concept-overview.md) |
| Observações | OneNote | Permite aos usuários planejar e organizar informações e ideias. | [Visão geral das anotações do OneNote](integrate-with-onenote.md) |
| Contatos pessoais | Outlook | Entra em contato com o gerente na Web e em dispositivos móveis e de desktop. Faz parte do hub de comunicação de mensagens do Outlook no Microsoft 365, que também permite que os usuários gerenciem emails e agendem reuniões.  | [Visão geral de contatos pessoais do Outlook](outlook-contacts-concept-overview.md) |
| Pastas de trabalho e gráficos | Excel | Permite que os usuários usem planilhas do Excel para fazer cálculos complexos, rastrear, analisar e visualizar dados e gerar relatórios profissionais. | [Visão geral de gráficos e pastas de trabalho do Excel](excel-concept-overview.md) |
| Tarefas pendentes | To Do | Permite aos usuários gerenciar suas tarefas pessoais em todo seu trabalho e na sua vida pessoal. Ele também está integrado ao Outlook, Equipes, Planner e Cortana, o que o torna o único destino para as tarefas pessoais do usuário no Microsoft 365 | [Visão geral sobre tarefas To Do](todo-concept-overview.md) |

## <a name="collaboration"></a>Colaboração

<!-- Want to update links to concept overviews as they are created over time. 
-->
|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Comunicações na nuvem | Microsoft Teams, Skype | Permite que aplicativos e serviços interajam com os usuários por meio de vários recursos relacionados à comunicação, por exemplo, permitindo que os robôs possam lidar com chamadas, integrando reuniões on-line em cenários de negócios, mostrando o status de presença dos usuários (visualização) e pesquisando registros de chamadas e reuniões on-line ( visualização). | [Visão geral das comunicações na nuvem](cloud-communications-concept-overview.md) |
| Sites e listas  | SharePoint | Plataforma baseada na Web para usuários e grupos do Microsoft 365 compartilharem, organizarem, gerenciarem e descobrirem conteúdo (incluindo listas, arquivos e anotações). | [Visão geral do conteúdo e sites do SharePoint](sharepoint-concept-overview.md) | 
|Tarefas e planos | Planner | Permite que os usuários dos grupos do Microsoft 365 criem planos, atribuam tarefas e acompanhem o progresso. | [Visão geral de tarefas e planos do Planner](planner-concept-overview.md) |
|Trabalho em equipe |  Microsoft Teams | O hub digital e espaço de trabalho baseado em bate-papo para as equipes compartilharem arquivos, observações, calendários e planos. | [Visão geral do trabalho em equipe do Microsoft Teams](teams-concept-overview.md) |


## <a name="people-and-workplace-intelligence"></a>Inteligência de pessoas e no local de trabalho

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Pessoas | Azure AD, Outlook, SharePoint e muito mais | Obtém informações sobre pessoas ordenados por relevância para o usuário, o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.  | [Inteligência de pessoas e no local de trabalho no Microsoft Graph](social-intel-concept-overview.md) |
| Perfil (visualização) | Perfil | Fornece um mecanismo leve para armazenar e recuperar informações sobre as pessoas em um locatário. | [Inteligência de pessoas e no local de trabalho no Microsoft Graph](social-intel-concept-overview.md) |
| Personalização do cartão de perfil (visualização) | Cartão de perfil | Fornece um mecanismo leve para que um administrador personalize o conteúdo que aparece no cartão de perfil do Microsoft 365 dentro de uma organização. | [Inteligência de pessoas e no local de trabalho no Microsoft Graph](social-intel-concept-overview.md) |
| Insights do documento  | Delve, OneDrive, Outlook, SharePoint | Usa análises avançadas e técnicas de aprendizado de máquina para obter documentos mais populares, vistos, modificados ou compartilhados por um usuário.  | [Inteligência de pessoas e no local de trabalho no Microsoft Graph](social-intel-concept-overview.md)  |
| Análise (visualização) | MyAnalytics | Usa análises e técnicas avançadas de aprendizado de máquina para fornecer informações sobre como e com quem as pessoas passam o tempo. Esses dados podem ajudar as pessoas a planejar o dia, obter informações sobre seus diferentes padrões de trabalho e ajudar a equilibrar o trabalho e a vida.  | [Inteligência de pessoas e no local de trabalho no Microsoft Graph](social-intel-concept-overview.md) |


## <a name="device-and-app-management"></a>Gerenciamento de aplicativo e dispositivo

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Impressão na nuvem | Impressão universal | A impressão universal é uma infraestrutura de impressão baseada na nuvem do Microsoft 365 que permite uma experiência de impressão simples, rica e segura aos usuários e reduz o tempo e o esforço de TI. | [Impressão na nuvem usando a API de Impressão Universal](universal-print-concept-overview.md) |
|Gerenciamento corporativo de dispositivos e aplicativos | Intune | Registra e configura dispositivos e gerencia aplicativos móveis em sua organização. | [Visão geral de dispositivos e aplicativos do Intune](intune-concept-overview.md) |
| Cloud PC (visualização) | Windows 365  | O Windows 365 é um serviço baseado em nuvem que permite aos administradores configurar e gerenciar facilmente Cloud PCs do Windows 365 para usuários em sua organização. Os usuários finais individuais podem transmitir com segurança sua experiência rica e personalizada com o Windows da Microsoft Cloud para qualquer dispositivo, a qualquer momento, com seu Cloud PC. | [Trabalhando com Cloud PCs do Windows 365 usando a API do Microsoft Graph](cloudpc-concept-overview.md) |
| Atualizações do dispositivo (visualização) | Serviço de implantação do Windows Update para Empresas | Fornece controle sobre a aprovação, agendamento, monitoramento e proteção do conteúdo fornecido pelo Windows Update. | [Atualizações do Windows no Microsoft Graph](windowsupdates-concept-overview.md) |
| Gerenciamento multilocatário (visualização) | Microsoft 365 Lighthouse | Permite que os Provedores de Serviços Gerenciados (MSPs) gerenciem remotamente vários locatários do cliente para conformidade e detecção de ameaças, e ajudam a manter os dispositivos dos locatários em um estado íntegro e seguro. | [Gerenciamento multilocatário usando o Microsoft 365 Lighthouse](managedtenants-concept-overview.md) |
| Comunicações e Integridade do serviço | Serviços do Microsoft 365 e Dynamics 365 | Fornece acesso ao status de integridade e postagens do centro de mensagens sobre os serviços em nuvem da Microsoft. Um exemplo importante que usa a API de comunicações de serviço é o Centro de administração do Microsoft 365. | [Acessando as comunicações e a Integridade do serviço no Microsoft Graph](service-communications-concept-overview.md) |


## <a name="security"></a>Segurança

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Integração de segurança | Azure AD Identity Protection, Proteção de Informações do Azure, Central de Segurança do Azure, Microsoft Defender for Cloud Apps, Windows Defender Proteção Avançada contra Ameaças e [mais](/graph/api/resources/security-api-overview) | Fornece um gateway unificado para insights e ações de segurança em todos os parceiros da Microsoft e do ecossistema. | [Segurança no Microsoft Graph](security-concept-overview.md) |



## <a name="cross-device-experiences"></a>Experiências entre dispositivos

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Experiências entre dispositivos | Feed de atividades, retransmissão de dispositivos | Permite experiências de aplicativos que transcendem um único dispositivo e que, em vez disso, são movidas com o usuário de dispositivo para dispositivo, independentemente do tipo e da plataforma. | [Visão geral das experiências entre dispositivos](cross-device-concept-overview.md) |

## <a name="user-notifications"></a>Notificações do usuário

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Notificações do usuário | Notificações do usuário | Permite que experiências de aplicativos criem experiências de notificação centradas no usuário e em várias plataformas, incluindo fan-out com base no usuário, dispensa universal e acesso ao histórico de notificações. | [Habilitando experiências de notificação centradas no ser humano usando notificações do Microsoft Graph](notifications-concept-overview.md) |


## <a name="usage-reports"></a>Relatórios de uso

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Relatórios | Microsoft Teams, OneDrive, Outlook, SharePoint, Skype for Business, Yammer | Obtém informações sobre atividades e uso de um serviço de suporte. | [Visão geral dos relatórios de uso](reportroot-concept-overview.md) |


## <a name="education"></a>Educação

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Educação | Azure AD, Educação | Fornece informações relevantes para cenários educacionais, incluindo escolas, turmas, alunos, professores e informações sobre tarefas. Permite que os ISVs criem aplicativos para as salas de aula que economizem o tempo dos professores e promovam o trabalho em equipe e a colaboração.  | [Visão geral de educação](education-concept-overview.md) |


## <a name="business-applications"></a>Aplicativos de negócios

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Reserva de clientes (prévia) | Microsoft Bookings | Tem como alvo organizações para permitir que seus usuários e clientes reservem serviços diretamente na Web ou no Facebook. Permite que os provedores de negócios gerenciem preferências, serviços e preços do cliente, listas e agendas de funcionários e outras informações empresariais comuns. | [Visão geral da API do Microsoft Bookings](booking-concept-overview.md) |
| Finanças (visualização) | Dynamics 365 Business Central | Permite o gerenciamento de dados financeiros, automação e segurança da cadeia de suprimentos, gerenciamento de vendas e melhor atendimento ao cliente, gerenciamento de projetos e otimização de operações com a solução completa de gerenciamento de negócios.| [Visão geral da API Business Central](dynamics-business-central-concept-overview.md) |


## <a name="next-steps"></a>Próximas etapas

<!-- Need to update the destination page titles and URLs as Matt's v-team finalize on the examples and featured scenarios content 
-->

- No índice, confira **Saiba mais** para ler sobre os serviços e recursos que _você_ pode usar em seus cenários.
- Experimente um exemplo de solicitação no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Use os [inícios rápidos](https://developer.microsoft.com/graph/quick-start) para configurar um aplicativo de amostra pronto para funcionar.
