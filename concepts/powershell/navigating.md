---
title: Navegando o SDK do Microsoft Graph PowerShell
description: O Microsoft Graph PowerShell SDK contém um grande número de comandos. Saiba como encontrar o comando certo para o que você deseja alcançar.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 40e441d620e72283f5c376422ebdc121cc461cb31d6bee8506a833ed4331b291
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230274"
---
# <a name="navigating-the-microsoft-graph-powershell-sdk"></a>Navegando o SDK do Microsoft Graph PowerShell

A API Graph microsoft é enorme e está crescendo o tempo todo. Por isso, o número de comandos no Microsoft Graph SDK do PowerShell também é muito grande. Encontrar o comando certo para o que você deseja alcançar pode ser um desafio, especialmente se você ainda não estiver familiarizado com o Microsoft Graph. Vejamos algumas maneiras de ajudar a encontrar um comando específico.

## <a name="command-naming-conventions"></a>Convenções de nomenis de comando

Os comandos no SDK são gerados diretamente da [API REST,](/graph/api/overview?view=graph-rest-1.0&preserve-view=true)portanto, os nomes são influenciados pela API. Você não precisa entender os detalhes da API para usar esse SDK, mas isso ajuda a entender a convenção de nomenis.

Os comandos do PowerShell são nomeados usando um par verbo-substantivo, como `Get-Command` ou `Update-List` . Vamos começar com o verbo.

### <a name="command-verbs"></a>Verbos de comando

Para operações REST básicas, o verbo é determinado pelo método HTTP usado para a API.

| Método HTTP | Verbo de comando | Exemplo |
|-------------|--------------|---|
| OBTER         | Obter          | `Get-MgUser` [Referência da API](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true) |
| POSTAR        | Novo          | `New-MgUserMessage` [Referência da API](/graph/api/user-post-messages?view=graph-rest-1.0&preserve-view=true) |
| PUT         | Novo          | `New-MgTeam` [Referência da API](/graph/api/team-put-teams?view=graph-rest-1.0&preserve-view=true) |
| PATCH       | Atualizar       | `Update-MgUserEvent` [Referência da API](/graph/api/event-update?view=graph-rest-1.0&preserve-view=true) |
| EXCLUIR      | Remover       | `Remove-MgDriveItem` [Referência da API](/graph/api/driveitem-delete?view=graph-rest-1.0&preserve-view=true) |

Para funções e ações, é um pouco mais complicado. APIs no Microsoft Graph que são implementadas como funções ou ações OData geralmente são nomeadas com pelo menos um verbo. O verbo do comando correspondente é baseado no verbo na função ou no nome da ação. No entanto, os verbos de comando [](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands)no PowerShell devem estar em conformidade com regras de nomenis específicas, portanto, isso pode resultar em mapeamentos não intuitivos de nome para comando.

Vejamos alguns exemplos. A API [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0&preserve-view=true) usa e é um verbo `get` aprovado do `Get` PowerShell, portanto, seu comando é `Get-MgUserCalendarSchedule` . A [](/graph/api/event-cancel?view=graph-rest-beta&preserve-view=true) API de cancelamento em um evento, por outro lado, usa um verbo não aprovado `cancel` . O verbo aprovado para cancelar ou descontinuar algo é , portanto, `Stop` seu comando é `Stop-MgUserEvent` . Por fim, o verbo da API [snoozeReminder,](/graph/api/event-snoozereminder?view=graph-rest-1.0&preserve-view=true) , não tem equivalente aprovado `snooze` pelo PowerShell. Para API é assim, o SDK usa o verbo , de modo que o `Invoke` comando da API é `Invoke-MgSnoozeUserEventReminder` .

### <a name="command-nouns"></a>Substantivos de comando

Até agora, você pode ter percebido que todos os substantivos nos comandos do SDK começam com `Mg` . Esse prefixo ajuda a evitar conflitos de nomeação com outros módulos do PowerShell. Com isso em mente, deve fazer sentido que comandos como `Get-MgUser` são usados para obter um usuário. E seguindo a convenção do PowerShell, mesmo que o substantivo seja singular, esses mesmos comandos podem retornar vários resultados se nenhuma instância específica for solicitada.

Mas e os comandos como `Get-MgUserMessage` `Get-MgUserMailFolderMessage` ou? Ambos têm um objeto [message,](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) então por que `Get-MgMessage` não? A resposta vem da [API get message](/graph/api/message-get?view=graph-rest-1.0&preserve-view=true).

Consulte as solicitações HTTP para esta API. Ignorando as solicitações com na URL, há duas outras maneiras `/me` de chamar essa API.

```http
GET /users/{id | userPrincipalName}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

Os caminhos combinam com os substantivos. Para o primeiro formulário, você começa com `users` , em `messages` seguida, para que o comando seja `Get-MgUserMessage` . No segundo formulário, você começa com `users` , em `mailFolders` seguida, mensagens, para que o comando seja `Get-MgUserMailFolderMessage` .

Outra maneira de ver isso é o que possui ou contém o quê. O usuário possui pastas de email e pastas de email contêm mensagens. Adicione o prefixo e você `Get-MgUserMailFolderMessage` obterá .

### <a name="listing-parameters"></a>Parâmetros de listagem

Depois de encontrar o comando certo, você pode examinar todos os parâmetros disponíveis usando o `Get-Help` comando. Por exemplo, o comando a seguir lista todos os parâmetros disponíveis para o `Get-MgUser` comando.

```powershell
Get-Help Get-MgUser -Detailed
```

## <a name="finding-available-commands"></a>Localizar comandos disponíveis

Às vezes, apenas conhecer as convenções de nomenis não é suficiente para adivinhar o comando certo. Nesse caso, você pode usar o `Get-Command` comando para pesquisar os comandos disponíveis no SDK. Por exemplo, se você estiver procurando comandos relacionados Microsoft Teams, execute o seguinte comando.

```powershell
Get-Command -Module Microsoft.Graph* *team*
```
