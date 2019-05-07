---
title: Visão geral de usuários do Microsoft Graph
description: Os usuários são a representação de uma conta de usuário corporativa ou de estudante do Azure Active Directory (Azure AD) ou uma conta da Microsoft no Microsoft Graph. O recurso **usuário** no Microsoft Graph é um hub do qual você pode acessar as relações e os recursos que são relevantes para seus usuários.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 4b9af2e4c1a7b461f6b515b48aba75d6af77d1d9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33599811"
---
# <a name="overview-of-users-in-microsoft-graph"></a><span data-ttu-id="69009-104">Visão geral de usuários do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="69009-104">Overview of users in Microsoft Graph</span></span>

<span data-ttu-id="69009-105">Os usuários são a representação de uma conta de usuário corporativa ou de estudante do Azure Active Directory (Azure AD) ou uma conta da Microsoft no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="69009-105">Users are the representation of an Azure Active Directory (Azure AD) work or school user account or a Microsoft account in Microsoft Graph.</span></span> <span data-ttu-id="69009-106">O recurso **usuário** no Microsoft Graph é um hub do qual você pode acessar as relações e os recursos que são relevantes para seus usuários.</span><span class="sxs-lookup"><span data-stu-id="69009-106">The **user** resource in Microsoft Graph is a hub from which you can access the relationships and resources that are relevant to your users.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/TUMPipN3UFI]

## <a name="develop-user-centric-applications"></a><span data-ttu-id="69009-107">Desenvolva aplicativos centrados no usuário</span><span class="sxs-lookup"><span data-stu-id="69009-107">Develop user-centric applications</span></span>

<span data-ttu-id="69009-108">Você pode usar o Microsoft Graph para acessar relações, documentos, contatos e preferências contextualmente relevantes para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="69009-108">You can use Microsoft Graph to access the relationships, documents, contacts, and preferences that are contextually relevant to the signed-in user.</span></span> <span data-ttu-id="69009-109">O recurso **usuário** oferece uma forma simples de acessar e manipular recursos do usuário sem precisar realizar chamadas adicionais, consultar informações de autenticação específicas e emitir consultas diretamente em outros recursos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="69009-109">The **user** resource provides straightforward way for you to access and manipulate user resources without having to perform additional calls, look up specific authentication information, and directly issue queries against other Microsoft Graph resources.</span></span>

<span data-ttu-id="69009-110">Para acessar as informações e os dados de um usuário, será necessário [obter acesso em nome dele](auth-v2-user.md).</span><span class="sxs-lookup"><span data-stu-id="69009-110">To access a user's information and data, you'll need to [get access on their behalf](auth-v2-user.md).</span></span> <span data-ttu-id="69009-111">Autenticar seu aplicativo com o [consentimento do administrador](permissions-reference.md) permite que você trabalhe e atualize uma gama maior de entidades associadas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="69009-111">Authenticating your application with [admin consent](permissions-reference.md) enables you to work with and update a wider range of entities associated with a user.</span></span>

### <a name="manage-your-organization"></a><span data-ttu-id="69009-112">Gerenciar sua organização</span><span class="sxs-lookup"><span data-stu-id="69009-112">Manage your organization</span></span>

<span data-ttu-id="69009-113">Crie novos usuários em sua organização ou atualize os recursos e relações de usuários existentes.</span><span class="sxs-lookup"><span data-stu-id="69009-113">Create new users in your organization or update the resources and relationships for existing users.</span></span> <span data-ttu-id="69009-114">Você pode usar o Microsoft Graph para executar as seguintes tarefas de gerenciamento de usuários:</span><span class="sxs-lookup"><span data-stu-id="69009-114">You can use Microsoft Graph to perform the following user management tasks:</span></span> 

- <span data-ttu-id="69009-115">Criar ou excluir usuários em sua organização do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="69009-115">Create or delete users in your Azure AD organization.</span></span>
- <span data-ttu-id="69009-116">Listar as associações de grupos de um usuário e determinar se um usuário é membro de um grupo.</span><span class="sxs-lookup"><span data-stu-id="69009-116">List a user's group memberships and determine whether a user is a member of a group.</span></span>
- <span data-ttu-id="69009-117">Listar os usuários subordinados a outro usuário e atribuir gerentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="69009-117">List the users who report to a user and assign managers to a user.</span></span>
- <span data-ttu-id="69009-118">Carregar ou recuperar uma foto do usuário.</span><span class="sxs-lookup"><span data-stu-id="69009-118">Upload or retrieve a photo for the user.</span></span>

### <a name="work-with-calendars-and-tasks"></a><span data-ttu-id="69009-119">Trabalhar com calendários e tarefas</span><span class="sxs-lookup"><span data-stu-id="69009-119">Work with calendars and tasks</span></span>

<span data-ttu-id="69009-120">Você pode exibir, consultar e atualizar grupos de calendários e calendários de usuários associados a um usuário, incluindo:</span><span class="sxs-lookup"><span data-stu-id="69009-120">You can view, query, and update user calendar and calendar groups associated with a user, including:</span></span>

