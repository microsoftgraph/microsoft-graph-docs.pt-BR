---
title: Proteção de Informações do Microsoft Purview de rotulagem
description: Use Proteção de Informações do Microsoft Purview para classificar, rotular e proteger dados com base em rótulos de confidencialidade. Saiba como usar APIs de rótulo no Microsoft Graph.
author: tommoser
ms.localizationpriority: medium
ms.prod: security
ms.openlocfilehash: 3d1018b76e72d8fde7384d516aa12848768c63bc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444926"
---
# <a name="microsoft-purview-information-protection-labeling-overview"></a>Proteção de Informações do Microsoft Purview de rotulagem

Proteção de Informações do Microsoft Purview ajuda as organizações a classificar, rotular e proteger dados com base em [rótulos de confidencialidade](/Office365/SecurityCompliance/sensitivity-labels).

As organizações usam rótulos para ajudar:

* Usuários no entendimento da importância das informações que estão sendo tratadas.
* Administradores de conformidade ao descobrir onde residem informações confidenciais.
* Administradores de segurança na implantação de políticas de prevenção contra perda de dados e acesso a dados com base em informações de rótulo mais avançadas.

## <a name="why-integrate-with-microsoft-purview-information-protection"></a>Por que integrar com Proteção de Informações do Microsoft Purview?

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>Integrar-se à plataforma de rotulagem onipresente, atendendo milhões de usuários e dispositivos

Mais de um milhão de organizações com dezenas de milhões de usuários usam Proteção de Informações do Microsoft Purview para classificar, rotular e proteger dados.  Além do Microsoft 365, vários serviços de DLP (prevenção contra perda de dados), plataformas de business intelligence e soluções de SaaS (software como serviço) adotaram uma [rotulagem Proteção de Informações do Microsoft Purview](https://www.microsoft.com/security/technology/information-protection) para fornecer uma experiência de classificação de dados mais avançada. 

### <a name="label-information-in-line-of-business-applications"></a>Informações de rótulo em aplicativos de linha de negócios

Os desenvolvedores corporativos usam Proteção de Informações do Microsoft Purview para rotular e proteger informações confidenciais do cliente sobre exportação de aplicativos de linha de negócios para garantir a segurança das informações do cliente. Conectar seus aplicativos ao ecossistema Proteção de Informações do Microsoft Purview permite que os aplicativos apliquem, atualizem e excluam rótulos de confidencialidade em seus próprios dados de aplicativo, sem a sobrecarga de integrar um SDK completo.[](/Office365/SecurityCompliance/sensitivity-labels)

## <a name="what-can-i-do-with-microsoft-purview-information-protection-label-apis-in-microsoft-graph"></a>O que posso fazer com apIs Proteção de Informações do Microsoft Purview rótulo no Microsoft Graph? 

### <a name="discover-labels-available-to-a-user-or-organization"></a>Descobrir rótulos disponíveis para um usuário ou organização

Com o Microsoft Graph, você pode acessar [os rótulos de](/graph/api/resources/informationprotectionlabel) confidencialidade disponíveis para um usuário ou para a organização. Os rótulos são aplicados por aplicativos e serviços a dados em repouso ou em movimento, ajudando os usuários e os aplicativos e serviços downstream a entender a confidencialidade das informações que estão tratando.

### <a name="understand-how-to-apply-labels"></a>Entender como aplicar rótulos

Ao fornecer informações sobre o rótulo de confidencialidade existente e desejado, a API REST pode informar de forma inteligente sua aplicação das ações [](/graph/api/resources/informationprotectionaction) que devem ser executadas para aplicar corretamente o rótulo. Isso inclui ações como aplicativo de [metadados](/graph/api/resources/metadataaction) , geração [de marca d'água](/graph/api/resources/addwatermarkaction) , [proteção](/graph/api/resources/protectbytemplateaction) e muito mais.

### <a name="interpret-labels-applied-to-data"></a>Interpretar rótulos aplicados aos dados

Aplicativos que consomem informações [](/graph/api/resources/metadataaction) que já têm metadados de rótulo de confidencialidade aplicados podem usar a API **extractLabel** para resolver metadados de rótulo para um Proteção de Informações do Microsoft Purview [rótulo de confidencialidade](/graph/api/resources/informationprotectionlabel). Use o rótulo para identificar as ações que devem ser executadas pelo aplicativo ao manipular ou consumir os dados rotulados. 

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [Proteção de Informações do Microsoft Purview API no Microsoft Graph beta](/graph/api/resources/informationprotectionlabel)

## <a name="next-steps"></a>Próximas etapas

- Selecione e tente Proteção de Informações consultas de exemplo de rotulagem no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). Escolha **Mostrar mais exemplos** na coluna à esquerda. Use o menu para ativar o **Proteção de Informações do Microsoft Purview**.
