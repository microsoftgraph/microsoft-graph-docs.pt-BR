---
title: Políticas e licença da Conexão de Dados do Microsoft Graph
description: Descreve quais políticas são compatíveis e como atribuir acesso ISV a SKUs para organizações.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: 2d592391222e39b3c6d4f6406205a99d72d32eb1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340675"
---
# <a name="microsoft-graph-data-connect-policies-and-billing"></a>Políticas e cobrança da Conexão de Dados do Microsoft Graph

A Conexão de Dados do Microsoft Graph utiliza [aplicativos gerenciados do Azure](/azure/managed-applications/overview) para que você possa criar e implantar soluções em seu ambiente do cliente do Azure. Aplicativos gerenciados permitem a você dar suporte a determinadas políticas do Azure, fornecendo aos clientes maior confiança e conforto ao usar seus aplicativos.

## <a name="policies"></a>Políticas

As seguintes políticas do Azure são compatíveis com um desenvolvedor de aplicativo gerenciando do Azure usando dados do Microsoft 365:

- [Armazenamento do Azure e política necessária do ADLS Gen 2](/azure/storage/common/policy-reference)
- [Política necessária do ADLS Gen1](/azure/data-lake-store/policy-reference)

> [!NOTE]
> O Azure Data Lake Store Gen 1 e Gen 2 usam políticas diferentes porque o ADLS Gen 2 implementa o Armazenamento do Azure.

Ao selecionar qualquer uma das políticas durante a publicação do Azure Marketplace, o status de conformidade da política será marcado e aplicado a todas as instalações do seu aplicativo. Todas as políticas selecionadas compatíveis serão exibidas para os aprovadores de dados como parte da solicitação de dados. Qualquer violação de conformidade da política causaria falha no pipeline e interrupção da extração de dados.

## <a name="billing-for-microsoft-graph-data-connect"></a>Cobrança da Conexão de Dados do Microsoft Graph

A fatura será associada à Assinatura do Azure, do Azure Data Factory que você estiver utilizando. O preço neste novo modelo de faturamento é baseado no número de objetos do Microsoft Graph que você está acessando. Para obter mais informações sobre faturamento, consulte a [página Preços](https://azure.microsoft.com/pricing/details/graph-data-connect/).

Os objetos de diretório que não serão cobrados são:

- BasicDataSet_v0.User
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport

## <a name="see-also"></a>Confira também

- [Políticas de Armazenamento do Azure](/azure/storage/common/policy-reference)
- [Cobrança da Conexão de Dados do Microsoft Graph](https://azure.microsoft.com/pricing/details/graph-data-connect/)
- [Aplicativos gerenciados pelo Azure](/azure/managed-applications/overview)
- [Seleção de usuário e filtragem](data-connect-filtering.md)
- [Perguntas frequentes sobre a Conexão de Dados](data-connect-faq.md)
