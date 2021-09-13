---
title: Visão geral da API Central de Negócios
description: Visão geral do motivo pelo qual você deseja integrar suas soluções às APIs da Central de Negócios.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a4b932b2cbc25f967bd0e881c56f1acc0c9382d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137403"
---
# <a name="dynamics-365-business-central-api-overview-preview"></a>Visão geral da API Central de Negócios do Dynamics 365 (visualização)
O Dynamics 365 Business Central é uma solução de gerenciamento de negócios completa e fácil de usar e se adaptar, ajudando você a conectar sua empresa e tomar decisões mais inteligentes. Ele fornece uma visão de ponta a ponta da sua empresa, permitindo que você gerencie suas finanças, automatize e proteja sua cadeia de fornecimento, venda mais inteligente e melhore o atendimento ao cliente, mantenha os projetos dentro do prazo e no orçamento e otimize suas operações.

> [!VIDEO https://www.youtube-nocookie.com/embed/na1kFk53cbk]

## <a name="why-integrate-with-dynamics-365-business-central"></a>Por que se integrar ao Dynamics 365 Business Central?
Ao integrar seus aplicativos com o Dynamics 365 Business Central, você pode criar experiências que abrangem suas necessidades de negócios. Você pode criar soluções que capacitam seus usuários a executar tarefas e funções comerciais importantes. Você pode usar o Microsoft Graph acessar e gerenciar suas finanças, trabalhar com contatos comerciais, criar e enviar vendas e comprar documentos e obter informações de relatórios financeiros.

### <a name="synchronize-your-business-applications"></a>Sincronizar seus aplicativos de negócios
Muitas empresas usam aplicativos comerciais diferentes e desconectados para gerenciar várias funções da empresa. O Microsoft Graph permite que você conecte os dados para reunir esses aplicativos. Isso facilita a conexão do aplicativo de folha de pagamento aos registros de funcionários, conectar seu aplicativo de despesas aos registros do fornecedor e fazer com que seu aplicativo CRM mantenha seus registros de clientes atualizados. Conexão seus dados para manter seus aplicativos em sincronia.

### <a name="create-custom-apps-to-manage-your-business-processes"></a>Criar aplicativos personalizados para gerenciar seus processos comerciais
Cada empresa é diferente e pode ter processos comerciais especializados. Esses processos podem ser simplificados com aplicativos personalizados personalizados para o processo. O microsoft Graph facilita a integração desses aplicativos com seus dados financeiros. A criação de um aplicativo de vendas ou serviço de campo que cria documentos de vendas, um aplicativo de despesas que cria documentos de compra ou um aplicativo de folha de pagamento que cria diários contábeis gerais se torna possível, mantendo todos os documentos em seu sistema financeiro.

### <a name="gain-insights-from-your-financial-data"></a>Obtenha informações de seus dados financeiros
O Microsoft Graph fornece acesso aos relatórios financeiros. Conexão Ferramentas de BI e aplicativos para seu balanço, instrução de fluxo de caixa, relatórios de ativos e créditos a receber e relatórios de balanceamento de avaliação para criar painéis de BI e garantir que os usuários tenham acesso às informações necessárias.

## <a name="authorization"></a>Autorização
Use o ponto de extremidade do Azure AD v2.0 para autenticar as APIs da Central de Negócios do Dynamics 365. Todas as APIs exigem `Authorization: Bearer {access-token}` o header de solicitação. Para obter mais informações sobre autorização, consulte [Obter tokens de acesso para chamar a Microsoft Graph](./auth/index.yml).

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

Consulte a API Central de Negócios do [Dynamics 365 no Microsoft Graph beta](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta).


## <a name="next-steps"></a>Próximas etapas
Saiba mais sobre a API Central de Negócios [e casos de uso](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta) suportados no Microsoft Graph.