- <span data-ttu-id="69009-121">Listar e criar eventos em um calendário de usuários.</span><span class="sxs-lookup"><span data-stu-id="69009-121">List and create events on a users calendar.</span></span>
- <span data-ttu-id="69009-122">Exibir tarefas atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="69009-122">View tasks assigned to a user.</span></span>
- <span data-ttu-id="69009-123">Encontrar horários livres para reuniões para um conjunto de usuários.</span><span class="sxs-lookup"><span data-stu-id="69009-123">Find free meeting times for a set of users.</span></span>
- <span data-ttu-id="69009-124">Obter uma lista de lembretes definidos no calendário de um usuário.</span><span class="sxs-lookup"><span data-stu-id="69009-124">Get a list of reminders set on a user's calendar.</span></span>

### <a name="administer-mail-and-handle-contacts"></a><span data-ttu-id="69009-125">Administrar o email e gerenciar contatos</span><span class="sxs-lookup"><span data-stu-id="69009-125">Administer mail and handle contacts</span></span>

<span data-ttu-id="69009-126">Você pode definir as configurações de email do usuário e as listas de contatos, e enviar emails em nome de um usuário, incluindo:</span><span class="sxs-lookup"><span data-stu-id="69009-126">You can configure user mail settings and contact lists and send mail on a user's behalf, including:</span></span>

- <span data-ttu-id="69009-127">Listar mensagens de email e enviar novos emails.</span><span class="sxs-lookup"><span data-stu-id="69009-127">List mail messages and send new mail.</span></span>
- <span data-ttu-id="69009-128">Criar e listar contatos do usuário e organizar contatos em pastas.</span><span class="sxs-lookup"><span data-stu-id="69009-128">Create and list user contacts and organize contacts in folders.</span></span>
- <span data-ttu-id="69009-129">Recuperar e atualizar as configurações e as pastas de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="69009-129">Retrieve and update mailbox folders and settings.</span></span>

### <a name="enrich-your-app-with-user-insights"></a><span data-ttu-id="69009-130">Aprimorar seu aplicativo com informações sobre o usuário</span><span class="sxs-lookup"><span data-stu-id="69009-130">Enrich your app with user insights</span></span>

<span data-ttu-id="69009-131">Maximizar a relevância no aplicativo promovendo documentos e contatos mais populares ou usados recentemente associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="69009-131">Maximize relevance in your application by promoting recently used or trending documents and contacts associated with a user.</span></span> <span data-ttu-id="69009-132">Você pode usar o Microsoft Graph para:</span><span class="sxs-lookup"><span data-stu-id="69009-132">You can use Microsoft Graph to:</span></span>

- <span data-ttu-id="69009-133">Retornar documentos visualizados e modificados recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="69009-133">Return documents recently viewed and modified by a user.</span></span>
- <span data-ttu-id="69009-134">Retornar documentos e sites mais populares relacionados à atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="69009-134">Return documents and sites trending around a user's activity.</span></span>
- <span data-ttu-id="69009-135">Listar documentos compartilhados com um usuário por email ou pelo OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="69009-135">List documents shared with a user through email or OneDrive for Business.</span></span>

## <a name="api-reference"></a><span data-ttu-id="69009-136">Referência da API</span><span class="sxs-lookup"><span data-stu-id="69009-136">API reference</span></span>
<span data-ttu-id="69009-137">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="69009-137">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="69009-138">API de Usuários no Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="69009-138">Users API in Microsoft Graph v1.0</span></span>](/graph/api/resources/users?view=graph-rest-1.0)
- [<span data-ttu-id="69009-139">API de Usuários no Microsoft Graph beta</span><span class="sxs-lookup"><span data-stu-id="69009-139">Users API in Microsoft Graph beta</span></span>](/graph/api/resources/users?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="69009-140">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="69009-140">Next steps</span></span>

- <span data-ttu-id="69009-141">Saiba mais sobre como [trabalhar com usuários](/graph/api/resources/users?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="69009-141">Learn more about how to [work with users](/graph/api/resources/users?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="69009-142">Explore seus próprios dados no recurso **usuário** no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="69009-142">Explore your own data from the **user** resource in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="69009-143">Autentique com o Microsoft Graph [em nome de um usuário](auth-v2-user.md) ou [como um daemon ou serviço autorizado por um administrador](auth-v2-service.md).</span><span class="sxs-lookup"><span data-stu-id="69009-143">Authenticate with Microsoft Graph [on behalf of a user](auth-v2-user.md) or [as a daemon or service by consent of an administrator](auth-v2-service.md).</span></span>
- <span data-ttu-id="69009-144">Configure o controle de acesso e políticas para usuários com a [API do Azure AD](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="69009-144">Set access control and policies for users with the [Azure AD API](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="69009-145">Analise as [permissões](permissions-reference.md) que serão necessárias para o aplicativo acessar dados do usuário.</span><span class="sxs-lookup"><span data-stu-id="69009-145">Review the [permissions](permissions-reference.md) your app will need to access user data.</span></span> 
<!-- This isn't really a next step; let's remove to keep the list of links concise.>
- Stay up to date with Microsoft Graph [changelog](changelog.md).
-->
