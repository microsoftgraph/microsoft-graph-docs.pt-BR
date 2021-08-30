---
title: Uso da API do Graph para Intune - API do Microsoft Graph
description: Lista a API do Microsoft Graph para Terminais do Intune (REST) que você pode usar para gerenciar sua organização de locatários e seus dispositivos, aplicativos, acesso e recursos.
author: rolyon
ms.localizationpriority: high
ms.prod: intune
ms.openlocfilehash: 39ef3452376f9d9805a851884dc1ad34dcd52427
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695597"
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

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

- Saiba [como usar o Azure AD](/intune/intune-graph-apis) para acessar a API do Microsoft Graph para Intune.
- Explore os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), que mostram como usar a API do Microsoft Graph para Intune no contexto dos exemplos de trabalho.
