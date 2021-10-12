---
title: Começar com o Microsoft Graph PowerShell SDK
description: Começar a usar o Microsoft Graph PowerShell SDK usando-o para executar algumas tarefas básicas.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 623c034622054150ff6b58b97e063f3e833489de
ms.sourcegitcommit: f7956d25472a55af03be83b6ab986a7149a7ac88
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/12/2021
ms.locfileid: "60270310"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a>Começar com o Microsoft Graph PowerShell SDK

Neste guia, você usará o Microsoft Graph PowerShell SDK para executar algumas tarefas básicas. Se você ainda não [instalou o SDK,](installation.md)faça isso antes de seguir este guia.

## <a name="api-version"></a>Versão da API

Por padrão, o SDK usa o [Microsoft Graph API REST v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=true). Você pode alterar isso usando o `Select-MgProfile` comando.

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a>Autenticação

O SDK do PowerShell dá suporte a dois tipos de autenticação: acesso delegado e acesso somente a aplicativos. Neste guia, você usará o acesso delegado para fazer logon como usuário, concederá consentimento ao SDK para agir em seu nome e chamará o Microsoft Graph.

Para obter detalhes sobre como usar o acesso somente a aplicativos para cenários autônomos, consulte [Use app-only authentication with the Microsoft Graph PowerShell SDK](app-only.md).

### <a name="determine-required-permission-scopes"></a>Determinar escopos de permissão necessários

Cada API no microsoft Graph é protegida por um ou mais escopos de permissão. O logon do usuário deve consentir com um dos escopos necessários para as APIs que você planeja usar. Neste exemplo, vamos usar as SEGUINTES APIs.

- [Listar usuários](/graph/api/user-list?view=graph-rest-1.0&preserve-view=true) para encontrar a ID do usuário conectado
- [List joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true) to get the Teams the user is a member of.
- [Listar canais](/graph/api/channel-list?view=graph-rest-1.0&preserve-view=true) para obter os canais em uma equipe.
- [Enviar mensagem](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) para enviar uma mensagem para um canal de equipe.

O `User.Read.All` escopo de permissão habilita as duas primeiras chamadas e o escopo `Group.ReadWrite.All` habilita o restante. Essas permissões exigem uma conta de administrador.

### <a name="sign-in"></a>Entrar

Use o `Connect-MgGraph` comando para entrar com os escopos necessários. Você precisará entrar com uma conta de administrador para consentir com os escopos necessários.

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

O comando solicita que você acesse uma página da Web para entrar usando um código de dispositivo. Depois de fazer isso, o comando indica sucesso com uma `Welcome To Microsoft Graph!` mensagem. Você só precisa fazer isso uma vez por sessão.

> [!TIP]
> Você pode adicionar permissões adicionais repetindo o `Connect-MgGraph` comando com os novos escopos de permissão.

## <a name="call-microsoft-graph"></a>Chamar o Microsoft Graph

Agora que você está assinado, você pode começar a fazer chamadas para o Microsoft Graph.

### <a name="get-the-signed-in-user"></a>Obter o usuário com assinatura

Nesta seção, você localizará o usuário que está assinado e obterá sua ID de usuário. Você precisará disso para usar como parâmetro para os outros comandos que você usará mais tarde. Comece executando o seguinte comando.

```powershell
Get-MgUser
```

Isso causa uma listagem de usuários em sua Microsoft 365 organização.

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

Você pode usar um [filtro OData para](../query-parameters.md#filter-parameter) ajudar a localizar o usuário específico que deseja. Execute o seguinte comando, `Megan Bowen` substituindo pelo nome de exibição do usuário com o que você se inscreveu.

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

Verifique se funcionou inserindo o seguinte.

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a>Listar as equipes ingressáveis do usuário

Agora use a ID do usuário como um parâmetro para o `Get-MgUserJoinedTeam` comando.

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

Assim como o `Get-MgUser` comando, isso fornece uma lista de equipes. Selecione uma das equipes ingressada pelo usuário e copie seu `Id` .

### <a name="list-team-channels"></a>Listar canais de equipe

Agora use a ID da equipe como um parâmetro para o comando, seguindo um padrão semelhante de listagem de todos os canais e filtrando a lista para obter o canal específico que `Get-MgTeamChannel` você deseja.

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId ID_FROM_PREVIOUS_STEP -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a>Enviar uma mensagem

Agora que você tem a ID da Equipe e a ID do canal, você pode postar uma mensagem no canal. Use o seguinte comando para enviar a mensagem.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

Esse comando difere dos comandos anteriores que você usou. Em vez de apenas consultar dados, ele está realmente criando algo. No Microsoft Graph, isso se converte em HTTP e requer um objeto no `POST` corpo dessa postagem. Nesse caso, o objeto é [um chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0&preserve-view=true). Observe que o `-Body` parâmetro para o comando mapeia para a propriedade em `body` `chatMessage` . Outras propriedades são mapeadas de maneira semelhante, para que você possa alterar a mensagem enviada. Por exemplo, para enviar uma mensagem urgente, use o seguinte comando.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

### <a name="sign-out"></a>Sair

Use o `Disconnect-MgGraph` comando para sair.

```powershell
Disconnect-MgGraph
```

## <a name="next-steps"></a>Próximos passos

- [Saiba como navegar no SDK](navigating.md)
- [Usar autenticação somente aplicativo com o Microsoft Graph PowerShell SDK](app-only.md)
