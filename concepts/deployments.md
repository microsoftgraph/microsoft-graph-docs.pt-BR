---
title: Implantações de nuvens nacionais
description: Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas. Essas versões de nuvem nacional são instâncias isoladas de redes físicas e lógicas dos serviços de nuvem corporativa da Microsoft, que são confinados pelas fronteiras geográficas de países específicos e operados pela equipe local. Para saber mais, confira Nuvens nacionais da Microsoft.
ms.openlocfilehash: b0f2ab257773faa14fe59566992bb1ed0dd77959
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091550"
---
# <a name="national-cloud-deployments"></a>Implantações de nuvem nacional


Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas. Essas versões de nuvens nacionais são instâncias isoladas de redes físicas e lógicas dos serviços de nuvem corporativa da Microsoft, que são confinados pelas fronteiras geográficas de países específicos e operados pela equipe local. Para saber mais, confira [Nuvens nacionais da Microsoft](https://www.microsoft.com/pt-BR/TrustCenter/CloudServices/NationalCloud).

As nuvens nacionais atuais incluem:

- Microsoft Cloud para o Governo dos EUA
- Microsoft Cloud Germany
- Azure e Office 365 operados pela 21Vianet na China

Este artigo fornece informações sobre as diferentes implantações de nuvem nacional do Microsoft Graph e os recursos em cada implantação que estão disponíveis para os desenvolvedores.

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a>Pontos de extremidade raiz de serviço do Microsoft Graph e do Microsoft Graph Explorer

A tabela a seguir mostra os pontos de extremidade do serviço raiz do Microsoft Graph e o Microsoft Graph Explorer para cada nuvem nacional.

| National Cloud | Microsoft Graph | Microsoft Graph Explorer
|---------------------------|----------------|----------------|
| Microsoft Graph China operado pela 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Microsoft Graph Alemanha | https://graph.microsoft.de | Sem suporte. |
| Microsoft Graph para o Governo dos Estados Unidos | https://graph.microsoft.com | Sem suporte. |
| Serviço global do Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> **Nota**: os aplicativos só podem acessar dados organizacionais por meio de pontos de extremidade de nuvens nacionais. Isso significa que somente os dados em locatários registrados na nuvem nacional específica podem ser acessados. Os aplicativos que estão tentando acessar dados de consumidor associados a uma conta Microsoft pessoal através do Microsoft Graph devem usar o serviço global https://graph.microsoft.com). Os tokens de acesso adquiridos para uma implantação de nuvens nacionais não são intercambiáveis com aqueles adquiridos para o serviço global.

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a>Pontos de extremidade Azure AD OpenID Connect e OAuth2.0

A tabela a seguir lista as URLs base para os pontos de extremidade do Azure AD (Azure Active Directory) usados para adquirir tokens para chamar o Microsoft Graph para cada nuvem nacional.

| National Cloud | Ponto de extremidade do Microsoft Azure AD raiz |
|---------------------------|----------------|
| Microsoft Azure AD China operado pela 21Vianet |https://login.chinacloudapi.cn |
| Microsoft Azure AD Alemanha | https://login.microsoftonline.de |
| Microsoft Azure AD para o Governo dos Estados Unidos | https://login.microsoftonline.us |
| Microsoft Azure AD (serviço global) | https://login.microsoftonline.com |

As solicitações para autorização do Microsoft Azure AD ou dos pontos de extremidades de tokens podem ser formadas usando a URL de base específica da região apropriada. Por exemplo, para a Alemanha:

- O ponto de extremidade comum para autorização é https://login.microsoftonline.de/common/oauth2/authorize.
- O ponto de extremidade comum para token é https://login.microsoftonline.de/common/oauth2/token.

Pontos de extremidade específicos do locatário podem ser formados por meio da substituição de "comum" nas URLs acima pela ID de locatário ou um domínio verificado para o locatário. O uso de pontos de extremidade comuns ou específicos do locatário dependerá dos requisitos do aplicativo e do fluxo de autenticação que você está usando para obter tokens. Para saber mais sobre tokens de acesso do Azure AD e do Microsoft Graph, confira [Obter tokens de autenticação](./auth-overview.md).

> **Observação:** Os [pontos de extremidade de Azure autorização e token do AD v 2.0](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-appmodel-v2-overview/) estão disponíveis apenas no serviço global. Eles ainda não têm suporte para uso com implantações de nuvem nacional.

## <a name="supported-features"></a>Recursos com suporte

Os seguintes recursos do Microsoft Graph estão geralmente disponíveis (no ponto de extremidade `/v1.0`) em todas as implantações de nuvens nacionais, exceto quando indicado:

* Usuários
* Grupos
* Excel (o suporte é limitado no Microsoft Graph operado pela 21Vianet na China.)
* OneDrive (o suporte é limitado no Microsoft Graph operado pela 21Vianet na China.)
* Email do Outlook
* Calendário do Outlook
* Contatos Pessoais 
* SharePoint (o suporte é limitado no Microsoft Graph operado pela 21Vianet na China.)
* Consulta delta (o suporte varia entre diferentes recursos em cada implantação de nuvem nacional.)
* Webhooks (o suporte varia entre diferentes recursos em cada implantação de nuvem nacional.)

Os seguintes recursos adicionais do Microsoft Graph estão disponíveis na visualização (no ponto de extremidade `/beta`) em todas as implantações de nuvens nacionais, exceto quando indicado:

* Contatos organizacionais
* Aplicativos
* Entidades de serviço

Os seguintes recursos do Microsoft Graph ainda não têm suporte em implantações de nuvem nacionais:

* Microsoft Planner
* Extensões de esquema de diretório
* Extensões de tipo aberto
