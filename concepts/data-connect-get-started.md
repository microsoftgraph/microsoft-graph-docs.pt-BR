---
title: Introdução à conexão de dados do Microsoft Graph
description: 'Antes de poder usar a conexão de dados do Microsoft Graph, um administrador do Microsoft 365 deve realizar duas ações que habilitam a capacidade do administrador de controlar a movimentação de dados de controle por meio de PAM (Privileged Access Management). '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: f451da704c0fce255f37b61da7c7446145d8afd1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897278"
---
# <a name="get-started-with-microsoft-graph-data-connect"></a>Introdução à conexão de dados do Microsoft Graph

Antes de poder usar a conexão de dados do Microsoft Graph, um administrador do Microsoft 365 deve realizar duas ações que habilitam a capacidade do administrador de controlar a movimentação de dados de controle por meio de PAM (Privileged Access Management). 

1. Dê consentimento à aceitação da conexão de dados do Microsoft Graph por meio do Portal de Administração Microsoft 365, na página **Serviços e suplementos**. Isso permitirá solicitações de movimentação de dados no Microsoft Azure (ou seja, manter o controle total sobre os dados, mas permitir que os recursos do Azure os acessem). Nenhum dado é transferido, a menos que a aprovação de um pipeline específico seja fornecida mais tarde.
2. Configure um grupo de segurança habilitado para email ou uma lista de distribuição na assinatura do Microsoft 365. Verifique se o grupo aprovador não está vazio. Somente os usuários no grupo podem aprovar solicitações de movimentação de dados.

## <a name="next-steps"></a>Próximas etapas

Parabéns! Agora você está pronto para começar a criar aplicativos inteligentes com as ferramentas do Azure. Para obter passo a passo das instruções, veja o [módulo de treinamento do Microsoft Graph Data Connect](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md). Para obter mais informações sobre os recursos que o Microsoft Graph Data Connect oferece, confira [conjuntos de dados, regiões e coletores](data-connect-datasets.md) ou [seleção de usuário e filtragem](data-connect-filtering.md) que o Data Connect suporta.
