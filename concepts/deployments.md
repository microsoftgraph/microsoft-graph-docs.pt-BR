---
title: Implantações de nuvens nacionais
description: Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas.
author: arpitha-dhanapathi
ms.openlocfilehash: f4e7a29043a55ddefc5a3f5b7fe5a53911d8ee40
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754275"
---
# <a name="national-cloud-deployments"></a>Implantações de nuvem nacional

Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas. Essas versões de nuvem nacionais são instâncias isoladas de rede física e lógica dos serviços de nuvem corporativa da Microsoft que são confinados nas bordas geográficas de países específicos e operados pela equipe local.

As nuvens nacionais atuais incluem:

* Microsoft Cloud para o Governo dos EUA
* Microsoft Cloud Germany
* Azure e Microsoft 365 operado pela 21Vianet na China

Cada ambiente de nuvem nacional é exclusivo e diferente do ambiente global da Microsoft. É importante estar ciente de algumas dessas diferenças importantes ao desenvolver aplicativos para ambientes de nuvem nacionais; por exemplo, registrar aplicativos, adquirir tokens e chamar a API do Microsoft Graph pode ser diferente.

Este artigo fornece informações sobre as diferentes implantações de nuvem nacional do Microsoft Graph e os recursos disponíveis para os desenvolvedores dentro de cada um.

> **Observação:** o [Microsoft Graph data Connect](./data-connect-concept-overview.md?view=graph-rest-1.0) não dá suporte a nenhuma implantação nacional de nuvem.

> [!VIDEO https://www.youtube-nocookie.com/embed/R\_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>Pontos de extremidade de registro de aplicativo e serviço de token

Antes de chamar as APIs do Microsoft Graph, você deve primeiro registrar seu aplicativo e adquirir um token. A tabela a seguir lista as URLs de base para os pontos de extremidade do Azure Active Directory (Azure AD) para registrar seu aplicativo e adquirir tokens para cada nuvem nacional.

| Nuvem nacional | Ponto de extremidade do portal do Azure AD | Ponto de extremidade do Azure AD |
| -------------- | ------------------------ | ----------------- |
| Microsoft Azure AD (serviço global) | https://portal.azure.com | `https://login.microsoftonline.com` |
| Microsoft Azure AD para o Governo dos Estados Unidos | https://portal.azure.us | `https://login.microsoftonline.us` |
| Microsoft Azure AD Alemanha | https://portal.microsoftazure.de | `https://login.microsoftonline.de` |
| Microsoft Azure AD China operado pela 21Vianet | https://portal.azure.cn | `https://login.chinacloudapi.cn` |

Para saber mais sobre os tokens de acesso do Azure AD e o Microsoft Graph, consulte [Basics Authentication](./auth/auth-concepts.md). Para cenários de autenticação do Azure AD, confira [noções básicas de autenticação do Azure ad](/azure/active-directory/develop/authentication-scenarios).

## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Pontos de extremidade raiz do serviço do Microsoft Graph e do Graph Explorer

A tabela a seguir mostra os pontos de extremidade da raiz do serviço para o Microsoft Graph e o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer) para cada nuvem nacional.

| National Cloud | Microsoft Graph | Graph Explorer |
| -------------- | --------------- | -------------- |
| Serviço global do Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |
| Microsoft Graph para o governo dos EUA | https://graph.microsoft.us | Sem suporte. |
| Microsoft Graph para o governo dos EUA L5 (DOD) | https://dod-graph.microsoft.us | Sem suporte. |
| Microsoft Graph Alemanha | https://graph.microsoft.de | Sem suporte. |
| Microsoft Graph China operado pela 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |

