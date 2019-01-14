---
title: Principais serviços e recursos do Microsoft Graph
description: 'O Microsoft Graph permite que você se integre com o melhor dos serviços do Office 365, Windows 10 e Enterprise Mobility + Security no Microsoft 365 usando APIs REST e bibliotecas de cliente. Além disso, ele oferece segurança e inteligência social que podem aumentar a produtividade do usuário, a criatividade e a colaboração em equipe, além de proteger os recursos de negócios e os dados dos usuários. '
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 0d164dc95b4ae5de683180de1b6f186dcd98f5f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820682"
---
# <a name="major-services-and-features-in-microsoft-graph"></a>Principais serviços e recursos do Microsoft Graph

O Microsoft Graph permite que você se integre com o melhor dos serviços do Office 365, Windows 10 e Enterprise Mobility + Security no Microsoft 365 usando APIs REST e bibliotecas de cliente. Além disso, ele oferece segurança e inteligência social que podem aumentar a produtividade do usuário, a criatividade e a colaboração em equipe, além de proteger os recursos de negócios e os dados dos usuários. 

## <a name="users-and-groups"></a>Usuários e grupos

Na parte central do Microsoft Graph estão os conceitos de usuário e de grupo. 

Um _usuário_ do Microsoft Graph é uma pessoa entre milhões que usam serviços em nuvem do Microsoft 365. Ele é o foco principal, aquele que é protegido e cujo acesso é bem gerenciado. Os dados do usuário é que orientam os negócios. Os serviços do Microsoft Graph disponibilizam esses dados para empresas em contextos sofisticados, atualizações em tempo real e insights profundos e, sempre, apenas com as permissões apropriadas.

Um _grupo_ do Office 365 é a principal entidade que permite aos usuários colaborar. Ele integra-se a outros serviços possibilitando cenários mais sofisticados no planejamento de tarefas, trabalho em equipe, educação e muito mais. 

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Usuários | O Azure AD e a maioria dos serviços de produtividade, colaboração, inteligência e educação | O usuário é um dos pontos centrais do Microsoft Graph, em torno do qual muitos serviços do Microsoft Graph criam uma funcionalidade centrada no usuário. | [Visão geral de usuários do Microsoft Graph](azuread-users-concept-overview.md)|
|Grupos | Azure AD, OneDrive, OneNote, Outlook, Planner | Um grupo do Office 365 fornece a unidade colaborativa fundamental para os usuários compartilharem conversas, arquivos, anotações, calendários, planos e muito mais. | [Visão geral dos grupos do Office 365 no Microsoft Graph](office365-groups-concept-overview.md) |

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
| Calendário | Outlook  | Permite que os usuários configurem compromissos e reuniões na Web, dispositivos móveis e computadores. Ele faz parte do hub de comunicação de mensagens do Outlook no Office 365 que também permite que os usuários gerenciem emails e contatos. | [Visão geral do calendário do Outlook](outlook-calendar-concept-overview.md)  |
| Arquivos | OneDrive e SharePoint | Gerencia e compartilha arquivos de usuários no OneDrive e no SharePoint. | [Visão geral do armazenamento de arquivos do OneDrive](onedrive-concept-overview.md) |
| Email | Outlook | Permite que os usuários se comuniquem, organizem mensagens e gerenciem prioridades em seus fluxos de trabalho na Web, em dispositivos móveis e de desktop. Ele faz parte do hub de comunicação do Outlook no Office 365 que também permite que os usuários gerenciem contatos e agendem reuniões. | [Visão geral do email do Outlook](outlook-mail-concept-overview.md) |
| Observações | OneNote | Permite aos usuários planejar e organizar informações e ideias. | [Visão geral das anotações do OneNote](integrate-with-onenote.md) |
| Contatos pessoais | Outlook | Entra em contato com o gerente na Web e em dispositivos móveis e de desktop. Ele faz parte do hub de comunicação de mensagens do Outlook no Office 365 que também permite que os usuários gerenciem emails e agendem reuniões.  | [Visão geral de contatos pessoais do Outlook](outlook-contacts-concept-overview.md) |
| Pastas de trabalho e gráficos | Excel | Permite que os usuários usem planilhas do Excel para fazer cálculos complexos, rastrear, analisar e visualizar dados e gerar relatórios profissionais. | [Visão geral de gráficos e pastas de trabalho do Excel](excel-concept-overview.md) |


