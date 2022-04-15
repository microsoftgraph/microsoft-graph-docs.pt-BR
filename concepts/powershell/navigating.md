---
title: Navegando pelo SDK do Microsoft Graph PowerShell
description: O Microsoft Graph SDK do PowerShell contém um grande número de comandos. Saiba como encontrar o comando certo para o que você deseja alcançar.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 2c4135691712bcc6cbe8a32a776aa40844ec668e
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2022
ms.locfileid: "64883399"
---
# <a name="navigating-the-microsoft-graph-powershell-sdk"></a>Navegando pelo SDK do Microsoft Graph PowerShell

O Microsoft API do Graph é enorme e está crescendo o tempo todo. Por isso, o número de comandos no Microsoft Graph SDK do PowerShell também é muito grande. Encontrar o comando certo para o que você deseja alcançar pode ser desafiador, especialmente se você ainda não estiver familiarizado com o Microsoft Graph. Vamos examinar algumas maneiras de ajudar a encontrar um comando específico.

[!INCLUDE [aad-advanced-queries-note](../../includes/aad-advanced-queries-note.md)]

## <a name="command-naming-conventions"></a>Convenções de nomenclatura de comando

Os comandos no SDK são gerados diretamente da [API REST](/graph/api/overview?view=graph-rest-1.0&preserve-view=true), portanto, os nomes são influenciados pela API. Você não precisa entender os detalhes da API para usar esse SDK, mas ajuda a entender a convenção de nomenclatura.

Os comandos do PowerShell são nomeados usando um par verbo-substantivo, como `Get-Command` ou `Update-List`. Vamos começar com o verbo.

### <a name="command-verbs"></a>Verbos de comando

Para operações REST básicas, o verbo é determinado pelo método HTTP usado para a API.

| Método HTTP | Verbo de comando | Exemplo |
|-------------|--------------|---|
| OBTER         | Obter          | `Get-MgUser` [Referência de API](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true) |
| POSTAR        | Novo          | `New-MgUserMessage` [Referência de API](/graph/api/user-post-messages?view=graph-rest-1.0&preserve-view=true) |
| PUT         | Novo          | `New-MgTeam` [Referência de API](/graph/api/team-put-teams?view=graph-rest-1.0&preserve-view=true) |
| PATCH       | Atualizar       | `Update-MgUserEvent` [Referência de API](/graph/api/event-update?view=graph-rest-1.0&preserve-view=true) |
| EXCLUIR      | Remover       | `Remove-MgDriveItem` [Referência de API](/graph/api/driveitem-delete?view=graph-rest-1.0&preserve-view=true) |

Para funções e ações, é um pouco mais complicado. APIs no Microsoft Graph implementadas como funções ou ações OData normalmente são nomeadas com pelo menos um verbo. O verbo do comando correspondente baseia-se no verbo na função ou no nome da ação. No entanto, os verbos de comando no PowerShell devem estar em conformidade com regras de nomenclatura específicas [, para](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands) que isso possa resultar em mapeamentos de nome para comando não intuitivos.

Vamos examinar alguns exemplos. A API [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0&preserve-view=true) usa `get`e `Get` é um verbo aprovado do PowerShell, portanto, seu comando é `Get-MgUserCalendarSchedule`. [A API](/graph/api/event-cancel?view=graph-rest-beta&preserve-view=true) de cancelamento em um evento, por outro lado, usa um verbo não aprovado`cancel`. O verbo aprovado para cancelar ou descontinuar algo é `Stop`, portanto, o comando é `Stop-MgUserEvent`. Por fim, [o verbo da API snoozeReminder](/graph/api/event-snoozereminder?view=graph-rest-1.0&preserve-view=true) , `snooze`não tem nenhum equivalente aprovado pelo PowerShell. Para API assim, o SDK usa o verbo `Invoke`, de modo que o comando da API é `Invoke-MgSnoozeUserEventReminder`.

### <a name="command-nouns"></a>Substantivos de comando

Agora você pode ter notado que todos os substantivos nos comandos do SDK começam com `Mg`. Esse prefixo ajuda a evitar conflitos de nomenclatura com outros módulos do PowerShell. Com isso em mente, deve fazer sentido que comandos como esses `Get-MgUser` sejam usados para obter um usuário. E seguindo a convenção do PowerShell, mesmo que o substantivo seja singular, esses mesmos comandos poderão retornar vários resultados se nenhuma instância específica for solicitada.

Mas e quanto a comandos como `Get-MgUserMessage` ou `Get-MgUserMailFolderMessage`? Ambos obtêm um [objeto de](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) mensagem, então por que não `Get-MgMessage`? A resposta vem da [API de obter mensagem](/graph/api/message-get?view=graph-rest-1.0&preserve-view=true).

Examine as solicitações HTTP para essa API. Ignorando as solicitações na `/me` URL, há duas outras maneiras de chamar essa API.

```http
GET /users/{id | userPrincipalName}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

Os caminhos correspondem aos substantivos. Para o primeiro formulário, você começa com `users`, em seguida `messages`, então, o comando é `Get-MgUserMessage`. No segundo formulário, você começa com `users`, em seguida `mailFolders`, mensagens, para que o comando seja `Get-MgUserMailFolderMessage`.

Outra maneira de ver isso é o que possui ou contém o quê. O usuário possui pastas de email e as pastas de email contêm mensagens. Adicione o prefixo e você obterá `Get-MgUserMailFolderMessage`.

### <a name="listing-parameters"></a>Parâmetros de listagem

Depois de encontrar o comando certo, você pode examinar todos os parâmetros disponíveis usando o `Get-Help` comando. Por exemplo, o comando a seguir lista todos os parâmetros disponíveis para o `Get-MgUser` comando.

```powershell
Get-Help Get-MgUser -Detailed
```

## <a name="finding-available-commands"></a>Localizando comandos disponíveis

Às vezes, apenas conhecer as convenções de nomenclatura não é suficiente para adivinhar o comando certo. Nesse caso, você pode usar o comando `Get-Command` para pesquisar os comandos disponíveis no SDK. Por exemplo, se você estiver procurando comandos relacionados Microsoft Teams, poderá executar o comando a seguir.

```powershell
Get-Command -Module Microsoft.Graph* *team*
```
