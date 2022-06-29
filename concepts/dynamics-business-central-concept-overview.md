---
title: Visão geral da API do Dynamics 365 Business Central (versão prévia)
description: Use o Dynamics 365 Business Central, uma solução de gerenciamento de negócios tudo em um, para gerenciar finanças, automatizar sua cadeia de fornecedores e manter os projetos abaixo do orçamento.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 393e2e192ccb6b6d4792d567fce60e87a8832b88
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440898"
---
# <a name="dynamics-365-business-central-api-overview-preview"></a>Visão geral da API do Dynamics 365 Business Central (versão prévia)
O Dynamics 365 Business Central é uma solução de gerenciamento de negócios tudo em um que é fácil de usar e adaptar, ajudando você a conectar seus negócios e tomar decisões mais inteligentes. Ele fornece uma visão de ponta a ponta da sua empresa, permitindo que você gerencie suas finanças, automatize e proteja sua cadeia de fornecedores, venda mais inteligente e melhore o atendimento ao cliente, mantenha os projetos no tempo e abaixo do orçamento e otimize suas operações.

> [!VIDEO https://www.youtube-nocookie.com/embed/na1kFk53cbk]

## <a name="why-integrate-with-dynamics-365-business-central"></a>Por que integrar-se ao Dynamics 365 Business Central?
Ao integrar seus aplicativos ao Dynamics 365 Business Central, você pode criar experiências que abrangem suas necessidades de negócios. Você pode criar soluções que capacitam os usuários a executar as principais tarefas e funções de negócios. Você pode usar o Microsoft Graph para acessar e gerenciar suas finanças, trabalhar com contatos comerciais, criar e enviar vendas e documentos de compra e obter insights de relatórios financeiros.

### <a name="synchronize-your-business-applications"></a>Sincronizar seus aplicativos de negócios
Muitas empresas usam aplicativos de negócios diferentes e desconectados para gerenciar várias funções do negócio. O Microsoft Graph permite que você conecte os dados para reunir esses aplicativos. Isso facilita conectar seu aplicativo de folha de pagamento aos registros de funcionários, conectar seu aplicativo de despesas aos registros do fornecedor e fazer com que seu aplicativo CRM mantenha seus registros de cliente atualizados. Conecte seus dados para manter seus aplicativos em sincronia.

### <a name="create-custom-apps-to-manage-your-business-processes"></a>Criar aplicativos personalizados para gerenciar seus processos de negócios
Cada negócio é diferente e pode ter processos de negócios especializados. Esses processos podem ser simplificados com aplicativos personalizados adaptados ao processo. O Microsoft Graph facilita a integração desses aplicativos com seus dados financeiros. A criação de um aplicativo de serviço de vendas ou de campo que cria documentos de vendas, um aplicativo de despesas que cria documentos de compra ou um aplicativo de folha de pagamento que cria diários do razão geral se torna possível, mantendo todos os seus documentos em seu sistema financeiro.

### <a name="gain-insights-from-your-financial-data"></a>Obtenha insights de seus dados financeiros
O Microsoft Graph fornece acesso aos seus relatórios financeiros. Conecte ferramentas e aplicativos de BI ao seu balanço, à declaração de fluxo de caixa, aos pagamentos e a receber relatórios de envelhecimento e a relatórios de saldo de avaliação para criar painéis de BI e garantir que os usuários tenham acesso às informações de que precisam.

## <a name="authorization"></a>Autorização
Use o Azure AD ponto de extremidade v2.0 para autenticar as APIs do Dynamics 365 Business Central. Todas as APIs exigem o `Authorization: Bearer {access-token}` cabeçalho da solicitação. Para obter mais informações sobre autorização, [consulte Obter tokens de acesso para chamar o Microsoft Graph](./auth/index.yml).

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [API do Dynamics 365 Business Central no Microsoft Graph beta](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta&preserve-view=true)
