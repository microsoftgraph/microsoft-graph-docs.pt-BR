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
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a>Introdução ao SDK do Microsoft Graph PowerShell

Neste guia, você usará o SDK do Microsoft Graph PowerShell para realizar algumas tarefas básicas. Se você ainda não [instalou o SDK](installation.md), faça isso antes de seguir este guia.

## <a name="api-version"></a>Versão da API

Por padrão, o SDK usa a [API REST do Microsoft Graph v 1.0](/graph/api/overview?view=graph-rest-1.0). Você pode alterar isso usando o `Select-MgProfile` comando.

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a>Autenticação

O SDK do PowerShell oferece suporte a dois tipos de autenticação: acesso delegado e acesso somente de aplicativo. Neste guia, você usará o acesso delegado para fazer logon como um usuário, conceder consentimento ao SDK para atuar em seu nome e chamar o Microsoft Graph.

Para obter detalhes sobre como usar o acesso somente de aplicativo para cenários autônomos, consulte [usar a autenticação somente aplicativo com o SDK do PowerShell do Microsoft Graph](app-only.md).

### <a name="determine-required-permission-scopes"></a>Determinar os escopos de permissão necessários

Cada API no Microsoft Graph é protegida por um ou mais escopos de permissão. O logon do usuário deve ser consentido em um dos escopos necessários para as APIs que você planeja usar. Neste exemplo, usaremos as seguintes APIs.

- [Listar usuários](/graph/api/user-list?view=graph-rest-1.0) para encontrar a ID de usuário do usuário conectado
- [Liste joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) para obter as equipes das quais o usuário é membro.
- [Listar canais](/graph/api/channel-list?view=graph-rest-1.0) para obter os canais de uma equipe.
- [Enviar mensagem](/graph/api/channel-post-messages?view=graph-rest-1.0) para enviar uma mensagem para um canal de equipe.

O `User.Read.All` escopo de permissão habilitará as duas primeiras chamadas, e o `Group.ReadWrite.All` escopo habilitará o restante. Essas permissões exigem uma conta de administrador.

### <a name="sign-in"></a>Entrar

Use o `Connect-MgGraph` comando para entrar com os escopos necessários. Você precisará entrar com uma conta de administrador para se concordar com os escopos necessários.

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

O comando solicita que você acesse uma página da Web para entrar usando um código de dispositivo. Depois de fazer isso, o comando indica êxito com uma `Welcome To Microsoft Graph!` mensagem. Você só precisa fazer isso uma vez por sessão.

> [!TIP]
> Você pode adicionar permissões adicionais repetindo o `Connect-MgGraph` comando com os novos escopos de permissão.

## <a name="call-microsoft-graph"></a>Chamar o Microsoft Graph

Agora que você está conectado, você pode começar a fazer chamadas para o Microsoft Graph.

### <a name="get-the-signed-in-user"></a>Obter o usuário conectado

Nesta seção, você localizará o usuário conectado e obterá sua ID de usuário. Você precisará usar como um parâmetro para os outros comandos que você usará posteriormente. Inicie executando o seguinte comando.

```powershell
Get-MgUser
```

Isso gera uma listagem de usuários na sua organização do Microsoft 365.

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

Você pode usar um [filtro OData](../query-parameters.md#filter-parameter) para ajudar a localizar o usuário específico desejado. Execute o comando a seguir, substituindo `Megan Bowen` pelo nome de exibição do usuário com o qual você entrou.

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

Verifique se funcionou, inserindo o seguinte.

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a>Listar as equipes Unidas do usuário

Agora use a ID do usuário como um parâmetro para o `Get-MgUserJoinedTeam` comando.

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

Assim como o `Get-MgUser` comando, isso fornece uma lista de equipes. Selecione uma das equipes Unidas do usuário e use seu `DisplayName` para filtrar a lista.

```powershell
$team = Get-MgUserJoinedTeam -UserId $user.Id -Filter "displayName eq 'Sales and Marketing'"
```

### <a name="list-team-channels"></a>Listar Canais de equipe

Agora use a ID da equipe como um parâmetro para o `Get-MgTeamChannel` comando, seguindo um padrão semelhante de listar todos os canais e, em seguida, filtrando a lista para obter o canal específico desejado.

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId $team.Id -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a>Enviar uma mensagem

Agora que você tem a ID da equipe e a ID do canal, é possível postar uma mensagem para o canal. Use o comando a seguir para enviar a mensagem.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

Este comando difere dos comandos anteriores que você usou. Em vez de apenas consultar dados, ele está realmente criando algo. No Microsoft Graph, isso é convertido em HTTP `POST` e requer um objeto no corpo dessa postagem. Nesse caso, o objeto é um [chat](/graph/resources/chatmessage?view=graph-rest-1.0). Observe que o `-Body` parâmetro para o comando é mapeado para a `body` propriedade em `chatMessage` . Outras propriedades são mapeadas de forma semelhante, para que você possa alterar a mensagem enviada. Por exemplo, para enviar uma mensagem urgente, use o comando a seguir.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

## <a name="next-steps"></a>Próximas etapas

- [Saiba como navegar no SDK](navigating.md)
- [Usar a autenticação somente de aplicativo com o SDK do Microsoft Graph PowerShell](app-only.md)
