---
title: Implantações de nuvens nacionais
description: Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas.
author: arpitha-dhanapathi
ms.localizationpriority: medium
ms.openlocfilehash: 06f3b34d8a1f41116f2e8e719ff81939f4999ecd
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924076"
---
# <a name="national-cloud-deployments"></a>Implantações de nuvem nacional

Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas. Essas versões de nuvem nacional são instâncias físicas e lógicas isoladas de rede dos serviços de nuvem empresarial da Microsoft que estão confinadas dentro das fronteiras geográficas de países específicos e operadas pela equipe local.

As nuvens nacionais atuais incluem:

* Microsoft Cloud para o Governo dos EUA
* Microsoft Cloud Germany
* Azure e Microsoft 365 operados pela 21Vianet na China

Cada ambiente de nuvem nacional é exclusivo e diferente do ambiente global da Microsoft. É importante estar ciente de algumas dessas principais diferenças ao desenvolver aplicativos para ambientes de nuvem nacionais; por exemplo, registrar aplicativos, adquirir tokens e chamar a API do Microsoft Graph pode ser diferente.

Este artigo fornece informações sobre as diferentes implantações de nuvem nacional do Microsoft Graph e os recursos que estão disponíveis para os desenvolvedores em cada uma delas.

> **Observação: o** [Microsoft Graph Data Connect](./data-connect-concept-overview.md) não dá suporte a nenhuma das implantações de nuvem nacional.

> [!VIDEO https://www.youtube-nocookie.com/embed/R\_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>Registros de aplicativo e pontos de extremidade raiz do serviço de token

Antes de chamar as APIs do Microsoft Graph, você deve primeiro registrar seu aplicativo e adquirir um token. A tabela a seguir lista as URLs base para os pontos de extremidade do Azure AD (Azure Active Directory) registrarem seu aplicativo e adquirirem tokens para cada nuvem nacional.

| Nuvem nacional | Ponto de extremidade do portal do Azure AD | Ponto de extremidade do Azure AD |
| -------------- | ------------------------ | ----------------- |
| Microsoft Azure AD (serviço global) | https://portal.azure.com | `https://login.microsoftonline.com` |
| Microsoft Azure AD para o Governo dos Estados Unidos | https://portal.azure.us | `https://login.microsoftonline.us` |
| Microsoft Azure AD Alemanha | https://portal.microsoftazure.de | `https://login.microsoftonline.de` |
| Microsoft Azure AD China operado pela 21Vianet | https://portal.azure.cn | `https://login.chinacloudapi.cn` |

Para saber mais sobre tokens de acesso e o Microsoft Graph, confira [noções básicas de autenticação](./auth/auth-concepts.md). Para cenários de autenticação do Azure AD, confira noções [básicas de autenticação do Azure AD](/azure/active-directory/develop/authentication-scenarios).

## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Pontos de extremidade raiz de serviço do Microsoft Graph e do Graph Explorer

A tabela a seguir mostra os pontos de extremidade raiz do serviço para o Microsoft Graph e o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer) para cada nuvem nacional.

| National Cloud | Microsoft Graph | Explorador do Graph |
| -------------- | --------------- | -------------- |
| Serviço global do Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |
| Microsoft Graph para GOVERNO DOS EUA L4 | https://graph.microsoft.us | Sem suporte. |
| Microsoft Graph para US Government L5 (DOD) | https://dod-graph.microsoft.us | Sem suporte. |
| Microsoft Graph Alemanha | https://graph.microsoft.de | Sem suporte. |
| Microsoft Graph China operado pela 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |

> [!IMPORTANT]
> Para um aplicativo no Governo dos EUA:
>
> * Se você estiver trabalhando em um ambiente do Microsoft 365 GCC, continue usando os pontos de extremidade em todo o mundo: `https://graph.microsoft.com` e `https://portal.azure.com`.
> * Se você estiver trabalhando em um ambiente microsoft 365 GCC High, use `https://portal.azure.us` e `https://graph.microsoft.us`.
> * Se você estiver trabalhando em um ambiente do Microsoft 365 DoD, use `https://portal.azure.us` e `https://dod-graph.microsoft.us`.

