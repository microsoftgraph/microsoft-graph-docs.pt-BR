---
title: Relatórios dos usuários ativos do Office 365
description: Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças de produtos estão sendo usadas por indivíduos em sua organização e detalhar para obter informações sobre quais usuários estão usando quais produtos. Esse relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 5937a855328224a319cdd148da936517b63171c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522502"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="805e2-104">Relatórios dos usuários ativos do Office 365</span><span class="sxs-lookup"><span data-stu-id="805e2-104">Office 365 active users reports</span></span>

<span data-ttu-id="805e2-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="805e2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="805e2-106">Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças de produtos estão sendo usadas por indivíduos em sua organização e detalhar para obter informações sobre quais usuários estão usando quais produtos.</span><span class="sxs-lookup"><span data-stu-id="805e2-106">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="805e2-107">Esse relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.</span><span class="sxs-lookup"><span data-stu-id="805e2-107">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="805e2-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="805e2-108">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="805e2-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="805e2-109">Reports</span></span>
| <span data-ttu-id="805e2-110">Função</span><span class="sxs-lookup"><span data-stu-id="805e2-110">Function</span></span>                                 | <span data-ttu-id="805e2-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="805e2-111">CSV return type</span></span> | <span data-ttu-id="805e2-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="805e2-112">JSON return type</span></span>                         | <span data-ttu-id="805e2-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="805e2-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="805e2-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="805e2-114">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="805e2-115">Stream</span><span class="sxs-lookup"><span data-stu-id="805e2-115">Stream</span></span>          | [<span data-ttu-id="805e2-116">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="805e2-116">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="805e2-117">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="805e2-117">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="805e2-118">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="805e2-118">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="805e2-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="805e2-119">Stream</span></span>          | [<span data-ttu-id="805e2-120">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="805e2-120">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="805e2-121">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="805e2-121">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="805e2-122">Obter contagens de usuários dos serviços</span><span class="sxs-lookup"><span data-stu-id="805e2-122">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="805e2-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="805e2-123">Stream</span></span>          | [<span data-ttu-id="805e2-124">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="805e2-124">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="805e2-125">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="805e2-125">Get the count of users by activity type and service.</span></span> |
