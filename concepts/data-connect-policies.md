---
title: Políticas e licença da Conexão de Dados do Microsoft Graph
description: Descreve quais políticas são compatíveis e como atribuir acesso ISV a SKUs para organizações.
author: fercobo-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: b550976f6fde1af5335fb328a9aaef8f48dea33d
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629326"
---
# <a name="microsoft-graph-data-connect-policies-and-billing"></a><span data-ttu-id="7cd14-103">Políticas e cobrança da Conexão de Dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7cd14-103">Microsoft Graph Data Connect policies and billing</span></span>

<span data-ttu-id="7cd14-104">A Conexão de Dados do Microsoft Graph utiliza [aplicativos gerenciados do Azure](/azure/managed-applications/overview) para que você possa criar e implantar soluções em seu ambiente do cliente do Azure.</span><span class="sxs-lookup"><span data-stu-id="7cd14-104">Microsoft Graph Data Connect uses [Azure managed applications](/azure/managed-applications/overview) to allow you to create and deploy your solutions in your Azure environment.</span></span> <span data-ttu-id="7cd14-105">Aplicativos gerenciados permitem a você dar suporte a determinadas políticas do Azure, fornecendo aos clientes maior confiança e conforto ao usar seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7cd14-105">Managed applications allow you to support certain Azure policies, giving customers greater confidence and comfortability when using your applications.</span></span>

## <a name="policies"></a><span data-ttu-id="7cd14-106">Políticas</span><span class="sxs-lookup"><span data-stu-id="7cd14-106">Policies</span></span>

<span data-ttu-id="7cd14-107">As seguintes políticas do Azure são compatíveis com um desenvolvedor de aplicativo gerenciando do Azure usando dados do Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="7cd14-107">The following Azure policies are supported for an Azure managed application built using Microsoft 365 data:</span></span>

- [<span data-ttu-id="7cd14-108">Armazenamento do Azure e política necessária do ADLS Gen 2</span><span class="sxs-lookup"><span data-stu-id="7cd14-108">Azure Storage and ADLS Gen 2 required policy</span></span>](/azure/storage/common/policy-reference)
- [<span data-ttu-id="7cd14-109">Política necessária do ADLS Gen1</span><span class="sxs-lookup"><span data-stu-id="7cd14-109">ADLS Gen1 required policy</span></span>](/azure/data-lake-store/policy-reference)

> [!NOTE]
> <span data-ttu-id="7cd14-110">O Azure Data Lake Store Gen 1 e Gen 2 usam políticas diferentes porque o ADLS Gen 2 implementa o Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="7cd14-110">Azure Data Lake Store Gen 1 and Gen 2 use different policies because ADLS Gen 2 implements Azure Storage.</span></span>

<span data-ttu-id="7cd14-111">Ao selecionar qualquer uma das políticas durante a publicação do Azure Marketplace, o status de conformidade da política será marcado e aplicado a todas as instalações do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7cd14-111">When you select any of the policies during Azure marketplace publishing, the policy compliance status will be checked and enforced for all installations of your application.</span></span> <span data-ttu-id="7cd14-112">Todas as políticas selecionadas compatíveis serão exibidas para os aprovadores de dados como parte da solicitação de dados.</span><span class="sxs-lookup"><span data-stu-id="7cd14-112">All selected policies that are compliant will be shown to the data approvers as part of the data request.</span></span> <span data-ttu-id="7cd14-113">Qualquer violação de conformidade da política causaria falha no pipeline e interrupção da extração de dados.</span><span class="sxs-lookup"><span data-stu-id="7cd14-113">Any policy compliance violation would cause the pipeline run to fail and stop the data extraction.</span></span>

## <a name="billing-for-microsoft-graph-data-connect"></a><span data-ttu-id="7cd14-114">Cobrança da Conexão de Dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7cd14-114">Billing for Microsoft Graph Data Connect</span></span>

<span data-ttu-id="7cd14-115">A fatura será associada à Assinatura do Azure, do Azure Data Factory que você estiver utilizando.</span><span class="sxs-lookup"><span data-stu-id="7cd14-115">The bill will be associated with the Azure Subscription of the Azure Data Factory you are using.</span></span> <span data-ttu-id="7cd14-116">O preço neste novo modelo de faturamento é baseado no número de objetos do Microsoft Graph que você está acessando.</span><span class="sxs-lookup"><span data-stu-id="7cd14-116">The price in this new billing model is based on the number of Microsoft Graph objects you are accessing.</span></span>

<span data-ttu-id="7cd14-117">Enquanto esse novo recurso de faturamento está versão prévia, a taxa é de US$ 0,375 para 1.000 objetos Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7cd14-117">While this new billing capability is in preview, the rate is $0.375 for 1,000 Microsoft Graph objects.</span></span> <span data-ttu-id="7cd14-118">Por exemplo, se você acessar o total de 10.000 objetos, você receberá uma conta do Azure por US$ 3,75.</span><span class="sxs-lookup"><span data-stu-id="7cd14-118">For example, if you access 10,000 total objects, you will receive an Azure bill for $3.75.</span></span> <span data-ttu-id="7cd14-119">Ao final do período de versão prévia, a taxa será de US$ 0,75 por 1.000 objetos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7cd14-119">At the end of the preview period, the rate will be $0.75 per 1,000 Microsoft Graph objects.</span></span>

<span data-ttu-id="7cd14-120">Os objetos de diretório que não serão cobrados são:</span><span class="sxs-lookup"><span data-stu-id="7cd14-120">Directory objects that will not be charged are:</span></span>

- <span data-ttu-id="7cd14-121">BasicDataSet_v0.User</span><span class="sxs-lookup"><span data-stu-id="7cd14-121">BasicDataSet_v0.User</span></span>
- <span data-ttu-id="7cd14-122">BasicDataSet_v0.MailboxSettings</span><span class="sxs-lookup"><span data-stu-id="7cd14-122">BasicDataSet_v0.MailboxSettings</span></span>
- <span data-ttu-id="7cd14-123">BasicDataSet_v0.Manager</span><span class="sxs-lookup"><span data-stu-id="7cd14-123">BasicDataSet_v0.Manager</span></span>
- <span data-ttu-id="7cd14-124">BasicDataSet_v0.DirectReport</span><span class="sxs-lookup"><span data-stu-id="7cd14-124">BasicDataSet_v0.DirectReport</span></span>

## <a name="see-also"></a><span data-ttu-id="7cd14-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="7cd14-125">See also</span></span>

- [<span data-ttu-id="7cd14-126">Políticas de Armazenamento do Azure</span><span class="sxs-lookup"><span data-stu-id="7cd14-126">Azure Storage policies</span></span>](/azure/storage/common/policy-reference)
- [<span data-ttu-id="7cd14-127">Cobrança da Conexão de Dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7cd14-127">Microsoft Graph Data Connect billing</span></span>](https://azure.microsoft.com/pricing/details/graph-data-connect/)
- [<span data-ttu-id="7cd14-128">Aplicativos gerenciados pelo Azure</span><span class="sxs-lookup"><span data-stu-id="7cd14-128">Azure managed applications</span></span>](/azure/managed-applications/overview)
- [<span data-ttu-id="7cd14-129">Seleção de usuário e filtragem</span><span class="sxs-lookup"><span data-stu-id="7cd14-129">User selection and filtering</span></span>](data-connect-filtering.md)
- [<span data-ttu-id="7cd14-130">Perguntas frequentes sobre a Conexão de Dados</span><span class="sxs-lookup"><span data-stu-id="7cd14-130">Data Connect frequently asked questions</span></span>](data-connect-faq.md)
