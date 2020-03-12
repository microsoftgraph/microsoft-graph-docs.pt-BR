---
title: Autorização para APIs lerem os relatórios de uso do Office 365
description: Os dados de relatórios acessíveis por meio da API de relatórios do Microsoft Graph são confidenciais e protegidos por permissões e funções do Azure AD (Azure Active Directory).
author: yixia
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: b62da7d042f4dc61c2ee4da648fd0b612f5caac8
ms.sourcegitcommit: dbc547a845e507aa934025f9dc73563c13b4fb90
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2020
ms.locfileid: "42606174"
---
# <a name="authorization-for-apis-to-read-office-365-usage-reports"></a>Autorização para APIs lerem os relatórios de uso do Office 365

Os dados do relatório acessíveis por meio da API de relatórios do Microsoft Graph são confidenciais. Em particular, os relatórios de uso do Office 365 são protegidos por permissões e funções do Azure AD (Azure Active Directory). As informações neste artigo se aplicam à API de relatórios que lê os relatórios de uso do Office 365.

As APIs que leem os relatórios de uso do Office 365 oferecem suporte a dois tipos de autorização:

- **Autorização no nível do aplicativo** – permite que um aplicativo leia todos os relatórios de uso de serviço sem um usuário conectado. As permissões concedidas ao aplicativo determinam a autorização. 
- **Permissão delegada pelo usuário** – permite que um aplicativo leia todos os relatórios de uso de serviço em nome do usuário conectado. Além do aplicativo ter recebido as permissões necessárias, o usuário deve ser membro de uma função de administrador limitada do Azure AD. Essa pode ser uma das seguintes funções: administrador da empresa, administrador do Exchange, administrador do SharePoint, administrador do Lync, Administrador de Serviço do Teams, Administrador de Comunicações do Teams, leitor global ou leitor de relatórios.

Se você estiver chamando as APIs do Explorador do Graph:

- O administrador de locatário do Azure AD deve conceder explicitamente o consentimento das permissões solicitadas ao aplicativo do Explorador do Graph.
- O usuário deve ser membro de uma função de administrador limitada no Azure AD, listada acima para autorização delegada pelo usuário.

>**Observação**: O Explorador do Graph não oferece suporte a autorização no nível de aplicativo.

Se você estiver chamando as APIs de um aplicativo:

- O administrador de locatário do Azure AD deve conceder explicitamente o consentimento ao aplicativo. Isso é necessário para autorização no nível de aplicativo e autorização delegada pelo usuário.
- Se você estiver usando uma autorização delegada pelo usuário, o usuário conectado deverá ser membro de uma função de administrador limitada no Azure AD.

## <a name="assign-azure-ad-roles-to-users"></a>Atribuir funções do Microsoft Azure AD aos usuários

Depois que um aplicativo receber permissões, todas as pessoas com acesso ao aplicativo (ou seja, membros do locatário do Azure AD) receberão as permissões concedidas. Para proteger ainda mais os dados de relatórios confidenciais, os administradores de locatários devem atribuir aos usuários do aplicativo as funções apropriadas do Azure AD. Para obter detalhes, confira [Permissões da função de administrador no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles-azure-portal) e [Atribuir funções de administrador e não-administrador aos usuários com o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-users-assign-role-azure-portal).

>**Observação:** você precisa ser um administrador de locatários para executar esta etapa.

Para atribuir uma função a um usuário:

1. Entre no [portal do Azure](https://portal.azure.com) (https://portal.azure.com).
2. Clique no ícone no canto superior esquerdo para expandir o menu do portal do Azure. Selecione **Azure Active Directory** > **Usuários**.
3. Clique no nome do usuário.
4. Escolha **Funções atribuídas** e, em seguida, **Adicionar atribuição**.
5. Escolha a função apropriada e clique em **Adicionar**.
