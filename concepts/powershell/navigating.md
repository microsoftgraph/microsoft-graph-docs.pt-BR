---
title: Navegar pelo SDK do Microsoft Graph PowerShell
description: O SDK do Microsoft Graph PowerShell contém um grande número de comandos. Saiba como encontrar o comando certo para o que você deseja obter.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 79c5ce415d00ba63ed6007e21248d51e721035c4
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777586"
---
# <a name="navigating-the-microsoft-graph-powershell-sdk"></a>Navegar pelo SDK do Microsoft Graph PowerShell

A API do Microsoft Graph é imensa e está crescendo o tempo todo. Por causa disso, o número de comandos no SDK do Microsoft Graph PowerShell também é muito grande. Encontrar o comando certo para o que você deseja obter pode ser desafiador, especialmente se você ainda não estiver familiarizado com o Microsoft Graph. Vamos dar uma olhada em algumas maneiras de ajudar a localizar um comando específico.

## <a name="command-naming-conventions"></a>Convenções de nomenclatura de comandos

Os comandos no SDK são gerados diretamente da [API REST](/graph/api/overview?view=graph-rest-1.0&preserve-view=true), de forma que os nomes são influenciados pela API. Você não precisa entender os detalhes da API para usar este SDK, mas ajuda a entender a Convenção de nomenclatura.

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

Para funções e ações, é um pouco mais complicado. As APIs no Microsoft Graph que são implementadas como funções ou ações de OData normalmente são nomeadas com pelo menos um verbo. O verbo do comando correspondente é baseado no verbo no nome da função ou da ação. No entanto, os verbos de comando no PowerShell têm que estar em conformidade com [as regras de nomenclatura](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands)específicas, portanto, isso pode resultar em mapeamentos de nome para comando não intuitivos.

Vamos ver alguns exemplos. A API [getschedule](/graph/api/calendar-getschedule?view=graph-rest-1.0&preserve-view=true) usa `get` e `Get` é um verbo aprovado do PowerShell, portanto, é o comando `Get-MgUserCalendarSchedule` . A API de [cancelamento](/graph/api/event-cancel?view=graph-rest-beta&preserve-view=true) em um evento por outro lado, usa um verbo não aprovado `cancel` . O verbo aprovado para cancelamento ou descontinuação de algo é `Stop` , portanto, é o comando `Stop-MgUserEvent` . Por fim, o verbo da API [snoozeReminder](/graph/api/event-snoozereminder?view=graph-rest-1.0&preserve-view=true) , `snooze` , não tem nenhum equivalente aprovado no PowerShell. Para a API como essa, o SDK usa o verbo `Invoke` , para que o comando da API seja `Invoke-MgSnoozeUserEventReminder` .

### <a name="command-nouns"></a>Substantivos de comando

Agora você pode ter notado que todos os substantivos nos comandos do SDK começam com `Mg` . Esse prefixo ajuda a evitar conflitos de nomenclatura com outros módulos do PowerShell. Com isso em mente, deve fazer sentido que os comandos como `Get-MgUser` são usados para obter um usuário. E, seguindo a Convenção do PowerShell, mesmo que o substantivo seja singular, esses mesmos comandos podem retornar vários resultados, caso nenhuma instância específica seja solicitada.

Mas e os comandos como `Get-MgUserMessage` ou `Get-MgUserMailFolderMessage` ? Ambos são um objeto [Message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) , então por quê não `Get-MgMessage` ? A resposta vem da [API de mensagens Get](/graph/api/message-get?view=graph-rest-1.0&preserve-view=true).

Observe as solicitações HTTP para esta API. Ignorando as solicitações com `/me` na URL, há duas outras maneiras de chamar esta API.

```http
GET /users/{id | userPrincipalName}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

Os caminhos correspondem aos substantivos. Para o primeiro formulário, comece com `users` e, em seguida `messages` , o comando é `Get-MgUserMessage` . No segundo formulário, comece com `users` , depois `mailFolders` , as mensagens, portanto, o comando é `Get-MgUserMailFolderMessage` .

Outra maneira de observar isso é o que é proprietário ou contém o que. O usuário possui pastas de email e as pastas de email contêm mensagens. Adicione o prefixo e você obtém `Get-MgUserMailFolderMessage` .

### <a name="listing-parameters"></a>Listando parâmetros

Depois de encontrar o comando certo, você pode examinar todos os parâmetros disponíveis usando o `Get-Help` comando. Por exemplo, o comando a seguir lista todos os parâmetros disponíveis para o `Get-MgUser` comando.

```powershell
Get-Help Get-MgUser -Detailed
```

## <a name="finding-available-commands"></a>Localizando comandos disponíveis

Às vezes, apenas conhecer as convenções de nomenclatura não é suficiente para adivinhar o comando correto. Nesse caso, você pode usar o `Get-Command` comando para pesquisar os comandos disponíveis no SDK. Por exemplo, se estiver procurando por comandos relacionados ao Microsoft Teams, você poderá executar o comando a seguir.

```powershell
Get-Command -Module Microsoft.Graph* *team*
```
