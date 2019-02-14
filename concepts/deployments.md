---
title: Implantações de nuvens nacionais
description: Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas. Essas versões nacional de nuvem são físicas e lógicas instâncias de isolados de rede de serviços de nuvem empresarial da Microsoft que são confinados dentro das bordas geográficas determinados países e operados pela equipe de local.
ms.openlocfilehash: e32330397a75670238f090599635ca68a89f115e
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994388"
---
# <a name="national-cloud-deployments"></a>Implantações de nuvem nacional

Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas. Essas versões nacional de nuvem são físicas e lógicas instâncias de isolados de rede de serviços de nuvem empresarial da Microsoft que são confinados dentro das bordas geográficas determinados países e operados pela equipe de local.

As nuvens nacionais atuais incluem:

- Microsoft Cloud para o Governo dos EUA
- Microsoft Cloud Germany
- Azure e Office 365 operados pela 21Vianet na China

Cada ambiente de nuvem nacional é exclusivo e diferente do ambiente global da Microsoft. É importante esteja ciente de alguns dessas diferenças cruciais ao desenvolver aplicativos para ambientes de nuvem nacional; Por exemplo, o registro de aplicativos, aquisição de tokens e chamando a API do Microsoft Graph podem ser diferentes.

Este artigo fornece informações sobre as implantações de nuvem nacional diferentes do Microsoft Graph e os recursos que estão disponíveis para os desenvolvedores dentro de cada uma.

## <a name="app-registration-and-token-service-root-endpoints"></a>App registro e o token de serviço raiz pontos de extremidade

Antes de chamar as APIs do Microsoft Graph, primeiro você deve registrar seu aplicativo e adquirir um token. A tabela a seguir lista as URLs de base para os pontos de extremidade do Azure Active Directory (AD Azure) para registrar seu aplicativo e adquira tokens para cada nacional nuvem.

| Nuvem nacional | Endpoint portal do Azure AD| Ponto de extremidade do Azure AD|
|---------------------------|----------------|----------------|
|Microsoft Azure AD para o Governo dos Estados Unidos |https://portal.azure.us|`https://login.microsoftonline.us`|
|Microsoft Azure AD Alemanha |https://portal.microsoftazure.de|`https://login.microsoftonline.de`|
|Microsoft Azure AD China operado pela 21Vianet |https://portal.azure.cn|`https://login.chinacloudapi.cn`|
|Microsoft Azure AD (serviço global)|https://portal.azure.com |`https://login.microsoftonline.com`|

Para saber que mais sobre o Azure AD acessar tokens e o Microsoft Graph, consulte [obter tokens de autenticação](./auth-overview.md). Para cenários de autenticação do Azure AD, consulte [Noções básicas de autenticação do Azure AD](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios).

> **Observação:** Os [pontos de extremidade de Azure autorização e token do AD v 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) estão disponíveis apenas no serviço global. Eles ainda não têm suporte para uso com implantações de nuvem nacional.


## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Microsoft Graph e o Explorer do gráfico de pontos de extremidade da raiz de serviço

A tabela a seguir mostra os pontos de extremidade do serviço raiz para o Microsoft Graph e o [Explorer do gráfico](https://developer.microsoft.com/graph/graph-explorer) para cada nacional nuvem.

| National Cloud | Microsoft Graph | Explorador do Graph |
|---------------------------|----------------|----------------|
| Microsoft Graph para o Governo dos Estados Unidos | https://graph.microsoft.us | Sem suporte. |
| Microsoft Graph Alemanha | https://graph.microsoft.de | Sem suporte. |
| Microsoft Graph China operado pela 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Serviço global do Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> **Nota**: os aplicativos só podem acessar dados organizacionais por meio de pontos de extremidade de nuvens nacionais. Isso significa que apps só possam acessar dados em inquilinos registrados na nuvem nacional específica. Aplicativos que estão tentando acessar dados do consumidor associados a contas do Microsoft pessoais por meio do Microsoft Graph devem usar o serviço global `https://graph.microsoft.com`. Adquiridos para uma implantação de nuvem nacional de tokens de acesso não são intercambiáveis com aqueles adquirido para o serviço de global ou qualquer outro nuvem nacional.

## <a name="supported-features"></a>Recursos com suporte

Os seguintes recursos do Microsoft Graph existem disponíveis no mercado de `/v1.0` ponto de extremidade em todas as implantações de nuvem nacional, exceto onde observado.

| Recursos do Microsoft Graph | Microsoft Cloud para o Governo dos EUA | China Microsoft Cloud operado pela 21Vianet | Microsoft Cloud Germany |
|---------------------------|----------------|----------------|----------------|
| Usuários | ✔ | ✔ | ✔ |
| Grupos | ✔ | ✔ | ✔ |
| Excel | ✔| ✔* | ✔ |
| OneDrive | ✔ | ✔* | ✔ |
| Email do Outlook | ✔ | ✔ | ✔ |
| Calendário do Outlook | ✔ | ✔ | ✔ |
| Contatos Pessoais | ✔ | ✔ | ✔ |
| SharePoint| ✔ | ✔ | ✔ |
| Planner|✔ |✔ |✔ |
| Relatórios  |➖| ✔ |➖|
| Webhooks  | ➖|✔* |✔* |
| Consulta delta | ➖ | ➖| ➖ |
|Extensões de esquema de diretório |➖|➖|➖|
| Extensões de tipo aberto|➖|➖|➖|
  
Os seguintes recursos do Microsoft Graph adicionais estão disponíveis no modo de visualização (sobre o `/beta` ponto de extremidade) em todas as implantações de nuvem nacional, exceto onde observado:

* Contatos organizacionais
* Aplicativos
* Entidades de serviço

(*) Suporte limitado para apenas os serviços Exchange e OneDrive. Serviços do Azure AD não são suportados. 

 > **Importante:** Determinados serviços e recursos que estão em regiões específicas do serviço global podem não estar disponíveis em todas as nuvens nacionais. Para descobrir quais serviços estão disponíveis, consulte [produtos disponíveis por região](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast).


Para saber mais sobre nacionais nuvens, consulte os seguintes tópicos:
- [Nuvens nacional da Microsoft](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
- [Office 365 para o governo dos EUA](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
- [Office 365 operado pela 21Vianet](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
- [Alemanha do Office 365](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
- [Azure governamentais](https://azure.microsoft.com/global-infrastructure/government/)
- [China Azure 21Vianet](https://docs.microsoft.com/azure/china/)
- [Alemanha Azure](https://docs.microsoft.com/azure/germany/)
