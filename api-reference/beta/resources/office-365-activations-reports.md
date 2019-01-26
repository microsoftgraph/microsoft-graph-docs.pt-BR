---
title: Relatórios de ativações do Office 365
description: O relatório de ativação do Office 365 oferece um modo de exibição dos quais usuários ativou suas assinaturas do Office 365 em pelo menos um dispositivo. Ele fornece uma divisão do Office 365 ProPlus, Project e Visio Pro para Office 365 ativações de assinatura, bem como a divisão da ativações entre dispositivos e área de trabalho. Este relatório pode ajudá-lo a identificar os usuários que talvez seja necessário suporte adicional para ativar sua assinatura do Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 345ab500ef5986471bb801a88ee5886473a3dd60
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573673"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="9c0b6-105">Relatórios de ativações do Office 365</span><span class="sxs-lookup"><span data-stu-id="9c0b6-105">Office 365 activations reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c0b6-106">O relatório de ativação do Office 365 oferece um modo de exibição dos quais usuários ativou suas assinaturas do Office 365 em pelo menos um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9c0b6-106">The Office 365 activation report gives you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="9c0b6-107">Ele fornece uma divisão do Office 365 ProPlus, Project e Visio Pro para Office 365 ativações de assinatura, bem como a divisão da ativações entre dispositivos e área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9c0b6-107">It provides a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="9c0b6-108">Este relatório pode ajudá-lo a identificar os usuários que talvez seja necessário suporte adicional para ativar sua assinatura do Office.</span><span class="sxs-lookup"><span data-stu-id="9c0b6-108">This report could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="9c0b6-109">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="9c0b6-109">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="9c0b6-110">Relatórios</span><span class="sxs-lookup"><span data-stu-id="9c0b6-110">Reports</span></span>
| <span data-ttu-id="9c0b6-111">Função</span><span class="sxs-lookup"><span data-stu-id="9c0b6-111">Function</span></span>                                 | <span data-ttu-id="9c0b6-112">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="9c0b6-112">CSV return type</span></span> | <span data-ttu-id="9c0b6-113">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="9c0b6-113">JSON return type</span></span>                         | <span data-ttu-id="9c0b6-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c0b6-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="9c0b6-115">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="9c0b6-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="9c0b6-116">Fluxo</span><span class="sxs-lookup"><span data-stu-id="9c0b6-116">Stream</span></span>          | [<span data-ttu-id="9c0b6-117">office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="9c0b6-117">office365ActivationsUserDetail</span></span>](../resources/office365activationsuserdetail.md) | <span data-ttu-id="9c0b6-118">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="9c0b6-118">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="9c0b6-119">Obter contagens de ativação</span><span class="sxs-lookup"><span data-stu-id="9c0b6-119">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="9c0b6-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="9c0b6-120">Stream</span></span>          | [<span data-ttu-id="9c0b6-121">office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="9c0b6-121">office365ActivationCounts</span></span>](../resources/office365activationcounts.md) | <span data-ttu-id="9c0b6-122">Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9c0b6-122">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="9c0b6-123">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="9c0b6-123">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="9c0b6-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="9c0b6-124">Stream</span></span>          | [<span data-ttu-id="9c0b6-125">office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="9c0b6-125">office365ActivationsUserCounts</span></span>](../resources/office365activationsusercounts.md) | <span data-ttu-id="9c0b6-126">Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office no desktop ou nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9c0b6-126">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-activations-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
