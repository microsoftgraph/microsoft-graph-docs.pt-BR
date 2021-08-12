---
title: Gerenciar números de telefone para bots
description: Este artigo descreve como criar um bot que é acessível por meio de um número de telefone.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 4f9215c0416001cd69d3fb4ad0728d0e858221fe1f06957e3251d0a253a7f791
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246442"
---
# <a name="manage-phone-numbers-for-bots"></a>Gerenciar números de telefone para bots 

Este artigo descreve como criar um bot que é acessível por meio de um número de telefone. À medida que você cria seu bot, será útil estar familiarizado com os seguintes termos:

- **Aplicativo** – Um aplicativo hospedado no Azure, também conhecido como **bot**.

- **Instância do** aplicativo – Um objeto de usuário desabilitado que pode ser atribuído a um número de telefone que pode ser usado por um bot. Isso também é conhecido como uma [conta de recurso](/microsoftteams/manage-resource-accounts). Essa é a única maneira de um número de telefone ser atribuído a um bot.

Um aplicativo pode ter várias instâncias de aplicativo e cada locatário pode ter várias instâncias de aplicativo, conforme mostrado na imagem a seguir.

![Imagem mostrando um número de telefone com locatários com uma ou mais instâncias de aplicativo](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a>Pré-requisito - Registrar um bot
Para começar, siga as instruções para registrar [um bot de chamada](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html). Você precisará de valores de configuração, como ID de bot, ID de aplicativo da Microsoft e senha de aplicativo da Microsoft para usar em seu código.

Adicione as seguintes permissões ao bot. Um administrador de locatário também precisa concordar com essas permissões:

- Calls.AccessMedia.All
- Calls.Initiate.All
- Calls.JoinGroupCall.All
- Calls.JoinGroupCallAsGuest.All

Para obter mais informações sobre permissões relacionadas a chamada, consulte [a referência Permissões](permissions-reference.md#calls-permissions).


## <a name="assign-a-phone-number-to-your-bot"></a>Atribuir um número de telefone ao bot

Atribuir um número de telefone ao bot envolve três etapas:

1.  Crie uma instância de aplicativo.
2.  Atribua Microsoft 365 licenças à instância do aplicativo.
3.  Atribua um número de telefone à instância do aplicativo (somente administrador de locatário).

### <a name="create-an-application-instance"></a>Criar uma instância de aplicativo

Se ainda não tiver sido instalado, um administrador de locatário precisará instalar o [módulo Skype for Business Online](https://www.microsoft.com/download/details.aspx?id=39366) para o PowerShell. O administrador do locatário deve entrar usando suas credenciais antes de executar o cmdlet.

Para criar uma nova instância de aplicativo, o administrador de locatário executa o cmdlet a seguir.

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId <app_id> -DisplayName <bot_display_name>`

Quando a instância do aplicativo for criada, use o cmdlet de sincronização.

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

Para obter mais informações, consulte [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).

### <a name="assign-microsoft-365-licenses-to-your-application-instance"></a>Atribuir Microsoft 365 licenças à instância do aplicativo

Atribua uma licença de usuário virtual à instância do aplicativo. Para obter detalhes, [consulte Telefone licença de usuário virtual do sistema.](/microsoftteams/teams-add-on-licensing/virtual-user)

Atribua um plano de chamada à instância do aplicativo. Para obter detalhes, consulte [Planos de chamada para Microsoft 365](/microsoftteams/calling-plans-for-office-365).

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a>Atribuir um número de telefone à instância do aplicativo (somente administrador de locatário)

Antes de poder configurar os usuários em sua organização para fazer e receber chamadas telefônicas, você deve obter os números de telefone para eles. Para obter detalhes, consulte [Obter números de telefone para seus usuários](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users).

Para atribuir o número de telefone à instância do aplicativo, o administrador do locatário:

1. Entre no centro de administração Teams como administrador de locatários.
2. Vai para **Teams Centro de administração**  >  **Voz**  >  **Telefone Números**.
3. Atribui um número de telefone de serviço (formato+11D) usando o cmdlet a seguir.

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`
  
Quando o número de telefone de serviço for atribuído, use o cmdlet de sincronização.

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

Para obter mais informações, consulte [Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).

## <a name="unassign-a-bot-phone-number"></a>Unassign a bot phone number

Use o cmdlet a seguir para desemplacar um número de telefone.

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

>**Observação:** Atualmente, isso só funciona com números online e não números de roteamento direto (DR). Este é um problema conhecido.

## <a name="update-a-bot-phone-number"></a>Atualizar um número de telefone bot

Depois de desatribuição do número, você pode atribuir um número diferente ao bot usando o cmdlet a seguir.

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a>Confira também

- [Exemplo de bot de incidente](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot). 
 - Para obter detalhes sobre como implantar, consulte [Deploying the sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).
