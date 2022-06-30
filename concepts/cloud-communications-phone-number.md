---
title: Gerenciar números de telefone para bots usando a API de comunicações na nuvem
description: Saiba como criar um bot que pode ser acessado por meio de um número de telefone e atribuir, cancelar a atribuição ou atualizar um número de telefone de bot usando a API de comunicações na nuvem do Microsoft Graph.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 607fbcb9dd522364ba3e5ec69e80ac2d93ddfe8b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440961"
---
# <a name="manage-phone-numbers-for-bots"></a>Gerenciar números de telefone para bots

Este artigo descreve como usar a API de comunicações na nuvem no Microsoft Graph para criar um bot que pode ser acessado por meio de um número de telefone. À medida que você cria seu bot, será útil estar familiarizado com os seguintes termos:

- **Aplicativo:** Um aplicativo hospedado no Azure, também conhecido como **bot**.

- **Instância do aplicativo:** Um objeto de usuário desabilitado que pode ser atribuído a um número de telefone que pode ser usado por um bot. Isso também é conhecido como uma [conta de recurso](/microsoftteams/manage-resource-accounts). Essa é a única maneira de um número de telefone ser atribuído a um bot.

Um aplicativo pode ter várias instâncias de aplicativo e cada locatário pode ter várias instâncias de aplicativo, conforme mostrado na imagem a seguir.

![Imagem mostrando um número de telefone com locatários com uma ou mais instâncias de aplicativo](images/communications-app-tenant.PNG)

## <a name="prerequisite-register-a-bot"></a>Pré-requisito: registrar um bot

Para começar, siga as instruções para registrar [um bot de chamada](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html). Você precisará de valores de configuração, como ID do bot, ID do aplicativo da Microsoft e senha de aplicativo da Microsoft para usar em seu código.

Adicione as permissões a seguir ao bot. Um administrador de locatários também precisa consentir com essas permissões:

- Calls.AccessMedia.All
- Calls.Initiate.All
- Calls.JoinGroupCall.All
- Calls.JoinGroupCallAsGuest.All

Para obter mais informações sobre permissões relacionadas a chamadas, consulte a [referência de Permissões](permissions-reference.md#calls-permissions).

## <a name="assign-a-phone-number-to-your-bot"></a>Atribuir um número de telefone ao bot

Atribuir um número de telefone ao bot envolve três etapas:

1. Crie uma instância de aplicativo.
2. Atribua licenças do Microsoft 365 à instância do aplicativo.
3. Atribua um número de telefone à instância do aplicativo (somente administrador de locatário).

### <a name="create-an-application-instance"></a>Criar uma instância de aplicativo

Se ele ainda não tiver sido instalado, um administrador de locatários precisará instalar o [módulo Skype for Business Online](https://www.microsoft.com/download/details.aspx?id=39366) para o PowerShell. O administrador do locatário deve entrar usando suas credenciais antes de executar o cmdlet.

Para criar uma nova instância de aplicativo, o administrador do locatário executa o seguinte cmdlet:

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId <app_id> -DisplayName <bot_display_name>`

Quando a instância do aplicativo for criada, use o cmdlet de sincronização:

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

Para obter mais informações, [consulte New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).

### <a name="assign-microsoft-365-licenses-to-your-application-instance"></a>Atribuir licenças do Microsoft 365 à instância do aplicativo

Atribua uma licença de usuário virtual à instância do aplicativo. Para obter detalhes, consulte [a licença de usuário virtual do sistema de telefonia](/microsoftteams/teams-add-on-licensing/virtual-user).

Atribua um plano de chamada à instância do aplicativo. Para obter detalhes, consulte [Planos de chamadas para o Microsoft 365](/microsoftteams/calling-plans-for-office-365).

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a>Atribuir um número de telefone à instância do aplicativo (somente administrador de locatário)

Antes de poder configurar os usuários em sua organização para fazer e receber chamadas telefônicas, você deve obter os números de telefone para eles. Para obter detalhes, consulte [Obter números de telefone para seus usuários](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users).

Para atribuir o número de telefone à instância do aplicativo, o administrador do locatário:

1. Entra no centro de administração do Teams como administrador de locatários.
2. Vai para **o Teams Administração centralizar números** > **de telefone** > **de voz**.
3. Atribui um número de telefone de serviço (formato +11D) usando o seguinte cmdlet:

   `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`
  
Quando o número de telefone de serviço for atribuído, use o cmdlet de sincronização:

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

Para obter mais informações, consulte [Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).

## <a name="unassign-a-bot-phone-number"></a>Cancelar a atribuição de um número de telefone do bot

Use o seguinte cmdlet para cancelar a atribuição de um número de telefone:

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

> [!NOTE]
> Atualmente, isso só funciona com números online e não números de DR (roteamento direto). Este é um problema conhecido.

## <a name="update-a-bot-phone-number"></a>Atualizar um número de telefone do bot

Depois de cancelar a atribuição do número, você pode atribuir um número diferente ao bot usando o seguinte cmdlet:

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a>Confira também

- [Visão geral da API de comunicações na nuvem](cloud-communications-concept-overview.md)
- [Exemplo de bot de incidente](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/RemoteMediaSamples/IncidentBot)
- [Implantando o exemplo](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/V1.0Samples/RemoteMediaSamples/README.md#deploying-the-sample)
