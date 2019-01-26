---
title: Relatórios dos usuários ativos do Office 365
description: Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças do produto estão sendo usadas por indivíduos em sua organização e fazer uma busca detalhada para obter informações sobre quais usuários estão usando quais produtos. Este relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 638550fbc44acd0154a2dab5c062e2061fa9c582
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571762"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="9bc23-104">Relatórios dos usuários ativos do Office 365</span><span class="sxs-lookup"><span data-stu-id="9bc23-104">Office 365 active users reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bc23-105">Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças do produto estão sendo usadas por indivíduos em sua organização e fazer uma busca detalhada para obter informações sobre quais usuários estão usando quais produtos.</span><span class="sxs-lookup"><span data-stu-id="9bc23-105">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="9bc23-106">Este relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.</span><span class="sxs-lookup"><span data-stu-id="9bc23-106">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="9bc23-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="9bc23-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="9bc23-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="9bc23-108">Reports</span></span>
| <span data-ttu-id="9bc23-109">Função</span><span class="sxs-lookup"><span data-stu-id="9bc23-109">Function</span></span>                                 | <span data-ttu-id="9bc23-110">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="9bc23-110">CSV return type</span></span> | <span data-ttu-id="9bc23-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="9bc23-111">JSON return type</span></span>                         | <span data-ttu-id="9bc23-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bc23-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="9bc23-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="9bc23-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="9bc23-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="9bc23-114">Stream</span></span>          | [<span data-ttu-id="9bc23-115">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="9bc23-115">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="9bc23-116">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9bc23-116">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="9bc23-117">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="9bc23-117">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="9bc23-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="9bc23-118">Stream</span></span>          | [<span data-ttu-id="9bc23-119">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="9bc23-119">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="9bc23-120">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="9bc23-120">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="9bc23-121">Obter contagens de usuários dos serviços</span><span class="sxs-lookup"><span data-stu-id="9bc23-121">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="9bc23-122">Fluxo</span><span class="sxs-lookup"><span data-stu-id="9bc23-122">Stream</span></span>          | [<span data-ttu-id="9bc23-123">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="9bc23-123">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="9bc23-124">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="9bc23-124">Get the count of users by activity type and service.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
