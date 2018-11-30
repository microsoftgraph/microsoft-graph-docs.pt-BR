---
title: Uso da API do Graph para Intune
description: " Implantações híbridas de Intune não são suportadas. "
ms.openlocfilehash: 2502b5209e9935fc923570947c38c0467534f4ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037983"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Trabalhando com o Intune no Microsoft Graph  

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.

A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.  

Em cenários de gerenciamento de dispositivo móvel (MDM), a API do Graph para Intune oferece suporte a implantações autônomas; não há suporte para[implantações híbridas](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) do Intune. 

## <a name="using-the-intune-graph-api"></a>Uso da API do Graph para Intune

Intune fornece dados para o Microsoft Graph da mesma forma, como outros serviços em nuvem, com a navegação de informações e a relação de entidade avançada.Use o Microsoft Graph para combinar informações de outros serviços e Intune construa ricas aplicativos de serviço entre para profissionais de TI ou usuários finais.     

Veja um exemplo de como determinar se um aplicativo está instalado no dispositivo de um usuário: 

1. Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário: 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. Em seguida, exiba a lista de aplicativos do seu locatário: 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-graph-permission-scopes"></a>Usando escopos de permissão do gráfico

Gráfico Microsof controla o acesso a recursos usando escopos de permissão. Como desenvolvedor, você deve especificar os escopos de permissão necessários para acessar os recursos do Intune. Normalmente, você deve especificar os escopos de permissão necessários no portal do Azure Active Directory. Para saber mais, veja [Escopos de permissão do Microsoft Graph](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) e [Escopos de permissão do Intune](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).

## <a name="to-use-the-table-of-contents-on-the-microsoft-graph-site"></a>Usar o sumário no site do Microsoft Graph
  
Você pode procurar o sumário (no painel esquerdo do site) para localizar as partes da documentação do Intune gráfico API e recursos que você deseja ver.

1. Clique em **Referência /Beta** para abrir os docs beta.
2. Role para baixo e clique em **Intune**.
3. Continue a clicar em subseções abaixo **Intune** das partes da API você 
