---
title: Políticas e licença do Microsoft Graph Data Connect
description: Descreve quais políticas são compatíveis e como atribuir acesso ISV a SKUs para organizações.
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: c9529c500ff2e086a3a1185a56b9db397f0ace49
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547615"
---
# <a name="microsoft-graph-data-connect-policies-and-licensing"></a>Políticas e licença do Microsoft Graph Data Connect

Microsoft Graph Data Connect utiliza [aplicativos gerenciados do Azure](/azure/managed-applications/overview) para que você possa criar e implantar soluções em seu ambiente do cliente do Azure. Aplicativos gerenciados permitem a você dar suporte a determinadas políticas do Azure, fornecendo aos clientes maior confiança e conforto ao usar seus aplicativos. Além disso, você deve comprar e aplicar licenças da Microsoft, sua organização ou organizações que instalam seus aplicativos, para permitir que o aplicativo acesse os dados através do Data Connect.

## <a name="policies"></a>Políticas

As seguintes políticas do Azure são compatíveis com um desenvolvedor de aplicativo gerenciando do Azure usando dados do Microsoft 365:

- [Política de Criptografia Necessária do ADLS Gen1](/azure/azure-policy/scripts/enforce-datalakestore-encryption)

Ao selecionar qualquer uma das políticas durante a publicação do Azure Marketplace, o status de conformidade da política será marcado e aplicado a todas as instalações do seu aplicativo. Todas as políticas selecionadas compatíveis serão exibidas para os aprovadores de dados como parte da solicitação de dados. Qualquer violação de conformidade da política causaria falha no pipeline e interrupção da extração de dados.

Se você deseja solicitar suporte para políticas adicionais, informe-nos no fórum de idéias da [Plataforma de Desenvolvedor do Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).

## <a name="licensing"></a>Licenças

A conexão de dados do Microsoft Graph está atualmente disponível como parte da licença do Workplace Analytics, que está disponível por usuário, por mês. As organizações com o Workplace Analytics podem estender seus insights a partir de dados do Microsoft 365, concedendo e governando o acesso a seus dados em escala. Para saber mais, incluindo como comprar, visite a  [página de produtos do Workplace Analytics](https://products.office.com/business/workplace-analytics).

A partir de 1 de fevereiro de 2021, a conexão de dados do Microsoft Graph fará a transição para o Azure Billing para todos os clientes. A fatura será associada à Assinatura do Azure, do Azure Data Factory que você estiver utilizando. O preço neste novo modelo de faturamento é baseado no número de objetos do Microsoft Graph que você está acessando.

Enquanto esse novo recurso de faturamento está versão prévia, a taxa é de US$ 0,375 para 1.000 objetos Microsoft Graph. Por exemplo, se você acessar o total de 10.000 objetos, você receberá uma conta do Azure por US$ 3,75. Ao final do período de versão prévia, a taxa será de US$ 0,75 por 1.000 objetos do Microsoft Graph. As taxas observadas acima serão aplicadas a mensagens de troca e objetos do bate-papo do Teams, incluindo: BasicDataSet_v0.Contact, BasicDataSet_v0.Event, BasicDataSet_v0.Message, BasicDataSet_v0.SentItem, BasicDataSet_v0.MailFolder, e BasicDataSet_v0.CalendarView.

Os objetos para diretório de objetos de não serão carregados, incluindo: BasicDataSet_v0.User, BasicDataSet_v0.MailboxSettings, BasicDataSet_v0.Manager, e BasicDataSet_v0.DirectReport.

## <a name="next-steps"></a>Próximas Etapas
Se você deseja solicitar suporte para políticas ou conjuntos de dados adicionais, informe-nos no fórum de idéias da [Plataforma de Desenvolvedor do Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph). Para saber mais sobre Workplace Analytics, inclusive sobre como comprar, visite a [página de produto do Workplace Analytics](https://products.office.com/business/workplace-analytics).