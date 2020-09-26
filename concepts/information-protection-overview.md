---
title: Visão geral da rotulação de proteção de informações da Microsoft
description: O rótulo de proteção de informações da Microsoft ajuda as organizações a classificar, identificar e proteger os dados com base nos rótulos de confidencialidade do centro de conformidade e segurança do Office 365.
author: tommoser
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 599e395d82cf74a22a9c26ceab066bdf53176e0c
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288900"
---
# <a name="information-protection-overview"></a>Visão geral da proteção de informações

A proteção de informações da Microsoft ajuda as organizações a classificar, identificar e proteger os dados com base na [confidencialidade](/Office365/SecurityCompliance/sensitivity-labels). 

As organizações usam rótulos para ajudar:

* Os usuários que compreendem a importância das informações que estão sendo tratadas.
* Administradores de conformidade na descoberta de onde as informações confidenciais residem. 
* Administradores de segurança em Implantando o acesso a dados e as políticas de prevenção contra perda de dados com base em informações mais ricas de rótulo.

## <a name="why-integrate-microsoft-information-protection"></a>Por que integrar a proteção de informações da Microsoft? 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>Integre-se com a plataforma de rotulagem onipresente, servindo milhões de usuários e dispositivos

Mais de um milhão de organizações com dezenas de milhões de usuários usam a proteção de informações da Microsoft para classificar, rotular e proteger os dados.  Além do Microsoft 365, vários serviços de prevenção de perda de dados (DLP), plataformas de Business Intelligence e software como serviço (SaaS) [adotaram](https://www.microsoft.com/security/technology/information-protection) a identificação de proteção de informações da Microsoft para fornecer uma experiência de classificação de dados mais rica. 

### <a name="label-information-in-line-of-business-applications"></a>Informações de rótulo em aplicativos de linha de negócios

Os desenvolvedores corporativos usam a proteção de informações da Microsoft para rotular e proteger informações confidenciais do cliente sobre exportação de aplicativos de linha de negócios para garantir a segurança das informações do cliente. A conexão de seus aplicativos ao ecossistema de proteção de informações da Microsoft permite que os aplicativos apliquem, atualizem e excluam [Rótulos de confidencialidade](/Office365/SecurityCompliance/sensitivity-labels) em seus próprios dados de aplicativo, sem a sobrecarga da integração de um SDK completo.

## <a name="what-can-i-do-with-microsoft-information-protection-label-apis-in-microsoft-graph"></a>O que posso fazer com as APIs de rótulo de proteção de informações da Microsoft no Microsoft Graph? 

### <a name="discover-labels-available-to-a-user-or-organization"></a>Descobrir rótulos disponíveis para um usuário ou organização

Com o Microsoft Graph, você pode acessar os [Rótulos de confidencialidade](/graph/api/informationprotectionlabel?view=graph-rest-beta) disponíveis para um usuário ou organização. Os rótulos são aplicados por aplicativos e serviços aos dados em repouso ou em movimento, ajudando os usuários e os aplicativos e serviços downstream a entender a confidencialidade das informações que estão lidando.

### <a name="understand-how-to-apply-labels"></a>Entender como aplicar rótulos

Fornecendo informações sobre o rótulo de confidencialidade existente e desejado, a API REST pode informar, de forma inteligente, o aplicativo sobre as [ações](/graph/api/resources/informationprotectionaction?view=graph-rest-beta) que devem ser executadas para aplicar corretamente o rótulo. Isso inclui ações como aplicativo de [metadados](/graph/api/resources/metadataaction?view=graph-rest-beta) , geração de [marca d' água](/graph/api/resources/addwatermarkaction?view=graph-rest-beta) , [proteção](/graph/api/resources/protectbytemplateaction?view=graph-rest-beta)e muito mais.

### <a name="interpret-labels-applied-to-data"></a>Interpretar rótulos aplicados aos dados

Os aplicativos que consomem informações que já possuem [metadados de rótulo de confidencialidade](/graph/api/resources/metadataaction?view=graph-rest-beta) aplicados podem usar a API **extractLabel** para resolver metadados de rótulo para um [rótulo de confidencialidade](/graph/api/resources/informationprotectionlabel.md?view=graph-rest-beta)de proteção de informações da Microsoft. Use o rótulo para identificar as ações que devem ser tomadas pelo aplicativo ao lidar ou consumo dos dados rotulados. 

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [API de proteção de informações da Microsoft no Microsoft Graph beta](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

- Selecione e tente a proteção de informações rotular consultas de exemplo no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). Escolha **Mostrar mais exemplos** na coluna à esquerda. Use o menu para ativar a **proteção de informações da Microsoft**.
