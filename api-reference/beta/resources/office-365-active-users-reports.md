---
title: Relatórios dos usuários ativos do Office 365
description: Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças do produto estão sendo usadas por indivíduos em sua organização e fazer uma busca detalhada para obter informações sobre quais usuários estão usando quais produtos. Este relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e85924b7066dde92f0db5fd0b3f1f83dd32fd0c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516207"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="016ce-104">Relatórios dos usuários ativos do Office 365</span><span class="sxs-lookup"><span data-stu-id="016ce-104">Office 365 active users reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="016ce-105">Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças do produto estão sendo usadas por indivíduos em sua organização e fazer uma busca detalhada para obter informações sobre quais usuários estão usando quais produtos.</span><span class="sxs-lookup"><span data-stu-id="016ce-105">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="016ce-106">Este relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.</span><span class="sxs-lookup"><span data-stu-id="016ce-106">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="016ce-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="016ce-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="016ce-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="016ce-108">Reports</span></span>
| <span data-ttu-id="016ce-109">Função</span><span class="sxs-lookup"><span data-stu-id="016ce-109">Function</span></span>                                 | <span data-ttu-id="016ce-110">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="016ce-110">CSV return type</span></span> | <span data-ttu-id="016ce-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="016ce-111">JSON return type</span></span>                         | <span data-ttu-id="016ce-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="016ce-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="016ce-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="016ce-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="016ce-114">Stream</span><span class="sxs-lookup"><span data-stu-id="016ce-114">Stream</span></span>          | [<span data-ttu-id="016ce-115">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="016ce-115">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="016ce-116">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="016ce-116">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="016ce-117">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="016ce-117">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="016ce-118">Stream</span><span class="sxs-lookup"><span data-stu-id="016ce-118">Stream</span></span>          | [<span data-ttu-id="016ce-119">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="016ce-119">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="016ce-120">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="016ce-120">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="016ce-121">Obter contagens de usuários dos serviços</span><span class="sxs-lookup"><span data-stu-id="016ce-121">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="016ce-122">Fluxo</span><span class="sxs-lookup"><span data-stu-id="016ce-122">Stream</span></span>          | [<span data-ttu-id="016ce-123">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="016ce-123">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="016ce-124">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="016ce-124">Get the count of users by activity type and service.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
