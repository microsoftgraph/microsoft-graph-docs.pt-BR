---
title: Visão geral da API do Business central
description: Visão geral do motivo pelo qual você deseja integrar suas soluções com as APIs do Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: b5bdb6974bc03653a95a36928b216045fa3d7b78
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289208"
---
# <a name="dynamics-365-business-central-api-overview-preview"></a>Visão geral da API do Dynamics 365 Business central (versão prévia)
O Dynamics 365 Business central é uma solução de gerenciamento de negócios unificada e fácil de usar e adaptar, ajudando você a se conectar à sua empresa e tomar decisões mais inteligentes. Ele fornece uma visão completa de sua empresa, permitindo que você gerencie suas finanças, automatize e proteja sua cadeia de fornecimento, venda mais inteligente e aprimore o atendimento ao cliente, mantenha projetos no prazo e sob o orçamento e otimize as operações.

> [!VIDEO https://www.youtube-nocookie.com/embed/na1kFk53cbk]

## <a name="why-integrate-with-dynamics-365-business-central"></a>Por que integrar com o Dynamics 365 Business central?
Integrando seus aplicativos ao Dynamics 365 Business central, você pode criar experiências que abranjam suas necessidades de negócios. Você pode criar soluções que permitem que os usuários realizem as principais tarefas e funções de negócios. Você pode usar o Microsoft Graph para acessar e gerenciar seus finanças, trabalhar com contatos comerciais, criar e enviar documentos de vendas e compras e obter informações sobre relatórios financeiros.

### <a name="synchronize-your-business-applications"></a>Sincronizar seus aplicativos de negócios
Muitas empresas usam diferentes aplicativos de negócios desconectados para gerenciar várias funções da empresa. O Microsoft Graph permite que você conecte os dados para trazer esses aplicativos juntos. Isso facilita a conexão do aplicativo de folha de pagamento aos registros de funcionários, a conexão de seus aplicativos de despesas aos registros de fornecedores e o seu aplicativo de CRM manter os registros do cliente atualizados. Conecte seus dados para manter seus aplicativos sincronizados.

### <a name="create-custom-apps-to-manage-your-business-processes"></a>Criar aplicativos personalizados para gerenciar seus processos de negócios
Cada empresa é diferente e pode ter processos de negócios especializados. Esses processos podem ser simplificados com aplicativos personalizados sob medida para o processo. O Microsoft Graph facilita a integração desses aplicativos com seus dados financeiros. A criação de um aplicativo de serviço de vendas ou de campo que cria documentos de vendas, um aplicativo de despesas que cria documentos de compra ou um aplicativo de folha de pagamento que cria diários-razão de contabilidade torna-se possível, mantendo todos os documentos em seu sistema financeiro.

### <a name="gain-insights-from-your-financial-data"></a>Obter informações sobre seus dados financeiros
O Microsoft Graph fornece acesso aos seus relatórios financeiros. Conecte as ferramentas e os aplicativos de BI à sua folha de saldo, declaração de fluxo de caixa, relatórios de envelhecimento de contas a pagar e contas a receber e relatórios de balancete para criar painéis de BI e garantir que os usuários tenham acesso às informações de que precisam.

## <a name="authorization"></a>Autorização
Use o ponto de extremidade do Azure AD v 2.0 para autenticar as APIs do Dynamics 365 Business central. Todas as APIs exigem o `Authorization: Bearer {access-token}` cabeçalho da solicitação. Para obter mais informações sobre autorização, consulte [obter tokens de acesso para chamar o Microsoft Graph](./auth/index.yml).

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

Confira [API do Dynamics 365 Business central no Microsoft Graph beta](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta).


## <a name="next-steps"></a>Próximas etapas
Saiba mais sobre a [API central de negócios e os casos de uso](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta) com suporte no Microsoft Graph.