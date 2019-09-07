---
title: Visão geral da API de educação
description: A API educacional do Microsoft Graph aprimora os recursos do Office 365 com informações relevantes para cenários educacionais, incluindo informações sobre escolas, aulas, usuários (alunos e professores), tarefas e trabalhos. Isso facilita a criação de soluções que se integrem aos recursos educacionais para vários cenários da escola e da sala de aula.
author: mmast-msft
localization_priority: Priority
ms.prod: education
scenarios: getting-started
ms.openlocfilehash: 749d97ed3181852751996792e07ca4c573bb1c60
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792846"
---
# <a name="education-api-overview"></a>Visão geral da API de educação

A API educacional do Microsoft Graph aprimora os recursos do Office 365 com informações relevantes para cenários educacionais, incluindo informações sobre escolas, aulas, usuários (alunos e professores), tarefas e trabalhos. Isso facilita a criação de soluções que se integrem aos recursos educacionais para vários cenários da escola e da sala de aula.

> [!VIDEO https://www.youtube-nocookie.com/embed/EnDM7KMTEqQ]

## <a name="why-integrate-with-education-scenarios"></a>Por que se integrar aos cenários educativos?

### <a name="build-applications-that-are-aware-of-class-roster"></a>Criar aplicativos que reconhecem a lista de participantes do curso

A maioria dos desenvolvedores de softwares educacionais sabe desde o início que essa lista de participantes do curso é uma das principais informações necessárias à execução do aplicativo, e geralmente ela está “presa” no Sistema de Informações do Aluno (SIS, Student Information System) da escola. Sempre que os professores utilizam um novo aplicativo na sala de aula, eles perdem tempo importando manualmente os dados da lista de participação para o aplicativo. Muitos fornecedores independentes de software (ISVs) abordam isso se conectando a um SIS para importar os dados da lista de participação. Com centenas de SIS com formatos proprietários, isso pode se tornar um desafio. O [Microsoft School Data Sync](https://sds.microsoft.com/), combinado às APIs de lista de participação, lida com esse desafio para desenvolvedores de aplicativos e escolas.

Vejamos a seguir alguns dos cenários permitidos pelas APIs de lista de participação:

- [Obter todas as aulas de uma escola](/graph/api/educationschool-list-classes?view=graph-rest-1.0)
- [Obter todos os usuários de uma aula](/graph/api/educationclass-list-members?view=graph-rest-1.0)
- [Obter todas as aulas que eu ensino](/graph/api/educationuser-list-classes?view=graph-rest-1.0)


### <a name="use-microsoft-teams-to-create-class-assignments-in-an-assignments-tab"></a>Usar o Microsoft Teams para criar tarefas da aula em uma guia de tarefas


Você pode usar a API de tarefas para criar um aplicativo Web que gerencia as tarefas da aula e, em seguida, integrar o seu aplicativo ao Microsoft Teams em uma nova guia personalizada.  

O Microsoft Teams no Office 365 é um hub digital que reúne conversas, conteúdo e aplicativos em um só lugar para as salas de aula. O Microsoft Teams oferece um [conjunto avançado de pontos de extensibilidade](https://docs.microsoft.com/pt-BR/microsoftteams/platform/concepts/apps/apps-overview), incluindo a criação de guias, conectores e bots. Esses pontos de extensibilidade podem chamar as APIs educacionais do Microsoft Graph para lidar com tarefas e trabalhos. Crie uma experiência mais abrangente habilitando o seu ponto de extensão com qualquer outra API do Microsoft Graph e as APIs de tarefa e de trabalhos.

Para o setor educacional, os aplicativos de guia personalizada do Microsoft Teams são abertos em um contexto de sala de aula educacional (uma equipe), onde faz sentido gerenciar o fluxo de tarefas de ponta a ponta, desde a criação e a distribuição até as notas e o feedback. Isso é apenas um exemplo de como o Microsoft Teams economiza tempo e simplifica a logística do dia a dia, deixando os educadores livres para se dedicarem aos alunos.

A imagem a seguir mostra um aplicativo Web para gerenciar tarefas em uma guia personalizada denominada Tarefas para uma aula de **Ciência – Biologia 1**.

![Captura de tela de uma guia denominada Tarefas no Microsoft Teams para uma aula de Ciência – Biologia](images/assignmentsinteams.png)


Com a API de tarefas, o seu aplicativo pode interagir com o serviço de tarefas fora do Microsoft Teams. O Microsoft Teams cuida da distribuição, das datas de conclusão e das notas, enquanto o sistema pode fornecer uma experiência avançada de aprendizagem aos alunos.
Vejamos a seguir exemplos de alguns cenários habilitados pela API de tarefas:

- [Adicionar uma tarefa que se vincula ao seu aplicativo](/graph/api/educationclass-post-assignments?view=graph-rest-beta) 
- [Atribuir notas a alunos individuais para as tarefas vinculadas ao seu aplicativo](/graph/api/educationsubmission-update?view=graph-rest-beta)
- [Criar um painel do aluno para mostrar as tarefas cuja data de entrega já passou](/graph/api/educationclass-list-assignments?view=graph-rest-beta)


### <a name="enable-school-admins-to-manage-identity-and-roster-sync-using-school-data-sync-management-preview"></a>Permitir que os diretores de escola gerenciem a identidade e a sincronização da lista de participação usando o Gerenciamento do School Data Sync (visualização)

O [School Data Sync](https://sds.microsoft.com/) ajuda a automatizar o processo de importação e sincronização da identidade do aluno e dos dados de lista de participação a partir de sistemas de informações do aluno com o Azure Active Directory (Azure AD) e o Office 365. Após as informações serem sincronizadas, você pode usar as APIs de lista de participação para ler as informações da lista nos aplicativos. Se você for um integrador de sistema configurando a integração do Sistema de Informações do Aluno de uma escola com a School Data Sync, use as [APIs de gerenciamento do SDS](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta) do Microsoft Graph para configurar a sincronização de um arquivo CSV ou de um conector da API do SIS compatível.

As APIs de gerenciamento da School Data Sync oferecem suporte a cenários completos para o gerenciamento de sincronização, por exemplo:

- [Criar um perfil que inicia automaticamente a sincronização](/graph/api/educationsynchronizationprofile-post?view=graph-rest-beta)
- Gerenciar o ciclo de vida da sincronização com as operações [pausar](/graph/api/educationsynchronizationprofile-pause?view=graph-rest-beta), [retomar](/graph/api/educationsynchronizationprofile-resume?view=graph-rest-beta) e [redefinir](/graph/api/educationsynchronizationprofile-reset?view=graph-rest-beta)

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API de Educação no Microsoft Graph v1.0](/graph/api/resources/education-overview?view=graph-rest-1.0)
- [API de Educação no Microsoft Graph beta](/graph/api/resources/education-overview?view=graph-rest-beta)


## <a name="next-steps"></a>Próximas etapas

- Para começar a usar as APIs educacionais, consulte:
  - [Usar as APIs de lista de participantes](/graph/api/resources/education-overview?view=graph-rest-1.0)
  - [Usar as APIs de tarefa](/graph/api/resources/educationassignment?view=graph-rest-beta)
  - [Usar as APIs de gerenciamento de SDS](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta)
- Experimente as APIs de educação no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Explore os seguintes exemplos relacionados ao setor educacional:
  - [Exemplo de SSO e lista de participantes em .NET](https://github.com/OfficeDev/O365-EDU-AspNetMVC-Samples)
  - [Exemplo de nó angular para SSO e Lista de participantes](https://github.com/OfficeDev/O365-EDU-AngularNodeJS-Samples)   
  - [Exemplo de SSO e Lista de participantes em Python](https://github.com/OfficeDev/O365-EDU-Python-Samples)
  - [Exemplo de PHP para Lista de Participantes & de SSO](https://github.com/OfficeDev/O365-EDU-PHP-Samples)
  - [Exemplo de APIs de gerenciamento de perfil](https://github.com/OfficeDev/O365-EDU-SDS-AspNetMVC-Samples) 



 