## <a name="collaboration"></a>Colaboração

<!-- Want to update links to concept overviews as they are created over time. 
-->
|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Sites e listas  | SharePoint | A plataforma baseada na Web para os usuários e grupos do Office 365 compartilharem, organizarem, gerenciarem e descobrirem conteúdo (incluindo listas, arquivos e anotações). | [Visão geral do conteúdo e sites do SharePoint](sharepoint-concept-overview.md) | 
|Tarefas e planos | Planner | Permite que os usuários de grupos do Office 365 criem planos, atribuam tarefas e controlem o progresso. | [Visão geral de tarefas e planos do Planner](planner-concept-overview.md) |
|Trabalho em equipe |  Microsoft Teams | O hub digital e espaço de trabalho baseado em bate-papo para as equipes compartilharem arquivos, observações, calendários e planos. | [Visão geral do trabalho em equipe do Microsoft Teams](teams-concept-overview.md) |


## <a name="social-intelligence-and-analytics"></a>Inteligência social e análise

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Inteligência social: pessoas | Azure AD, Outlook, SharePoint e muito mais | Obtém informações sobre pessoas ordenados por relevância para o usuário, o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.  | [Inteligência social no Microsoft Graph](social-intel-concept-overview.md) |
| Inteligência social: insights de documentos (prévia) | Delve, OneDrive, Outlook, SharePoint | Usa análises avançadas e técnicas de aprendizado de máquina para obter documentos mais populares, vistos, modificados ou compartilhados por um usuário.  | [Inteligência social no Microsoft Graph](social-intel-concept-overview.md)  |


## <a name="device-management"></a>Gerenciamento de dispositivo

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
|Dispositivos e aplicativos | Intune | Registra e configura dispositivos e gerencia aplicativos móveis em sua organização. | [Visão geral de dispositivos e aplicativos do Intune](intune-concept-overview.md) |


## <a name="security"></a>Segurança

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Integração de segurança | Azure AD Identity Protection, Proteção de Informações do Azure, Central de Segurança do Azure, Segurança do Aplicativo Microsoft Cloud, Proteção Avançada contra Ameaças do Windows Defender e [mais](/graph/api/resources/security-api-overview?view=graph-rest-1.0) | Fornece um gateway unificado para insights e ações de segurança em todos os parceiros da Microsoft e do ecossistema. | [Segurança no Microsoft Graph](security-concept-overview.md) |



## <a name="cross-device-experiences"></a>Experiências entre dispositivos

|Recurso     |Serviços de suporte  |Descrição |Mais informações |
|:-----------|:--------------------|:-----------|:----------------|
| Experiências entre dispositivos | Feed de atividades, retransmissão de dispositivos | Permite experiências de aplicativos que transcendem um único dispositivo e que, em vez disso, são movidas com o usuário de dispositivo para dispositivo, independentemente do tipo e da plataforma. | [Visão geral das experiências entre dispositivos](cross-device-concept-overview.md) |


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
| Reserva de clientes (prévia) | Microsoft Bookings | Tem como alvo pequenas empresas para permitir que seus clientes reservem serviços diretamente na Web ou no Facebook. Permite que os operadores de negócios gerenciem as preferências, os serviços e os preços dos clientes, as listas de funcionários e os agendamentos e outras informações comerciais comuns. | [Visão geral da API do Microsoft Bookings](booking-concept-overview.md) |


## <a name="next-steps"></a>Próximas etapas

<!-- Need to update the destination page titles and URLs as Matt's v-team finalize on the examples and featured scenarios content 
-->

- Veja [exemplos](https://developer.microsoft.com/graph/examples) de soluções criativas criadas sobre os serviços do Microsoft Graph que solucionam problemas reais de clientes.
- No índice, confira **Saiba mais** para ler sobre os serviços e recursos que _você_ pode usar em seus cenários.
- Experimente um exemplo de solicitação no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Use os [inícios rápidos](https://developer.microsoft.com/graph/quick-start) para configurar um aplicativo de amostra pronto para funcionar.
