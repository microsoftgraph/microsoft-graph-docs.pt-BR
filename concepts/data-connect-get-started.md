---
title: Introdução ao Microsoft Graph Data Connect
description: 'Antes de poder usar a conexão de dados do Microsoft Graph, um administrador do Microsoft 365 deve realizar duas ações que habilitam a capacidade do administrador de controlar a movimentação de dados de controle por meio de PAM (Privileged Access Management). '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 312dac9554df89957963364e3ba55eb2899e7702
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013559"
---
# <a name="get-started-with-microsoft-graph-data-connect"></a>Introdução ao Microsoft Graph Data Connect

Antes de poder usar a conexão de dados do Microsoft Graph, um administrador do Microsoft 365 deve realizar duas ações que habilitam a capacidade do administrador de controlar a movimentação de dados de controle por meio de PAM (Privileged Access Management). 

1. Dê consentimento à aceitação da conexão de dados do Microsoft Graph por meio do Portal de Administração do Microsoft 365, na página **Configurações da organização** dentro do **Centro de administração do Microsoft 365**. Isso permitirá solicitações de movimentação de dados no Microsoft Azure (ou seja, manter o controle total sobre os dados, mas permitir que os recursos do Azure os acessem). Nenhum dado é transferido, a menos que aprovação de um pipeline específico seja fornecida mais tarde.
2. Configure um grupo de segurança habilitado para email ou uma lista de distribuição na assinatura do Microsoft 365. Verifique se o grupo aprovador não está vazio. Somente os usuários no grupo podem aprovar solicitações de movimentação de dados.

## <a name="next-steps"></a>Próximas etapas

Parabéns! Agora você está pronto para começar a criar aplicativos inteligentes com as ferramentas do Azure. Para obter passo a passo das instruções, veja o [módulo de treinamento do Microsoft Graph Data Connect](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md). Para obter mais informações sobre os recursos que o Microsoft Graph Data Connect oferece, confira [conjuntos de dados, regiões e coletores](data-connect-datasets.md) ou [seleção de usuário e filtragem](data-connect-filtering.md) que o Data Connect suporta.
