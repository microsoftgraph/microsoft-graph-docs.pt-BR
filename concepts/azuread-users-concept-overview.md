---
title: Visão geral de usuários do Microsoft Graph
description: Os usuários são a representação de uma conta de usuário corporativa ou de estudante do Azure Active Directory (Azure AD) ou uma conta da Microsoft no Microsoft Graph. O recurso **usuário** no Microsoft Graph é um hub do qual você pode acessar as relações e os recursos que são relevantes para seus usuários.
author: dkershaw10
localization_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: 26e3eb7fe76cfabfd1b8a7348f84e575bc3590dca4f532b7b39196bcd646ad81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169190"
---
# <a name="overview-of-users-in-microsoft-graph"></a>Visão geral de usuários do Microsoft Graph

Os usuários são a representação de uma conta de usuário corporativa ou de estudante do Azure Active Directory (Azure AD) ou uma conta da Microsoft no Microsoft Graph. O recurso **usuário** no Microsoft Graph é um hub do qual você pode acessar as relações e os recursos que são relevantes para seus usuários.

> [!VIDEO https://www.youtube-nocookie.com/embed/TUMPipN3UFI]

## <a name="develop-user-centric-applications"></a>Desenvolva aplicativos centrados no usuário

Você pode usar o Microsoft Graph para acessar relações, documentos, contatos e preferências contextualmente relevantes para o usuário conectado. O recurso **usuário** oferece uma forma simples de acessar e manipular recursos do usuário sem precisar realizar chamadas adicionais, consultar informações de autenticação específicas e emitir consultas diretamente em outros recursos do Microsoft Graph.

Para acessar as informações e os dados de um usuário, será necessário [obter acesso em nome dele](auth-v2-user.md). Autenticar seu aplicativo com o [consentimento do administrador](permissions-reference.md) permite que você trabalhe e atualize uma gama maior de entidades associadas a um usuário.

### <a name="manage-your-organization"></a>Gerenciar sua organização

Crie novos usuários em sua organização ou atualize os recursos e relações de usuários existentes. Você pode usar o Microsoft Graph para executar as seguintes tarefas de gerenciamento de usuários: 

- Criar ou excluir usuários em sua organização do Azure AD.
- Listar as associações de grupos de um usuário e determinar se um usuário é membro de um grupo.
- Listar os usuários subordinados a outro usuário e atribuir gerentes a um usuário.
- Carregar ou recuperar uma foto do usuário.

### <a name="work-with-calendars-and-tasks"></a>Trabalhar com calendários e tarefas

Você pode exibir, consultar e atualizar grupos de calendários e calendários de usuários associados a um usuário, incluindo:

- Listar e criar eventos no calendário de um usuário.
- Exibir tarefas atribuídas a um usuário.
- Encontrar horários livres para reuniões para um conjunto de usuários.
- Obter uma lista de lembretes definidos no calendário de um usuário.

### <a name="administer-mail-and-handle-contacts"></a>Administrar o email e gerenciar contatos

Você pode definir as configurações de email do usuário e as listas de contatos, e enviar emails em nome de um usuário, incluindo:

- Listar mensagens de email e enviar novos emails.
- Criar e listar contatos do usuário e organizar contatos em pastas.
- Recuperar e atualizar as configurações e as pastas de caixa de correio.

### <a name="enrich-your-app-with-user-insights"></a>Aprimorar seu aplicativo com informações sobre o usuário

Maximizar a relevância no aplicativo promovendo documentos e contatos mais populares ou usados recentemente associados a um usuário. Use o Microsoft Graph para:

- Retornar documentos visualizados e modificados recentemente por um usuário.
- Retornar documentos e sites mais populares relacionados à atividade do usuário.
- Listar documentos compartilhados com um usuário por email ou pelo OneDrive for Business.

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API de Usuários no Microsoft Graph v1.0](/graph/api/resources/users?view=graph-rest-1.0)
- [API de Usuários no Microsoft Graph beta](/graph/api/resources/users?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre como [trabalhar com usuários](/graph/api/resources/users?view=graph-rest-1.0).
- Explore seus próprios dados no recurso **usuário** no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
- Autentique com o Microsoft Graph [em nome de um usuário](auth-v2-user.md) ou [como um daemon ou serviço autorizado por um administrador](auth-v2-service.md).
- Configure o controle de acesso e políticas para usuários com a [API do Azure AD](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).
- Analise as [permissões](permissions-reference.md) que serão necessárias para o aplicativo acessar dados do usuário. 
<!-- This isn't really a next step; let's remove to keep the list of links concise.>
- Stay up to date with Microsoft Graph [changelog](changelog.md).
-->
