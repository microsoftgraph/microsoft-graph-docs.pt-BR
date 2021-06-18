---
title: Visão geral da API de educação
description: A API educacional do Microsoft Graph aprimora os recursos do Microsoft 365 com informações relevantes para cenários educacionais, incluindo informações sobre escolas, aulas, usuários (alunos e professores), tarefas e trabalhos. Isso facilita a criação de soluções que se integrem aos recursos educacionais para vários cenários da escola e da sala de aula.
author: mmast-msft
localization_priority: Priority
ms.prod: education
ms.custom: scenarios:getting-started
ms.openlocfilehash: 258659da2ad842971043d76ec52888bfd15a236e
ms.sourcegitcommit: 2d0daa446c7b37ced1d214e0c6e18e2b8243bb09
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2021
ms.locfileid: "53010182"
---
# <a name="education-api-overview"></a>Visão geral da API de educação

A API educacional do Microsoft Graph aprimora os recursos do Microsoft 365 com informações relevantes para cenários educacionais, incluindo informações sobre escolas, aulas, usuários (alunos e professores), tarefas e trabalhos. Isso facilita a criação de soluções que se integrem aos recursos educacionais para vários cenários da escola e da sala de aula.

> [!VIDEO https://www.youtube-nocookie.com/embed/EnDM7KMTEqQ]

## <a name="why-integrate-with-education-scenarios"></a>Por que se integrar aos cenários educativos?

### <a name="build-applications-that-are-aware-of-class-roster"></a>Criar aplicativos que reconhecem a lista de participantes do curso

A maioria dos desenvolvedores de softwares educacionais sabe desde o início que essa lista de participantes do curso é uma das principais informações necessárias à execução do aplicativo, e geralmente ela está “presa” no Sistema de Informações do Aluno (SIS, Student Information System) da escola. Sempre que os professores utilizam um novo aplicativo na sala de aula, eles perdem tempo importando manualmente os dados da lista de participação para o aplicativo. Muitos fornecedores independentes de software (ISVs) abordam isso se conectando a um SIS para importar os dados da lista de participação. Com centenas de SIS com formatos proprietários, isso pode se tornar um desafio. O [Microsoft School Data Sync](https://sds.microsoft.com/), combinado às APIs de lista de participação, lida com esse desafio para desenvolvedores de aplicativos e escolas.

Vejamos a seguir alguns dos cenários permitidos pelas APIs de lista de participação:

- [Obter todas as aulas de uma escola](/graph/api/educationschool-list-classes?view=graph-rest-1.0)
- [Obter todos os usuários de uma aula](/graph/api/educationclass-list-members?view=graph-rest-1.0)
- [Obter todas as aulas que eu ensino](/graph/api/educationuser-list-classes?view=graph-rest-1.0)


### <a name="use-microsoft-teams-to-create-class-assignments-in-an-assignments-tab"></a>Usar o Microsoft Teams para criar tarefas da aula em uma guia de tarefas

Você pode usar as APIs de educação relacionadas a atribuições para integrá-las às atribuições do Microsoft Teams. O Microsoft Teams no Microsoft 365 Educacional é baseado nas mesmas APIs educacionais e fornece um caso de uso para o que você pode fazer com as APIs. Seu aplicativo pode usar essas APIs para interagir com as tarefas em todo o ciclo de vida da tarefa.

As APIs de atribuição fornecem os seguintes recursos-chave:

•   [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-1.0) - O objeto central de atribuições API. Representa uma tarefa ou unidade de trabalho designada a um aluno ou membro da equipe em uma classe como parte de seu estudo.
•   [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-1.0) - Representa os recursos que um indivíduo (ou grupo) apresenta para uma tarefa e a nota e feedback associados para essa tarefa.
•   [educationResource](/graph/api/resources/educationresource?view=graph-rest-1.0) - Representa o objeto de aprendizagem que está sendo designado ou apresentado. Um **educaçãoResource** está associado a um **educationAssignment** e/ou a um **educationSubmission**.


Com a API de tarefas, o seu aplicativo pode interagir com o serviço de tarefas fora do Microsoft Teams. O Microsoft Teams cuida da distribuição, das datas de conclusão e das notas, enquanto o sistema pode fornecer uma experiência avançada de aprendizagem aos alunos.
Vejamos a seguir exemplos de alguns cenários habilitados pela API de tarefas:

- [Adicionar uma tarefa que se vincula ao seu aplicativo](/graph/api/educationclass-post-assignments?view=graph-rest-1.0) 
- [Atribuir resultados como notas a alunos individuais para as tarefas vinculadas ao seu aplicativo](/graph/api/educationoutcome-update?view=graph-rest-1.0)
- [Criar um painel do aluno para mostrar as tarefas cuja data de entrega já passou](/graph/api/educationclass-list-assignments?view=graph-rest-1.0)


### <a name="enable-school-admins-to-manage-identity-and-roster-sync-using-school-data-sync-management-preview"></a>Permitir que os diretores de escola gerenciem a identidade e a sincronização da lista de participação usando o Gerenciamento do School Data Sync (visualização)

A [Sincronização de Dados Escolares](https://sds.microsoft.com/) ajuda a automatizar o processo de importação e sincronização da identidade do aluno e dos dados de lista de participação a partir de sistemas de informações do aluno com o Azure Active Directory (Azure AD) e o Microsoft 365. Após as informações serem sincronizadas, você pode usar as APIs de lista de participação para ler as informações da lista nos aplicativos. Se você for um integrador de sistema configurando a integração do Sistema de Informações do Aluno de uma escola com a School Data Sync, use as [APIs de gerenciamento do SDS](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta) do Microsoft Graph para configurar a sincronização de um arquivo CSV ou de um conector da API do SIS compatível.

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
  - [Usar as APIs de tarefa](/graph/api/resources/educationassignment?view=graph-rest-1.0)
  - [Usar as APIs de gerenciamento de SDS](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta)
- Experimente as APIs de educação no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Explore os seguintes exemplos relacionados ao setor educacional:
  - [Exemplo de SSO e lista de participantes em .NET](https://github.com/OfficeDev/O365-EDU-AspNetMVC-Samples)
  - [Exemplo de APIs de gerenciamento de perfil](https://github.com/OfficeDev/O365-EDU-SDS-AspNetMVC-Samples) 



