---
title: Introdução ao SDK do Microsoft Graph PowerShell
description: Introdução ao SDK do Microsoft Graph PowerShell usando-o realiza algumas tarefas básicas.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: eeeaee7bf45e3b8d17f866425556102eef2c1cae
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782883"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="fb5e0-103">Introdução ao SDK do Microsoft Graph PowerShell</span><span class="sxs-lookup"><span data-stu-id="fb5e0-103">Get started with the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="fb5e0-104">Neste guia, você usará o SDK do Microsoft Graph PowerShell para realizar algumas tarefas básicas.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-104">In this guide you'll use the Microsoft Graph PowerShell SDK to perform some basic tasks.</span></span> <span data-ttu-id="fb5e0-105">Se você ainda não [instalou o SDK](installation.md), faça isso antes de seguir este guia.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-105">If you haven't already [installed the SDK](installation.md), please do so before following this guide.</span></span>

## <a name="api-version"></a><span data-ttu-id="fb5e0-106">Versão da API</span><span class="sxs-lookup"><span data-stu-id="fb5e0-106">API version</span></span>

<span data-ttu-id="fb5e0-107">Por padrão, o SDK usa a [API REST do Microsoft Graph v 1.0](/graph/api/overview?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="fb5e0-107">By default, the SDK uses the [Microsoft Graph REST API v1.0](/graph/api/overview?view=graph-rest-1.0).</span></span> <span data-ttu-id="fb5e0-108">Você pode alterar isso usando o `Select-MgProfile` comando.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-108">You can change this by using the `Select-MgProfile` command.</span></span>

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a><span data-ttu-id="fb5e0-109">Autenticação</span><span class="sxs-lookup"><span data-stu-id="fb5e0-109">Authentication</span></span>

<span data-ttu-id="fb5e0-110">O SDK do PowerShell oferece suporte a dois tipos de autenticação: acesso delegado e acesso somente de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-110">The PowerShell SDK supports two types of authentication: delegated access, and app-only access.</span></span> <span data-ttu-id="fb5e0-111">Neste guia, você usará o acesso delegado para fazer logon como um usuário, conceder consentimento ao SDK para atuar em seu nome e chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-111">In this guide, you will use delegated access to login as a user, grant consent to the SDK to act on your behalf, and call the Microsoft Graph.</span></span>

<span data-ttu-id="fb5e0-112">Para obter detalhes sobre como usar o acesso somente de aplicativo para cenários autônomos, consulte [usar a autenticação somente aplicativo com o SDK do PowerShell do Microsoft Graph](app-only.md).</span><span class="sxs-lookup"><span data-stu-id="fb5e0-112">For details on using app-only access for unattended scenarios, see [Use app-only authentication with the Microsoft Graph PowerShell SDK](app-only.md).</span></span>

### <a name="determine-required-permission-scopes"></a><span data-ttu-id="fb5e0-113">Determinar os escopos de permissão necessários</span><span class="sxs-lookup"><span data-stu-id="fb5e0-113">Determine required permission scopes</span></span>

<span data-ttu-id="fb5e0-114">Cada API no Microsoft Graph é protegida por um ou mais escopos de permissão.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-114">Each API in the Microsoft Graph is protected by one or more permission scopes.</span></span> <span data-ttu-id="fb5e0-115">O logon do usuário deve ser consentido em um dos escopos necessários para as APIs que você planeja usar.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-115">The user logging in must consent to one of the required scopes for the APIs you plan to use.</span></span> <span data-ttu-id="fb5e0-116">Neste exemplo, usaremos as seguintes APIs.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-116">In this example, we'll use the following APIs.</span></span>

- <span data-ttu-id="fb5e0-117">[Listar usuários](/graph/api/user-list?view=graph-rest-1.0) para encontrar a ID de usuário do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="fb5e0-117">[List users](/graph/api/user-list?view=graph-rest-1.0) to find the user ID of the logged-in user</span></span>
- <span data-ttu-id="fb5e0-118">[Liste joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) para obter as equipes das quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-118">[List joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) to get the Teams the user is a member of.</span></span>
- <span data-ttu-id="fb5e0-119">[Listar canais](/graph/api/channel-list?view=graph-rest-1.0) para obter os canais de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-119">[List channels](/graph/api/channel-list?view=graph-rest-1.0) to get the channels in a Team.</span></span>
- <span data-ttu-id="fb5e0-120">[Enviar mensagem](/graph/api/channel-post-messages?view=graph-rest-1.0) para enviar uma mensagem para um canal de equipe.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-120">[Send message](/graph/api/channel-post-messages?view=graph-rest-1.0) to send a message to a Team channel.</span></span>

<span data-ttu-id="fb5e0-121">O `User.Read.All` escopo de permissão habilitará as duas primeiras chamadas, e o `Group.ReadWrite.All` escopo habilitará o restante.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-121">The `User.Read.All` permission scope will enable the first two calls, and the `Group.ReadWrite.All` scope will enable the rest.</span></span> <span data-ttu-id="fb5e0-122">Essas permissões exigem uma conta de administrador.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-122">These permissions require an admin account.</span></span>

### <a name="sign-in"></a><span data-ttu-id="fb5e0-123">Entrar</span><span class="sxs-lookup"><span data-stu-id="fb5e0-123">Sign in</span></span>

<span data-ttu-id="fb5e0-124">Use o `Connect-MgGraph` comando para entrar com os escopos necessários.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-124">Use the `Connect-MgGraph` command to sign in with the required scopes.</span></span> <span data-ttu-id="fb5e0-125">Você precisará entrar com uma conta de administrador para se concordar com os escopos necessários.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-125">You'll need to sign in with an admin account to consent to the required scopes.</span></span>

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

<span data-ttu-id="fb5e0-126">O comando solicita que você acesse uma página da Web para entrar usando um código de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-126">The command prompts you to go to a web page to sign in using a device code.</span></span> <span data-ttu-id="fb5e0-127">Depois de fazer isso, o comando indica êxito com uma `Welcome To Microsoft Graph!` mensagem.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-127">Once you've done that, the command indicates success with a `Welcome To Microsoft Graph!` message.</span></span> <span data-ttu-id="fb5e0-128">Você só precisa fazer isso uma vez por sessão.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-128">You only need to do this once per session.</span></span>

> [!TIP]
> <span data-ttu-id="fb5e0-129">Você pode adicionar permissões adicionais repetindo o `Connect-MgGraph` comando com os novos escopos de permissão.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-129">You can add additional permissions by repeating the `Connect-MgGraph` command with the new permission scopes.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="fb5e0-130">Chamar o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fb5e0-130">Call Microsoft Graph</span></span>

<span data-ttu-id="fb5e0-131">Agora que você está conectado, você pode começar a fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-131">Now that you're signed in, you can start making calls to Microsoft Graph.</span></span>

### <a name="get-the-signed-in-user"></a><span data-ttu-id="fb5e0-132">Obter o usuário conectado</span><span class="sxs-lookup"><span data-stu-id="fb5e0-132">Get the signed-in user</span></span>

<span data-ttu-id="fb5e0-133">Nesta seção, você localizará o usuário conectado e obterá sua ID de usuário.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-133">In this section you'll locate the signed-in user and get her user ID.</span></span> <span data-ttu-id="fb5e0-134">Você precisará usar como um parâmetro para os outros comandos que você usará posteriormente.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-134">You'll need that to use as a parameter to the other commands you'll use later.</span></span> <span data-ttu-id="fb5e0-135">Inicie executando o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-135">Start by running the following command.</span></span>

```powershell
Get-MgUser
```

<span data-ttu-id="fb5e0-136">Isso gera uma listagem de usuários na sua organização do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-136">This outputs a listing of users in your Microsoft 365 organization.</span></span>

```powershell
Id                                   DisplayName              Mail                                  UserPrincipalName
--                                   -----------              ----                                  -----------------
88d1ba68-8ff5-4de2-90ed-768c00abcfae Conf Room Adams          Adams@contoso.onmicrosoft.com         Adams@contoso.…
3103c7b9-cfe6-4cd3-a696-f88909b9a609 Adele Vance              AdeleV@contoso.OnMicrosoft.com        AdeleV@contoso…
da3a885e-2d97-41de-9347-5271ef321b58 MOD Administrator        admin@contoso.OnMicrosoft.com         admin@contoso.…
e0c6ee40-e105-476d-9597-acd061d21fcb Alex Wilber              AlexW@contoso.OnMicrosoft.com         AlexW@contoso.…
17c6bdee-8ed3-49af-a65e-71b64cca8382 Allan Deyoung            AllanD@contoso.OnMicrosoft.com        AllanD@contoso…
e5b78950-27cd-4f01-b083-eab4da97ca6a Conf Room Baker          Baker@contoso.onmicrosoft.com         Baker@contoso.…
40467725-1a58-495d-9e2f-5970c6306d8d Bianca Pisani                                                  BiancaP@contoso…
ce73bdb5-bf12-405e-ab85-40122fdd6eb7 Brian Johnson (TAILSPIN) BrianJ@contoso.onmicrosoft.com        BrianJ@contoso…
df1347a3-7ce7-4b4d-8aab-7c65b5c907b9 Cameron White                                                  CameronW@contoso…
```

<span data-ttu-id="fb5e0-137">Você pode usar um [filtro OData](../query-parameters.md#filter-parameter) para ajudar a localizar o usuário específico desejado.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-137">You can use an [OData filter](../query-parameters.md#filter-parameter) to help locate the specific user you want.</span></span> <span data-ttu-id="fb5e0-138">Execute o comando a seguir, substituindo `Megan Bowen` pelo nome de exibição do usuário com o qual você entrou.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-138">Run the following command, replacing `Megan Bowen` with the display name of the user you signed in with.</span></span>

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

<span data-ttu-id="fb5e0-139">Verifique se funcionou, inserindo o seguinte.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-139">Verify that worked by entering the following.</span></span>

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a><span data-ttu-id="fb5e0-140">Listar as equipes Unidas do usuário</span><span class="sxs-lookup"><span data-stu-id="fb5e0-140">List the user's joined Teams</span></span>

<span data-ttu-id="fb5e0-141">Agora use a ID do usuário como um parâmetro para o `Get-MgUserJoinedTeam` comando.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-141">Now use the user's ID as a parameter to the `Get-MgUserJoinedTeam` command.</span></span>

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

<span data-ttu-id="fb5e0-142">Assim como o `Get-MgUser` comando, isso fornece uma lista de equipes.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-142">Just like the `Get-MgUser` command, this gives a list of Teams.</span></span> <span data-ttu-id="fb5e0-143">Selecione uma das equipes Unidas do usuário e use seu `DisplayName` para filtrar a lista.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-143">Select one of the user's joined Teams and use its `DisplayName` to filter the list.</span></span>

```powershell
$team = Get-MgUserJoinedTeam -UserId $user.Id -Filter "displayName eq 'Sales and Marketing'"
```

### <a name="list-team-channels"></a><span data-ttu-id="fb5e0-144">Listar Canais de equipe</span><span class="sxs-lookup"><span data-stu-id="fb5e0-144">List Team channels</span></span>

<span data-ttu-id="fb5e0-145">Agora use a ID da equipe como um parâmetro para o `Get-MgTeamChannel` comando, seguindo um padrão semelhante de listar todos os canais e, em seguida, filtrando a lista para obter o canal específico desejado.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-145">Now use the Team's ID as a parameter to the `Get-MgTeamChannel` command, following a similar pattern of listing all channels, then filtering the list to get the specific channel you want.</span></span>

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId $team.Id -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a><span data-ttu-id="fb5e0-146">Enviar uma mensagem</span><span class="sxs-lookup"><span data-stu-id="fb5e0-146">Send a message</span></span>

<span data-ttu-id="fb5e0-147">Agora que você tem a ID da equipe e a ID do canal, é possível postar uma mensagem para o canal.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-147">Now that you have both the Team ID and the channel ID, you can post a message to the channel.</span></span> <span data-ttu-id="fb5e0-148">Use o comando a seguir para enviar a mensagem.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-148">Use the following command to send the message.</span></span>

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

<span data-ttu-id="fb5e0-149">Este comando difere dos comandos anteriores que você usou.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-149">This command differs from the previous commands you used.</span></span> <span data-ttu-id="fb5e0-150">Em vez de apenas consultar dados, ele está realmente criando algo.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-150">Instead of just querying data, it's actually creating something.</span></span> <span data-ttu-id="fb5e0-151">No Microsoft Graph, isso é convertido em HTTP `POST` e requer um objeto no corpo dessa postagem.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-151">In Microsoft Graph, this translates to an HTTP `POST`, and it requires an object in the body of that post.</span></span> <span data-ttu-id="fb5e0-152">Nesse caso, o objeto é um [chat](/graph/resources/chatmessage?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="fb5e0-152">In this case, the object is a [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0).</span></span> <span data-ttu-id="fb5e0-153">Observe que o `-Body` parâmetro para o comando é mapeado para a `body` propriedade em `chatMessage` .</span><span class="sxs-lookup"><span data-stu-id="fb5e0-153">Note that the `-Body` parameter to the command maps to the `body` property on `chatMessage`.</span></span> <span data-ttu-id="fb5e0-154">Outras propriedades são mapeadas de forma semelhante, para que você possa alterar a mensagem enviada.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-154">Other properties are mapped in a similar way, so you can change the message you send.</span></span> <span data-ttu-id="fb5e0-155">Por exemplo, para enviar uma mensagem urgente, use o comando a seguir.</span><span class="sxs-lookup"><span data-stu-id="fb5e0-155">For example, to send an urgent message use the following command.</span></span>

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

## <a name="next-steps"></a><span data-ttu-id="fb5e0-156">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="fb5e0-156">Next steps</span></span>

- [<span data-ttu-id="fb5e0-157">Saiba como navegar no SDK</span><span class="sxs-lookup"><span data-stu-id="fb5e0-157">Learn how to navigate the SDK</span></span>](navigating.md)
- [<span data-ttu-id="fb5e0-158">Usar a autenticação somente de aplicativo com o SDK do Microsoft Graph PowerShell</span><span class="sxs-lookup"><span data-stu-id="fb5e0-158">Use app-only authentication with the Microsoft Graph PowerShell SDK</span></span>](app-only.md)
