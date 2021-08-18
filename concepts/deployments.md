---
title: Implantações de nuvens nacionais
description: Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas.
author: arpitha-dhanapathi
ms.openlocfilehash: 951e907eca736042cf4684811618d0f5939acc2d
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384461"
---
# <a name="national-cloud-deployments"></a>Implantações de nuvem nacional

Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas. Essas versões de nuvem nacionais são instâncias físicas e lógicas isoladas de rede dos serviços de nuvem empresariais da Microsoft que estão confinadas dentro das bordas geográficas de países específicos e operadas por funcionários locais.

As nuvens nacionais atuais incluem:

* Microsoft Cloud para o Governo dos EUA
* Microsoft Cloud Germany
* Azure e Microsoft 365 operados pela 21Vianet na China

Cada ambiente de nuvem nacional é exclusivo e diferente do ambiente global da Microsoft. É importante estar ciente de algumas dessas principais diferenças ao desenvolver aplicativos para ambientes de nuvem nacionais; por exemplo, registrar aplicativos, adquirir tokens e chamar a API do Microsoft Graph pode ser diferente.

Este artigo fornece informações sobre as diferentes implantações de nuvem Graph Microsoft e os recursos disponíveis para desenvolvedores em cada uma delas.

> **Observação:** [Conexão de Dados do Microsoft Graph](./data-connect-concept-overview.md) não dá suporte a nenhuma das implantações nacionais de nuvem.

