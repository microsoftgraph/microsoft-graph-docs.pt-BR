---
title: Introdução ao Microsoft Graph Data Connect (versão prévia)
description: 'Antes de poder usar o Microsoft Graph Data Connect, um administrador do Office 365 deve realizar duas ações que habilitam a capacidade do administrador de controlar a movimentação de dados de controle por meio de PAM (Privileged Access Management). '
author: ajacks-msft
ms.openlocfilehash: 1cd8d5734b0fd8b48df8a49fe0a833583c21148d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312079"
---
# <a name="get-started-with-microsoft-graph-data-connect-preview"></a>Introdução ao Microsoft Graph Data Connect (versão prévia)

Antes de poder usar o Microsoft Graph Data Connect, um administrador do Office 365 deve realizar duas ações que habilitam a capacidade do administrador de controlar a movimentação de dados de controle por meio de PAM (Privileged Access Management). 

1. Dê consentimento à aceitação do Microsoft Graph Data Connect por meio do Portal de Administração do Microsoft 365, na página **Serviços e suplementos**. Isso permitirá solicitações de movimentação de dados no Microsoft Azure (ou seja, manter o controle total sobre os dados, mas permitir que os recursos do Azure os acessem). Nenhum dado é transferido, a menos que aprovação de um pipeline específico seja fornecida mais tarde.
2. Configure um grupo aprovador dentro da assinatura do Office 365. Verifique se o grupo aprovador não está vazio. Somente os usuários no grupo podem aprovar solicitações de movimentação de dados.

Para obter instruções passo a passo, veja o [módulo de treinamento do Microsoft Graph Data Connect](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).

## <a name="next-steps"></a>Próximas etapas

Parabéns! Agora você está pronto para começar a criar aplicativos inteligentes com as ferramentas do Azure. Para documentação adicional e um aplicativo de exemplo, veja o [repositório do GitHub do Microsoft Graph Data Connect](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki). 
