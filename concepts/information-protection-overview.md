---
title: Visão geral da rotulagem da Proteção de Informações do Microsoft Purview
description: A rotulagem da Proteção de Informações do Microsoft Purview ajuda as organizações a classificar, rotular e proteger dados com base nos Rótulos de Confidencialidade do Centro de Conformidade e Segurança do Office 365.
author: tommoser
ms.localizationpriority: medium
ms.prod: security
ms.openlocfilehash: e2f93def1a27e3a19866319650122ba6d4fca09b
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884229"
---
# <a name="information-protection-overview"></a>Visão geral da Proteção de Informações

A Proteção de Informações do Microsoft Purview ajuda as organizações a classificar, rotular e proteger dados com base [na confidencialidade](/Office365/SecurityCompliance/sensitivity-labels). 

As organizações usam rótulos para auxiliar:

* Usuários no entendimento da importância das informações que estão sendo tratadas.
* Administradores de conformidade ao descobrir onde residem informações confidenciais. 
* Administradores de segurança na implantação de políticas de prevenção contra perda de dados e acesso a dados com base em informações de rótulo mais avançadas.

## <a name="why-integrate-microsoft-purview-information-protection"></a>Por que integrar a Proteção de Informações do Microsoft Purview? 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>Integrar-se à plataforma de rotulagem onipresente, atendendo milhões de usuários e dispositivos

Mais de um milhão de organizações com dezenas de milhões de usuários usam a Proteção de Informações do Microsoft Purview para classificar, rotular e proteger dados.  Além do Microsoft 365, vários serviços de DLP (prevenção contra perda de dados), plataformas de business intelligence e soluções de SaaS (software como serviço) adotaram a rotulagem da Proteção de Informações do [Microsoft Purview](https://www.microsoft.com/security/technology/information-protection) para fornecer uma experiência de classificação de dados mais avançada. 

### <a name="label-information-in-line-of-business-applications"></a>Informações de rótulo em aplicativos de linha de negócios

Os desenvolvedores corporativos usam a Proteção de Informações do Microsoft Purview para rotular e proteger informações confidenciais do cliente sobre exportação de aplicativos de linha de negócios para garantir a segurança das informações do cliente. Conectar seus aplicativos ao ecossistema da Proteção de Informações do Microsoft Purview permite que os aplicativos apliquem, [](/Office365/SecurityCompliance/sensitivity-labels) atualizem e excluam rótulos de confidencialidade em seus próprios dados de aplicativo, sem a sobrecarga de integrar um SDK completo.

## <a name="what-can-i-do-with-microsoft-purview-information-protection-label-apis-in-microsoft-graph"></a>O que posso fazer com as APIs de rótulo da Proteção de Informações do Microsoft Purview no Microsoft Graph? 

### <a name="discover-labels-available-to-a-user-or-organization"></a>Descobrir rótulos disponíveis para um usuário ou organização

Com o Microsoft Graph, você pode acessar [os rótulos de](/graph/api/resources/informationprotectionlabel) confidencialidade disponíveis para um usuário ou para a organização. Os rótulos são aplicados por aplicativos e serviços a dados em repouso ou em movimento, ajudando os usuários e os aplicativos e serviços downstream a entender a confidencialidade das informações que estão tratando.

### <a name="understand-how-to-apply-labels"></a>Entender como aplicar rótulos

Ao fornecer informações sobre o rótulo de confidencialidade existente e desejado, a API REST pode informar de forma inteligente sua aplicação das ações [](/graph/api/resources/informationprotectionaction) que devem ser executadas para aplicar corretamente o rótulo. Isso inclui ações como aplicativo de [metadados](/graph/api/resources/metadataaction) , geração [de marca d'água](/graph/api/resources/addwatermarkaction) , [proteção](/graph/api/resources/protectbytemplateaction) e muito mais.

### <a name="interpret-labels-applied-to-data"></a>Interpretar rótulos aplicados aos dados

Os aplicativos que consomem [](/graph/api/resources/metadataaction) informações que já têm metadados de rótulo de confidencialidade aplicados podem usar a API **extractLabel** para resolver metadados de rótulo para um rótulo de confidencialidade da Proteção de Informações do Microsoft Purview [.](/graph/api/resources/informationprotectionlabel) Use o rótulo para identificar as ações que devem ser executadas pelo aplicativo ao manipular ou consumir os dados rotulados. 

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [API de Proteção de Informações do Microsoft Purview no Microsoft Graph beta](/graph/api/resources/informationprotectionlabel)

## <a name="next-steps"></a>Próximas etapas

- Selecione e experimente consultas de exemplo de rotulagem da Proteção de Informações no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). Escolha **Mostrar mais exemplos** na coluna à esquerda. Use o menu para ativar a **Proteção de Informações do Microsoft Purview**.