> [!NOTE]
> Os aplicativos só podem acessar dados organizacionais por meio dos pontos de extremidade de nuvem nacional. Isso significa que os aplicativos só podem acessar dados em locatários registrados na nuvem nacional específica. Os aplicativos que estão tentando acessar dados de consumidor associados a contas pessoais da Microsoft por meio do Microsoft Graph devem usar o serviço global `https://graph.microsoft.com`. Os tokens de acesso adquiridos para uma implantação de nuvem nacional não são intercambiáveis com aqueles adquiridos para o serviço global ou qualquer outra nuvem nacional.

## <a name="supported-features"></a>Recursos suportados

Os seguintes recursos do Microsoft Graph estão geralmente disponíveis `/v1.0` no ponto de extremidade em todas as implantações de nuvem nacionais, exceto quando especificado.

| Recursos do Microsoft Graph | Microsoft Cloud para o Governo dos EUA | Microsoft Cloud China operado pela 21Vianet | Microsoft Cloud Germany |
| ------------------------ | --------------------------------- | ------------------------------------------ | ----------------------- |
| Avaliações do acesso | ✔ | ✔ | ➖ |
| Aplicativos | ✔ | ➖ | ➖ |
| Alterar notificações (Webhooks) | ✔ | ✔ | ✔\* |
| Consulta delta | ✔ | ✔ | ➖ |
| Extensões de esquema de diretório | ✔ | ✔ | ➖ |
| Excel | ✔ | ➖ | ✔ |
| Grupos | ✔ | ✔ | ✔ |
| OneDrive | ✔ | ✔\* | ✔ |
| Extensões de tipo aberto | ✔ | ➖ | ➖ |
| Contatos organizacionais | ✔ | ➖ | ➖ |
| Calendário do Outlook | ✔ | ✔ | ✔ |
| Email do Outlook | ✔ | ✔ | ✔ |
| Contatos pessoais | ✔ | ✔ | ✔ |
| Privileged Identity Management | ✔ | ✔ | ➖ |
| Planner | ✔ | ✔ | ✔ |
| Relatórios | ➖ | ➖ | ➖ |
| Pesquisa (Pesquisa da Microsoft) | ✔ | ➖ | ➖ |
| Segurança | ✔ | ✔ | ✔ |
| Comunicações e integridade do serviço | ✔ | ✔ | ✔ |
| Entidades de serviço | ✔ | ➖ | ➖ |
| SharePoint | ✔ | ✔ | ✔ |
| Teams | ✔ | ✔ | ✔ |
| Comercial | ✔ | ✔ | ✔ |

Os seguintes recursos do Microsoft Graph estão disponíveis em versão prévia ( `/beta` no ponto de extremidade) no Microsoft Cloud China e no Microsoft Cloud Germany (os pontos de extremidade v1.0 para esses recursos estão disponíveis apenas no Microsoft Cloud for US Government):

* Contatos organizacionais
* Aplicativos
* Entidades de serviço

(\*) Suporte limitado somente para serviços do Exchange e do OneDrive. Não há suporte para os serviços do Azure AD.

> [!IMPORTANT]
> Determinados serviços e recursos que estão em regiões específicas do serviço global podem não estar disponíveis em todas as nuvens nacionais. Para descobrir quais serviços estão disponíveis, confira [os produtos disponíveis por região](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast).

Para saber mais sobre nuvens nacionais, confira os seguintes tópicos:

* [Nuvens Nacionais da Microsoft](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
* [Microsoft 365 para o Governo dos EUA](/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
* [Microsoft 365 operado pela 21Vianet](/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
* [Office 365 Germany](/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
* [Azure Governamental](https://azure.microsoft.com/global-infrastructure/government/)
* [Azure China 21Vianet](/azure/china/)
* [Azure Alemanha](/azure/germany/)

Explore exemplos para autenticar e trabalhar com o Azure e o Microsoft 365 em implantações de nuvem nacional:

* [Trabalhar com o Azure por meio do Microsoft Graph para o Governo dos EUA](https://github.com/SteveWinward/Azure-Samples/blob/master/AAD/SampleAadToken_AzureForGovernment.ps1)
* [Conectar-se a ambientes O365 do Governo dos EUA (GCC, GCC High e GCC DoD) usando o PowerShell do Microsoft Graph](https://github.com/microsoft/Federal-Business-Applications/tree/main/demos/powershell-gov-samples#microsoft-graph-powershell)

