---
title: Trabalhando com a API Central de Negócios do Dynamics 365 no Microsoft Graph
description: Documentação da API para integração com o Microsoft Graph
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: conceptualPageType
ms.openlocfilehash: b1fdc91d884c4c0869b97f2068d005407158d6a5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473565"
---
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a><span data-ttu-id="c5de5-103">Trabalhando com a API Central de Negócios do Dynamics 365 no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c5de5-103">Working with the Dynamics 365 Business Central API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5de5-104">Você pode usar o Microsoft Graph para conectar e integrar seu serviço Web ou solução SaaS com o Microsoft Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="c5de5-104">You can use Microsoft Graph to connect and integrate your web service or SaaS solution with Microsoft Dynamics 365 Business Central.</span></span> <span data-ttu-id="c5de5-105">Com o Microsoft Graph, você pode criar aplicativos que tenham acesso autorizado e se integrem perfeitamente aos dados do Microsoft Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="c5de5-105">With Microsoft Graph, you can build apps that get authorized access to and integrate seamlessly with Microsoft Dynamics 365 Business Central data.</span></span>

## <a name="authorization"></a><span data-ttu-id="c5de5-106">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5de5-106">Authorization</span></span>
<span data-ttu-id="c5de5-107">Use o ponto de extremidade do Azure AD v2.0 para autenticar as APIs da Central de Negócios do Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c5de5-107">Use the Azure AD v2.0 endpoint to authenticate Dynamics 365 Business Central APIs.</span></span> <span data-ttu-id="c5de5-108">Todas as APIs exigem `Authorization: Bearer {access-token}` o header de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5de5-108">All APIs require the `Authorization: Bearer {access-token}` request header.</span></span> <span data-ttu-id="c5de5-109">Para obter mais informações sobre autorização, consulte [Obter tokens de acesso para chamar o Microsoft Graph](/graph/auth/).</span><span class="sxs-lookup"><span data-stu-id="c5de5-109">For more information about authorization, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span>

## <a name="common-dynamics-365-business-central-scenarios"></a><span data-ttu-id="c5de5-110">Cenários comuns do Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="c5de5-110">Common Dynamics 365 Business Central scenarios</span></span>
<span data-ttu-id="c5de5-111">A API Central de Negócios do Dynamics 365 permite que você leia e modifique dados de negócios por meio de aplicativos conectados e integrados por meio de um único ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="c5de5-111">The Dynamics 365 Business Central API allows you to read and modify business data through apps that are connected and integrated through a single endpoint.</span></span> <span data-ttu-id="c5de5-112">Use a API para, por exemplo, obter acesso às informações do [cliente](../resources/dynamics-customer.md) e [do](../resources/dynamics-vendor.md) fornecedor ou exibir pagamentos [atrasados.](../resources/dynamics-agedaccountspayable.md)</span><span class="sxs-lookup"><span data-stu-id="c5de5-112">Use the API to, for example, get access to [customer](../resources/dynamics-customer.md) and [vendor](../resources/dynamics-vendor.md) information, or [view overdue payments](../resources/dynamics-agedaccountspayable.md).</span></span>

## <a name="whats-new"></a><span data-ttu-id="c5de5-113">Novidades</span><span class="sxs-lookup"><span data-stu-id="c5de5-113">What's new</span></span>
<span data-ttu-id="c5de5-114">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="c5de5-114">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c5de5-115">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="c5de5-115">Next steps</span></span>
<span data-ttu-id="c5de5-116">A API Central de Negócios do Dynamics 365 pode abrir novas maneiras de você se envolver com os usuários.</span><span class="sxs-lookup"><span data-stu-id="c5de5-116">The Dynamics 365 Business Central API can open up new ways for you to engage with users.</span></span> <span data-ttu-id="c5de5-117">Para saber mais, consulte o seguinte:</span><span class="sxs-lookup"><span data-stu-id="c5de5-117">To learn more, see the following:</span></span>

+ [<span data-ttu-id="c5de5-118">Visão geral central do Dynamics 365 Business</span><span class="sxs-lookup"><span data-stu-id="c5de5-118">Dynamics 365 Business Central Overview</span></span>](/graph/dynamics-business-central-concept-overview)
+ <span data-ttu-id="c5de5-119">Experimente [o Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="c5de5-119">Try [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<!--
|For Resource Type |See                                                 |
|:-----------------|:---------------------------------------------------|
|account resource type|[account](../resources/dynamics-account.md)|
|aged accounts receivable resource type|[agedAccountsReceivable](../resources/dynamics-agedaccountsreceivable.md)|
|aged accounts payable resource type|[agedAccountsPayable](../resources/dynamics-agedaccountspayable.md)|
|balance sheet resource type|[balanceSheet](../resources/dynamics-balancesheet.md)|
|companies resource type|[companies](../resources/dynamics-companies.md)|
|companyInformation resource type|[companyInformation](../resources/dynamics-companyinformation.md)|
|countriesRegions resource type|[countriesRegions](../resources/dynamics-countriesregions.md)|
|currencies resource type|[currencies](../resources/dynamics-currencies.md)|
|customer resource type|[customer](../resources/dynamics-customer.md)|
|customerPaymentJournal resource type|[customerPaymentsJournal](../resources/dynamics-customerpaymentsjournal.md)|
|customerPayment resource type|[customerPayment](../resources/dynamics-customerpayment.md)|
|dimension resource type|[dimension](../resources/dynamics-dimension.md)|
|dimensionValue resource type|[dimensionValue](../resources/dynamics-dimensionvalue.md)
|employee resource type|[employee](../resources/dynamics-employee.md)|
|generalLedgerEntries resource type|[generalLedgerEntries](../resources/dynamics-generalledgerentries.md)|
|item resource type|[item](../resources/dynamics-item.md)|
|itemCategories resource type|[itemCategories](../resources/dynamics-itemcategories.md)|
|income statement resource type|[incomeStatement](../resources/dynamics-incomestatement.md)|
|IRS1099 resource type|[irs1099](../resources/dynamics-irs1099.md)|
|journal resource type|[journal](../resources/dynamics-journal.md)|
|journalLine resource type|[journalLine](../resources/dynamics-journalline.md)|
|paymentMethods resource type|[paymentMethods](../resources/dynamics-paymentmethods.md)|
|paymentTerms resource type|[paymentTerms](../resources/dynamics-paymentterms.md)|
|retained earnings statement resource type|[retainedEarningsStatement](../resources/dynamics-retainedearningsstatement.md)|
|shipmentMethods resource type|[shipmentMethods](../resources/dynamics-shipmentmethods.md)|
|taxGroups resource type|[taxGroups](../resources/dynamics-taxgroups.md)|
|taxArea resource type|[taxAreas](..resources/dynamics-taxarea.md)|
|unitsOfMeasure resource type|[unitsOfMeasure](../resources/dynamics-unitsofmeasure.md)|
|vendor resource type|[vendor](../resources/dynamics-vendor.md)|
-->