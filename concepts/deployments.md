---
title: Implantações de nuvens nacionais
description: Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas. Essas versões de nuvem nacionais são instâncias isoladas de rede física e lógica dos serviços de nuvem corporativa da Microsoft que são confinados nas bordas geográficas de países específicos e operados pela equipe local.
ms.openlocfilehash: a4169426a65a3c2d2766e07194ff326f0fdb2434
ms.sourcegitcommit: 889096fb1821ee90ffa1b2dcce046efd6e97acef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022800"
---
# <a name="national-cloud-deployments"></a>Implantações de nuvem nacional

Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas. Essas versões de nuvem nacionais são instâncias isoladas de rede física e lógica dos serviços de nuvem corporativa da Microsoft que são confinados nas bordas geográficas de países específicos e operados pela equipe local.

As nuvens nacionais atuais incluem:

- Microsoft Cloud para o Governo dos EUA
- Microsoft Cloud Germany
- Azure e Office 365 operados pela 21Vianet na China

Cada ambiente de nuvem nacional é exclusivo e diferente do ambiente global da Microsoft. É importante estar ciente de algumas dessas diferenças importantes ao desenvolver aplicativos para ambientes de nuvem nacionais; por exemplo, registrar aplicativos, adquirir tokens e chamar a API do Microsoft Graph pode ser diferente.

Este artigo fornece informações sobre as diferentes implantações de nuvem nacional do Microsoft Graph e os recursos disponíveis para os desenvolvedores dentro de cada um.

>**Observação:** o [Microsoft Graph data Connect](https://docs.microsoft.com/graph/data-connect-concept-overview?view=graph-rest-1.0) não dá suporte a nenhuma implantação nacional de nuvem. 

> [!VIDEO https://www.youtube-nocookie.com/embed/R_3E0IVypRM]

## <a name="app-registration-and-token-service-root-endpoints"></a>Pontos de extremidade de registro de aplicativo e serviço de token

Antes de chamar as APIs do Microsoft Graph, você deve primeiro registrar seu aplicativo e adquirir um token. A tabela a seguir lista as URLs de base para os pontos de extremidade do Azure Active Directory (Azure AD) para registrar seu aplicativo e adquirir tokens para cada nuvem nacional.

| Nuvem nacional | Ponto de extremidade do portal do Azure AD| Ponto de extremidade do Azure AD|
|---------------------------|----------------|----------------|
|Microsoft Azure AD para o Governo dos Estados Unidos |https://portal.azure.us|`https://login.microsoftonline.us`|
|Microsoft Azure AD Alemanha |https://portal.microsoftazure.de|`https://login.microsoftonline.de`|
|Microsoft Azure AD China operado pela 21Vianet |https://portal.azure.cn|`https://login.chinacloudapi.cn`|
|Microsoft Azure AD (serviço global)|https://portal.azure.com |`https://login.microsoftonline.com`|

Para saber mais sobre os tokens de acesso do Azure AD e o Microsoft Graph, consulte [Basics Authentication](./auth/auth-concepts.md). Para cenários de autenticação do Azure AD, confira [noções básicas de autenticação do Azure ad](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios).


## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Pontos de extremidade raiz do serviço do Microsoft Graph e do Graph Explorer

A tabela a seguir mostra os pontos de extremidade da raiz do serviço para o Microsoft Graph e o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer) para cada nuvem nacional.

| National Cloud | Microsoft Graph | Explorador do Graph |
|---------------------------|----------------|----------------|
| Microsoft Graph para o governo dos EUA | https://graph.microsoft.us | Sem suporte. |
| Microsoft Graph para o governo dos EUA L5 (DOD) | https://dod-graph.microsoft.us | Sem suporte. |
| Microsoft Graph Alemanha | https://graph.microsoft.de | Sem suporte. |
| Microsoft Graph China operado pela 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Serviço global do Microsoft Graph | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> [!IMPORTANT]
> Se você já tiver um aplicativo no governo dos EUA e estiver usando o ponto de `https://graph.microsoft.com`extremidade internacional, recomendamos mudar para `https://graph.microsoft.us` o novo ponto de extremidade. O acesso aos dados do governo dos EUA usando o ponto de extremidade internacional está funcional no momento, mas será desabilitado em um futuro próximo.

> [!NOTE]
> Os aplicativos podem acessar apenas os dados organizacionais por meio dos pontos de extremidade da nuvem nacional. Isso significa que os aplicativos só podem acessar dados em locatários registrados na nuvem nacional específica. Os aplicativos que estão tentando acessar os dados do cliente associados às contas pessoais da Microsoft por meio do Microsoft Graph `https://graph.microsoft.com`devem usar o serviço global. Tokens de acesso adquiridos para implantação de nuvem nacional não são intercambiáveis com aqueles adquiridos para o serviço global ou qualquer outra nuvem nacional.

## <a name="supported-features"></a>Recursos com suporte

Os seguintes recursos do Microsoft Graph geralmente estão disponíveis no `/v1.0` ponto de extremidade em todas as implantações de nuvem nacionais, exceto quando observado.

| Recursos do Microsoft Graph | Microsoft Cloud para o Governo dos EUA | Microsoft Cloud China operado pela 21Vianet | Microsoft Cloud Germany |
|---------------------------|----------------|----------------|----------------|
| Usuários | ✔ | ✔ | ✔ |
| Grupos | ✔ | ✔ | ✔ |
| Excel | ✔| ✔* | ✔ |
| OneDrive | ✔ | ✔* | ✔ |
| Email do Outlook | ✔ | ✔ | ✔ |
| Calendário do Outlook | ✔ | ✔ | ✔ |
| Contatos pessoais | ✔ | ✔ | ✔ |
| SharePoint| ✔ | ✔ | ✔ |
| Planner|✔ |✔ |✔ |
| Relatórios  |➖| ✔ |➖|
| Alterar notificações (Webhooks)  | ➖|✔* |✔* |
| Consulta delta | ➖ | ✔ | ➖ |
| Extensões de esquema de diretório |➖|➖|➖|
| Extensões de tipo aberto|➖|➖|➖|
  
Os seguintes recursos adicionais do Microsoft Graph estão disponíveis na visualização (no `/beta` ponto de extremidade) em todas as implantações de nuvem nacionais, exceto quando observado:

* Contatos organizacionais
* Aplicativos
* Entidades de serviço
* Alterar notificações (Webhooks)

(*) Suporte limitado somente para o Exchange e serviços do OneDrive. Não há suporte para os serviços do Azure AD. 

> [!IMPORTANT]
> Determinados serviços e recursos que estão em regiões específicas do serviço global podem não estar disponíveis em todas as nuvens nacionais. Para descobrir quais serviços estão disponíveis, consulte [produtos disponíveis por região](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast).


Para saber mais sobre nuvens nacionais, confira os seguintes tópicos:
- [Nuvens nacionais da Microsoft](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
- [Office 365 para o governo dos EUA](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
- [Office 365 operado pela 21Vianet](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
- [Office 365 Germany](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
- [Governo do Azure](https://azure.microsoft.com/global-infrastructure/government/)
- [Azure da 21Vianet da China](https://docs.microsoft.com/azure/china/)
- [Azure Alemanha](https://docs.microsoft.com/azure/germany/)
