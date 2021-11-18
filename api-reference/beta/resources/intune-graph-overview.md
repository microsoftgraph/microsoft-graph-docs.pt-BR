---
title: Trabalhando com o Intune no Microsoft Graph
description: A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo Portal do Azure.
author: rolyon
ms.localizationpriority: high
ms.prod: intune
ms.openlocfilehash: 835cdb2e15f942b1adef688e58cea6bd4e83879c
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044810"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Trabalhando com o Intune no Microsoft Graph  

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.  

Em cenários de gerenciamento de dispositivo móvel (MDM), a API do Microsoft Graph para Intune oferece suporte a implantações autônomas; não há suporte para[implantações híbridas](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) do Intune.

Todas as APIs do Microsoft Graph beta para o Intune são testadas e validadas pela equipe do Intune antes de serem implantadas. Para as últimas mudanças nas APIs, consulte o [changelog](/graph/changelog).

## <a name="using-the-microsoft-graph-api-for-intune"></a>Uso da API do Microsoft Graph no Intune

O Intune fornece dados para o Microsoft Graph da mesma forma que outros serviços em nuvem, com informações avançadas de entidade e navegação de relacionamento. Use o Microsoft Graph para combinar informações de outros serviços e do Intune e criar aplicativos avançados com serviços variados para profissionais de TI ou usuários finais.     

O exemplo a seguir mostra como determinar se um aplicativo está instalado no dispositivo de um usuário: 

1. Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário: 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. Em seguida, exiba a lista de aplicativos do seu locatário: 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>Uso das permissões do Microsoft Graph

O Microsoft Graph controla o acesso aos recursos por meio de permissões. Como desenvolvedor, você deve especificar as permissões necessárias para acessar os recursos do Intune. Normalmente, você deve especificar as permissões no portal do Azure Active Directory. Para saber mais, confira [Referência de permissões do Microsoft Graph](/graph/permissions-reference).

## <a name="interaction-between-microsoft-graph-apis-for-windows-updates"></a>Interação entre APIs do Microsoft Graph para as atualizações do Windows

O Microsoft Graph inclui dois conjuntos de APIs que você pode utilizar para gerenciar as atualizações do Windows: 

- [APIs do Intune](/graph/intune-concept-overview)
- [APIs de atualizações do Windows](/graph/windowsupdates-concept-overview)

Você pode utilizar qualquer uma das APIs para gerenciar as atualizações do Windows; no entanto, essas duas APIs não são compatíveis entre si. Cada um pode sobrescrever as configurações feitas pelo outro sem fornecer visibilidade a essa ação. O uso de ambas as APIs para gerenciar atualizações pode resultar em comportamentos inesperados, incluindo o que parece ser configurações temporárias para implantações de atualização que são canceladas ou modificadas sem uma causa identificada.

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

- Saiba [como usar o Azure AD](/intune/intune-graph-apis) para acessar a API do Microsoft Graph para Intune.
- Explore os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), que mostram como usar a API do Microsoft Graph para Intune no contexto dos exemplos de trabalho.
