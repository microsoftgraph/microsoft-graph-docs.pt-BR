---
title: Gerenciar números de telefone para bots
description: Este artigo descreve como criar um bot alcançável por meio de um número de telefone.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 762ff0e8d166781fee4adcde64298760320d45fc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871547"
---
# <a name="manage-phone-numbers-for-bots"></a>Gerenciar números de telefone para bots 

Este artigo descreve como criar um bot alcançável por meio de um número de telefone. Ao criar o bot, será útil estar familiarizado com os seguintes termos:

- **Aplicativo** – um aplicativo hospedado no Azure, também chamado de **bot**.

- **Instância de aplicativo** – um objeto de usuário desabilitado que pode ser atribuído a um número de telefone que pode ser usado por um bot. Isso também é conhecido como uma [conta de recurso](https://docs.microsoft.com/microsoftteams/manage-resource-accounts). Essa é a única maneira de atribuir um número de telefone a um bot.

Um aplicativo pode ter várias instâncias de aplicativo, e cada locatário pode ter várias instâncias de aplicativo, conforme mostrado na imagem a seguir.

![Imagem mostrando um número de telefone com locatários com uma ou mais instâncias de aplicativo](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a>Pré-requisitos-registrar um bot
Para começar, siga as instruções para [registrar um bot de chamada](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html). Você precisará de valores de configuração como ID do bot, ID do aplicativo da Microsoft e senha do Microsoft App para usar no seu código.

Adicione as seguintes permissões ao bot. Um administrador de locatários também precisa concordar com essas permissões:

- Calls.AccessMedia.All
- Calls.Initiate.All
- Calls.JoinGroupCall.All
- Calls. JoinGroupCallAsGuest. All

Para obter mais informações sobre permissões relacionadas a chamadas, consulte a [referência de permissões](permissions-reference.md#calls-permissions).


## <a name="assign-a-phone-number-to-your-bot"></a>Atribuir um número de telefone ao bot

Atribuir um número de telefone ao bot envolve três etapas:

1.  Criar uma instância de aplicativo.
2.  Atribua uma licença de usuário virtual à sua instância de aplicativo.
3.  Atribuir um número de telefone à instância do aplicativo (somente administrador de locatário).

### <a name="create-an-application-instance"></a>Criar uma instância de aplicativo

Se ainda não tiver sido instalado, um administrador de locatários precisará instalar o [módulo do Skype for Business online](https://www.microsoft.com/download/details.aspx?id=39366) para o PowerShell. O administrador de locatários deve entrar usando suas credenciais antes de executar o cmdlet.

Para criar uma nova instância de aplicativo, o administrador de locatários executa o cmdlet a seguir.

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId “<app_id>” -DisplayName "<bot_display_name>"`

Quando a instância do aplicativo for criada, use o cmdlet Sync.

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

### <a name="assign-a-virtual-user-license-to-your-application-instance"></a>Atribuir uma licença de usuário virtual à sua instância de aplicativo

Atribua uma licença de usuário virtual à sua instância de aplicativo. Para obter detalhes, consulte [licença de usuário virtual do sistema de telefonia](https://docs.microsoft.com/microsoftteams/teams-add-on-licensing/virtual-user).

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a>Atribuir um número de telefone à instância do aplicativo (somente administrador de locatário)

Para atribuir o número de telefone à instância do aplicativo, o locatário addmin:

1. Entrar no centro de administração do Skype for Business como administrador de locatários
2. Vai para **** > **equipes do centro de administração e** > para o**administrador herdado**do Skype Skype.
3. Vai para **** > **números de telefone** de voz
4. Atribui um número de telefone de serviço (+ formato 11D) usando o cmdlet a seguir.

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`

## <a name="unassign-a-bot-phone-number"></a>Cancelar a atribuição de um número de telefone de bot

Use o cmdlet a seguir para cancelar a atribuição de um número de telefone.

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

>**Observação:** Atualmente, isso só funciona com números online e não para os números de roteamento direto (DR). Este é um problema conhecido.

## <a name="update-a-bot-phone-number"></a>Atualizar um número de telefone de bot

Depois de cancelar a atribuição do número, você pode atribuir um número diferente ao bot usando o cmdlet a seguir.

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a>Confira também

- [Exemplo de bot de incidentes](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot). 
 - Para obter detalhes sobre como implantar o, consulte [Deploying The Sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).