> [!VIDEO https://www.youtube-nocookie.com/embed/R\_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>Pontos de extremidade raiz do serviço de registro de aplicativo e token

Antes de chamar as APIs do Microsoft Graph, você deve primeiro registrar seu aplicativo e adquirir um token. A tabela a seguir lista as URLs base dos pontos de extremidade Azure Active Directory (Azure AD) para registrar seu aplicativo e adquirir tokens para cada nuvem nacional.

| Nuvem nacional | Ponto de extremidade do portal do Azure AD | Ponto de extremidade do Azure AD |
| -------------- | ------------------------ | ----------------- |
| Microsoft Azure AD (serviço global) | https://portal.azure.com | `https://login.microsoftonline.com` |
| Microsoft Azure AD para o Governo dos Estados Unidos | https://portal.azure.us | `https://login.microsoftonline.us` |
| Microsoft Azure AD Alemanha | https://portal.microsoftazure.de | `https://login.microsoftonline.de` |
| Microsoft Azure AD China operado pela 21Vianet | https://portal.azure.cn | `https://login.chinacloudapi.cn` |

Para saber mais sobre os tokens de acesso do Azure AD e o Microsoft Graph, consulte [as noções básicas de autenticação.](./auth/auth-concepts.md) Para cenários de autenticação do Azure AD, consulte Noções básicas de autenticação [do Azure AD.](/azure/active-directory/develop/authentication-scenarios)

## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Pontos de extremidade raiz do serviço do Microsoft Graph e Graph Explorer

A tabela a seguir mostra os pontos de extremidade raiz do serviço para o Microsoft Graph e [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) para cada nuvem nacional.

| National Cloud | Microsoft Graph | Graph Explorer |
| -------------- | --------------- | -------------- |
| Serviço global do Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |
| Microsoft Graph para o Governo dos EUA L4 | https://graph.microsoft.us | Sem suporte. |
| Microsoft Graph para US Government L5 (DOD) | https://dod-graph.microsoft.us | Sem suporte. |
| Microsoft Graph Alemanha | https://graph.microsoft.de | Sem suporte. |
| Microsoft Graph China operado pela 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |

> [!IMPORTANT]
> Para um aplicativo no Governo dos EUA:
> 
> 
> * Se você estiver trabalhando em um ambiente Microsoft 365 GCC, continue usando os pontos de extremidade mundiais: `https://graph.microsoft.com` e `https://portal.azure.com` .
> * Se você estiver trabalhando em um ambiente Microsoft 365 GCC Alto, use: `https://portal.azure.us` e `https://graph.microsoft.us` .
> * Se você estiver trabalhando em um ambiente Microsoft 365 DoD, use `https://portal.azure.us` e `https://dod-graph.microsoft.us` .
> 
> 
> O acesso aos dados do Governo dos EUA usando o ponto de extremidade mundial será desabilitado em um futuro próximo.

> [!NOTE]
> Os aplicativos só podem acessar dados organizacionais por meio dos pontos de extremidade da nuvem nacional. Isso significa que os aplicativos só podem acessar dados em locatários registrados na nuvem nacional específica. Aplicativos que estão tentando acessar dados de consumidor associados a contas pessoais da Microsoft por meio do Microsoft Graph devem usar o serviço global `https://graph.microsoft.com` . Os tokens de acesso adquiridos para uma implantação nacional de nuvem não são intercambiáveis com aqueles adquiridos para o serviço global ou qualquer outra nuvem nacional.

## <a name="supported-features"></a>Recursos com suporte

Os seguintes recursos do Microsoft Graph estão geralmente disponíveis no ponto de extremidade em todas as implantações de nuvem `/v1.0` nacionais, exceto quando notados.

| Recursos Graph Microsoft | Microsoft Cloud para o Governo dos EUA | Microsoft Cloud China operado pela 21Vianet | Microsoft Cloud Germany |
| ------------------------ | --------------------------------- | ------------------------------------------ | ----------------------- |
| Aplicativos | ✔ | ➖ | ➖ |
| Alterar notificações (Webhooks) | ✔ | ✔ | ✔\* |
| Consulta delta | ✔ | ✔ | ➖ |
| Extensões de esquema de diretório | ✔ | ✔ | ➖ |
| Excel | ✔ | ✔\* | ✔ |
| Grupos | ✔ | ✔ | ✔ |
| OneDrive | ✔ | ✔\* | ✔ |
| Extensões de tipo aberto | ✔ | ➖ | ➖ |
| Contatos organizacionais | ✔ | ➖ | ➖ |
| Calendário do Outlook | ✔ | ✔ | ✔ |
| Email do Outlook | ✔ | ✔ | ✔ |
| Contatos pessoais | ✔ | ✔ | ✔ |
| Planner | ✔ | ✔ | ✔ |
| Relatórios | ➖ | ✔ | ➖ |
| Pesquisa (Pesquisa da Microsoft) | ➖ | ➖ | ➖ |
| Segurança | ✔ | ✔ | ✔ |
| Comunicações e Integridade do serviço | ✔ | ✔ | ✔ |
| Entidades de serviço | ✔ | ➖ | ➖ |
| SharePoint | ✔ | ✔ | ✔ |
| Teams | ✔ | ✔ | ✔ |
| Usuários | ✔ | ✔ | ✔ |

Os seguintes recursos do Microsoft Graph estão disponíveis na visualização (no ponto de extremidade) no Microsoft Cloud China e no Microsoft Cloud Germany (pontos de extremidade V1.0 para esses recursos estão disponíveis somente `/beta` no Microsoft Cloud for US Government):

* Contatos organizacionais
* Aplicativos
* Entidades de serviço

( \* ) Suporte limitado somente para serviços Exchange e OneDrive. Os serviços do Azure AD não são suportados.

> [!IMPORTANT]
> Determinados serviços e recursos que estão em regiões específicas do serviço global podem não estar disponíveis em todas as nuvens nacionais. Para descobrir quais serviços estão disponíveis, consulte [produtos disponíveis por região](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast).

Para saber mais sobre nuvens nacionais, consulte os seguintes tópicos:

* [Nuvens Nacionais da Microsoft](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
* [Microsoft 365 para o Governo dos EUA](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
* [Microsoft 365 operado pela 21Vianet](/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
* [Office 365 Germany](/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
* [Governo do Azure](https://azure.microsoft.com/global-infrastructure/government/)
* [Azure China 21Vianet](/azure/china/)
* [Azure Alemanha](/azure/germany/)
