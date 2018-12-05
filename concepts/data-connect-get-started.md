---
title: Introdução ao Microsoft Graph dados conectar (preview)
description: 'Antes de poder usar a conexão de dados do Microsoft Graph, um administrador do Office 365 deve levar duas ações, ambos habilitam a capacidade para o administrador para movimentação de dados de controle por meio de gerenciamento de acesso privilegiado (PAM). '
ms.openlocfilehash: eb21f0d850f64694514c0ecd82f03de687606a56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091565"
---
# <a name="get-started-with-microsoft-graph-data-connect-preview"></a>Introdução ao Microsoft Graph dados conectar (preview)

Antes de poder usar a conexão de dados do Microsoft Graph, um administrador do Office 365 deve levar duas ações, ambos habilitam a capacidade para o administrador para movimentação de dados de controle por meio de gerenciamento de acesso privilegiado (PAM). 

1. Conceder consentimento optarem dados se conectar por meio de Portal de administração do Microsoft 365, na página **serviços e suplementos** do Microsoft Graph. Isso permitirá que as solicitações de movimentação de dados para o Microsoft Azure (isto é, mantenha o controle total sobre os dados, mas permitir recursos Azure para acessá-lo). Nenhum dado será transferido, a menos que a aprovação de um pipeline específico é fornecida posteriormente.
2. Defina um grupo de aprovador dentro de assinatura do Office 365. Certifique-se de que o grupo de aprovador não está vazio. Somente os usuários no grupo podem aprovar solicitações de movimentação de dados.

Para obter instruções detalhadas passo a passo, consulte o [módulo de treinamento de conexão de dados do Microsoft Graph](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).

## <a name="next-steps"></a>Próximas etapas

Parabéns! Agora você está pronto para começar a criar aplicativos inteligentes com ferramentas do Windows Azure. Para obter um exemplo de aplicativo e documentação adicional, consulte os [dados do Microsoft Graph conectar GitHub repo](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki). 
