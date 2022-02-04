---
title: Proteção de Informações da Microsoft visão geral de rotulagem
description: 'Proteção de Informações da Microsoft rotulagem ajuda as organizações a classificar, rotular e proteger dados com base Office 365 Rótulos de Sensibilidade do Centro de Conformidade e Segurança.'
author: tommoser
ms.localizationpriority: medium
ms.prod: security
---

# <a name="information-protection-overview"></a>Visão geral da Proteção de Informações

Proteção de Informações da Microsoft ajuda as organizações a classificar, rotular e proteger dados com base [na sensibilidade](/Office365/SecurityCompliance/sensitivity-labels). 

As organizações usam rótulos para ajudar:

* Os usuários no entendimento da importância das informações que estão sendo manipuladas.
* Administradores de conformidade ao descobrir onde residem informações confidenciais. 
* Administradores de segurança na implantação de políticas de prevenção contra perda de dados e acesso a dados com base em informações de rótulo mais ricas.

## <a name="why-integrate-microsoft-information-protection"></a>Por que integrar Proteção de Informações da Microsoft? 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a>Integrar-se à plataforma de rotulagem onipresente, atendendo milhões de usuários e dispositivos

Mais de um milhão de organizações com dezenas de milhões de usuários usam Proteção de Informações da Microsoft para classificar, rotular e proteger dados.  Além do Microsoft 365, vários serviços de prevenção contra perda de dados (DLP), plataformas de business intelligence e soluções de software como serviço (SaaS) adotaram uma rotulagem [Proteção de Informações da Microsoft](https://www.microsoft.com/security/technology/information-protection) para fornecer uma experiência de classificação de dados mais rica. 

### <a name="label-information-in-line-of-business-applications"></a>Informações de rótulo em aplicativos de linha de negócios

Enterprise os desenvolvedores usam Proteção de Informações da Microsoft para rotular e proteger informações confidenciais do cliente sobre a exportação de aplicativos de linha de negócios para garantir a segurança das informações do cliente. Conectar seus aplicativos ao ecossistema Proteção de Informações da Microsoft permite que os aplicativos apliquem, atualizem [e excluam](/Office365/SecurityCompliance/sensitivity-labels) rótulos de sensibilidade em seus próprios dados de aplicativo, sem a sobrecarga de integrar um SDK completo.

## <a name="what-can-i-do-with-microsoft-information-protection-label-apis-in-microsoft-graph"></a>O que posso fazer com Proteção de Informações da Microsoft de rótulos no Microsoft Graph? 

### <a name="discover-labels-available-to-a-user-or-organization"></a>Descobrir rótulos disponíveis para um usuário ou organização

Com o microsoft Graph você pode [acessar os](/graph/api/resources/informationprotectionlabel) rótulos de sensibilidade disponíveis para um usuário ou para a organização. Os rótulos são aplicados por aplicativos e serviços aos dados em repouso ou em movimento, ajudando os usuários e aplicativos e serviços downstream a entender a sensibilidade das informações que estão manipulando.

### <a name="understand-how-to-apply-labels"></a>Entender como aplicar rótulos

Fornecendo informações sobre o rótulo de sensibilidade existente e desejado, a API REST pode informar inteligentemente sua aplicação das ações que devem [](/graph/api/resources/informationprotectionaction) ser tomadas para aplicar corretamente o rótulo. Isso inclui ações como aplicativo de [metadados](/graph/api/resources/metadataaction) , geração [de marcas](/graph/api/resources/addwatermarkaction) d'água, [proteção](/graph/api/resources/protectbytemplateaction) e muito mais.

### <a name="interpret-labels-applied-to-data"></a>Interpretar rótulos aplicados aos dados

Aplicativos que consomem informações que já têm [metadados](/graph/api/resources/metadataaction) de rótulo de sensibilidade aplicados podem usar a API **extractLabel** para resolver metadados de rótulo para um rótulo Proteção de Informações da Microsoft [de sensibilidade.](/graph/api/resources/informationprotectionlabel) Use o rótulo para identificar as ações que devem ser tomadas pelo aplicativo ao manipular ou consumir os dados rotulados. 

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [Proteção de Informações da Microsoft API no Microsoft Graph beta](/graph/api/resources/informationprotectionlabel)

## <a name="next-steps"></a>Próximas etapas

- Selecione e experimente consultas de exemplo de rotulagem da Proteção de Informações [no Graph Explorer](https://developer.microsoft.com/graph/graph-explorer). Escolha **Mostrar mais exemplos** na coluna à esquerda. Use o menu **para ativar Proteção de Informações da Microsoft**.
