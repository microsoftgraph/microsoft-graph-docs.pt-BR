---
title: Políticas e cobrança da Conexão de Dados do Microsoft Graph
description: Saiba mais sobre as políticas do Azure com suporte para um aplicativo criado com dados do Microsoft 365 e a fatura associada ao Azure Data Factory que você está usando.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: cf3942063936f2b26811251290c9c4a135dfd43e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093980"
---
# <a name="microsoft-graph-data-connect-policies-and-billing"></a>Políticas e cobrança da Conexão de Dados do Microsoft Graph

A Conexão de Dados do Microsoft Graph utiliza [aplicativos gerenciados do Azure](/azure/managed-applications/overview) para que você possa criar e implantar soluções em seu ambiente do cliente do Azure. Os aplicativos gerenciados permitem que você suporte certas políticas do Azure, dando aos clientes maior confiança e conforto ao usar seus aplicativos.

## <a name="policies"></a>Políticas

As seguintes políticas do Azure são suportadas para um aplicativo gerenciado do Azure criado usando dados do Microsoft 365:

- [Definições internas da Política do Azure para o Armazenamento do Azure ](/azure/storage/common/policy-reference)
- [Introdução ao Azure Data Lake Storage Gen2](/azure/storage/blobs/data-lake-storage-introduction)
- [Definições internas da Política do Azure para o Azure Data Lake Storage Gen1](/azure/data-lake-store/policy-reference)

> [!NOTE]
> O Azure Data Lake Storage Gen1 e Gen2 utilizam políticas diferentes porque o Azure Data Lake Storage Gen2 implementa o Armazenamento do Azure.

Quando você seleciona qualquer uma das políticas durante a publicação do Azure Marketplace, o status de conformidade da política é verificado e aplicado a todas as instalações do seu aplicativo. Todas as políticas selecionadas que estão em conformidade são mostradas aos aprovadores de dados como parte da solicitação dos dados. Qualquer violação de conformidade da política faz com que a execução do pipeline falhe e interrompa a extração de dados.

## <a name="billing"></a>Cobrança

Uma conta está associada à assinatura do Azure do Azure Data Factory que você está utilizando. O preço neste novo modelo de cobrança é baseado no número de objetos do Microsoft Graph que você está acessando. Para obter mais informações sobre faturamento, consulte a [página Preços](https://azure.microsoft.com/pricing/details/graph-data-connect/).

Os objetos de diretório que não são cobrados são os seguintes:

- BasicDataSet_v0.User
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport

## <a name="see-also"></a>Confira também

- [Seleção de usuário e filtragem](data-connect-filtering.md)
- [Perguntas frequentes sobre a Conexão de Dados](data-connect-faq.md)