> [!IMPORTANT]
> Para um aplicativo no governo dos EUA:
> 
> 
> * Se você estiver trabalhando em um ambiente Microsoft 365 GCC, continue usando os pontos de extremidade mundiais: `https://graph.microsoft.com` e `https://portal.azure.com` .
> * Se você estiver trabalhando em um ambiente High do Microsoft 365 GCC, use: `https://portal.azure.us` e `https://graph.microsoft.us` .
> * Se você estiver trabalhando em um ambiente Microsoft 365 DoD, use `https://portal.azure.us` e `https://dod-graph.microsoft.us` .
> 
> 
> O acesso aos dados do governo dos EUA usando o ponto de extremidade internacional será desabilitado em um futuro próximo.

> [!NOTE]
> Os aplicativos podem acessar apenas os dados organizacionais por meio dos pontos de extremidade da nuvem nacional. Isso significa que os aplicativos só podem acessar dados em locatários registrados na nuvem nacional específica. Os aplicativos que estão tentando acessar os dados do cliente associados às contas pessoais da Microsoft por meio do Microsoft Graph devem usar o serviço global `https://graph.microsoft.com` . Tokens de acesso adquiridos para implantação de nuvem nacional não são intercambiáveis com aqueles adquiridos para o serviço global ou qualquer outra nuvem nacional.

## <a name="supported-features"></a>Recursos com suporte

Os seguintes recursos do Microsoft Graph geralmente estão disponíveis no `/v1.0` ponto de extremidade em todas as implantações de nuvem nacionais, exceto quando observado.

| Recursos do Microsoft Graph | Microsoft Cloud para o Governo dos EUA | Microsoft Cloud China operado pela 21Vianet | Microsoft Cloud Germany |
| ------------------------ | --------------------------------- | ------------------------------------------ | ----------------------- |
| Usuários | ✔ | ✔ | ✔ |
| Grupos | ✔ | ✔ | ✔ |
| Excel | ✔ | ✔\* | ✔ |
| OneDrive | ✔ | ✔\* | ✔ |
| Email do Outlook | ✔ | ✔ | ✔ |
| Calendário do Outlook | ✔ | ✔ | ✔ |
| Contatos pessoais | ✔ | ✔ | ✔ |
| Segurança | ✔ | ✔ | ✔ |
| SharePoint | ✔ | ✔ | ✔ |
| Teams | ✔ | ✔ | ✔ |
| Planner | ✔ | ✔ | ✔ |
| Relatórios | ➖ | ✔ | ➖ |
| Contatos organizacionais | ✔ | ➖ | ➖ |
| Aplicativos | ✔ | ➖ | ➖ |
| Entidades de serviço | ✔ | ➖ | ➖ |
| Alterar notificações (Webhooks) | ✔ | ✔ | ✔\* |
| Consulta delta | ✔ | ✔ | ➖ |
| Extensões de esquema de diretório | ✔ | ✔ | ➖ |
| Extensões de tipo aberto | ✔ | ➖ | ➖ |
| Pesquisa (Microsoft Search) | ➖ | ➖ | ➖ |
 
Os seguintes recursos do Microsoft Graph estão disponíveis na visualização (no `/beta` ponto de extremidade) no Microsoft Cloud China e no Microsoft Cloud Alemanha (pontos de extremidade do v 1.0 para esses recursos estão disponíveis no Microsoft Cloud para o governo dos EUA apenas):

* Contatos organizacionais
* Aplicativos
* Entidades de serviço

( \* ) Suporte limitado somente para serviços do Exchange e do onedrive. Não há suporte para os serviços do Azure AD.

> [!IMPORTANT]
> Determinados serviços e recursos que estão em regiões específicas do serviço global podem não estar disponíveis em todas as nuvens nacionais. Para descobrir quais serviços estão disponíveis, consulte [produtos disponíveis por região](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast).

Para saber mais sobre nuvens nacionais, confira os seguintes tópicos:

* [Nuvens nacionais da Microsoft](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
* [Microsoft 365 para o governo dos EUA](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
* [Microsoft 365 operado pela 21Vianet](/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
* [Office 365 Germany](/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
* [Governo do Azure](https://azure.microsoft.com/global-infrastructure/government/)
* [Azure da 21Vianet da China](/azure/china/)
* [Azure Alemanha](/azure/germany/)