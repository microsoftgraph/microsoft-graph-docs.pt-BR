---
title: Uso da API do Graph para Intune
description: " Implantações híbridas de Intune não são suportadas. "
author: tfitzmac
ms.openlocfilehash: 9ac823fcc1e3c09bfedc57d9caf4901c95aa9142
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332729"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Trabalhando com o Intune no Microsoft Graph  

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.

A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.  

Para cenários de gerenciamento (MDM) do dispositivo móvel, a API do Microsoft Graph para Intune oferece suporte a implantações autônomo; Não há suporte para Intune [implantações híbridas](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) . 

## <a name="using-the-microsoft-graph-api-for-intune"></a>Usando a API do Microsoft Graph para Intune

O Intune fornece dados para a API da Microsoft Graph da mesma forma que outros serviços de nuvem fazem, com valiosas informações sobre entidades e navegação de relacionamentos.Use a API do Microsoft Graph para combinar informações de outros serviços e Intune construa ricas aplicativos de serviço entre para profissionais de TI ou usuários finais.     

O exemplo a seguir mostra como você pode determinar se um aplicativo está instalado em um dispositivo do usuário: 

1. Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário: 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. Em seguida, exiba a lista de aplicativos do seu locatário: 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permissions"></a>Utilização das permissões

A API do Microsoft Graph controla o acesso aos recursos por meio de permissões. Como um desenvolvedor, você deve especificar as permissões que necessárias para acessar recursos Intune. Normalmente, você deve especificar as permissões no portal do Azure Active Directory. Para obter mais informações, consulte [referência de permissões do Microsoft Graph](https://docs.microsoft.com/en-us/graph/permissions-reference).

## <a name="next-steps"></a>Próximas etapas

- Saiba [como usar o Windows Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) para acessar a API do Microsoft Graph para Intune.  
- Explore os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), que mostram como usar a API do Microsoft Graph para Intune no contexto dos exemplos de trabalho.
