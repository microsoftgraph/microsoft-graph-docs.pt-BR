---
title: Uso da API do Graph para Intune
description: " Não há suporte para as implantações híbridas do Intune. "
author: dougeby
ms.localizationpriority: high
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 6f283c2002212e232fdf87dc4008409590c19c45
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59052969"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Trabalhando com o Intune no Microsoft Graph  

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/cloud-platform/microsoft-intune-pricing) pelo cliente.

A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.  

Em cenários de gerenciamento de dispositivo móvel (MDM), a API do Microsoft Graph para Intune oferece suporte a implantações autônomas; não há suporte para[implantações híbridas](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) do Intune. 

## <a name="using-the-microsoft-graph-api-for-intune"></a>Uso da API do Microsoft Graph para Intune

O Intune fornece dados para a API da Microsoft Graph da mesma forma que outros serviços de nuvem fazem, com valiosas informações sobre entidades e navegação de relacionamentos. Use a API do Microsoft Graph para combinar informações de outros serviços e do Intune e criar aplicativos avançados de vários serviços para profissionais de TI ou usuários finais.     

O exemplo a seguir mostra como determinar se um aplicativo está instalado no dispositivo de um usuário: 

1. Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário: 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. Em seguida, exiba a lista de aplicativos do seu locatário: 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/

## <a name="accessing-the-microsoft-graph-api-for-intune"></a>Acessando a API do Microsoft Graph para o Intune

O Intune tem suporte para [permissões delegadas](/graph/auth-v2-user) e para [permissões do aplicativo](/graph/auth-v2-service). As permissões delegadas e de aplicativo têm suporte para operações de leitura e gravação. As permissões delegadas e de aplicativo oferecem suporte a aplicativos de locatário único, bem como a aplicativos multilocatários. Para obter mais informações sobre as permissões disponíveis por meio do Microsoft Graph, consulte [referência de permissões do Microsoft Graph](/graph/permissions-reference).

## <a name="using-permissions"></a>Usando permissões

A API do Microsoft Graph controla o acesso a recursos por meio de permissões. Como desenvolvedor, você deve especificar as permissões necessárias para acessar os recursos do Intune. Normalmente, você deve especificar as permissões no portal do Azure Active Directory. Para saber mais, confira [Referência de permissões do Microsoft Graph](/graph/permissions-reference).

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

- Saiba [como usar o Azure AD](/intune/intune-graph-apis) para acessar a API do Microsoft Graph para Intune.  
- Explore os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), que mostram como usar a API do Microsoft Graph para Intune no contexto dos exemplos de trabalho.
