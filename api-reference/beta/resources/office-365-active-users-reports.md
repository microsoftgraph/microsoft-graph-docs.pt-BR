---
title: Relatórios de usuários ativos do Microsoft 365
description: Você pode usar o relatório do Microsoft 365 active Users para saber quantas licenças de produto estão sendo usadas por indivíduos em sua organização e detalhar as informações sobre quais usuários estão usando quais produtos. Esse relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 3d795c3308b7c1494bbff2a24545ba4ca8053583
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021242"
---
# <a name="microsoft-365-active-users-reports"></a><span data-ttu-id="6e5dc-104">Relatórios de usuários ativos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6e5dc-104">Microsoft 365 active users reports</span></span>

<span data-ttu-id="6e5dc-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e5dc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e5dc-106">Você pode usar o relatório do Microsoft 365 active Users para saber quantas licenças de produto estão sendo usadas por indivíduos em sua organização e detalhar as informações sobre quais usuários estão usando quais produtos.</span><span class="sxs-lookup"><span data-stu-id="6e5dc-106">You can use the Microsoft 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="6e5dc-107">Esse relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.</span><span class="sxs-lookup"><span data-stu-id="6e5dc-107">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="6e5dc-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="6e5dc-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="6e5dc-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="6e5dc-109">Reports</span></span>
| <span data-ttu-id="6e5dc-110">Função</span><span class="sxs-lookup"><span data-stu-id="6e5dc-110">Function</span></span>                                 | <span data-ttu-id="6e5dc-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="6e5dc-111">CSV return type</span></span> | <span data-ttu-id="6e5dc-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="6e5dc-112">JSON return type</span></span>                         | <span data-ttu-id="6e5dc-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e5dc-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="6e5dc-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="6e5dc-114">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="6e5dc-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="6e5dc-115">Stream</span></span>          | [<span data-ttu-id="6e5dc-116">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="6e5dc-116">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="6e5dc-117">Obtenha detalhes sobre usuários ativos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6e5dc-117">Get details about Microsoft 365 active users.</span></span> |
| [<span data-ttu-id="6e5dc-118">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="6e5dc-118">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="6e5dc-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="6e5dc-119">Stream</span></span>          | [<span data-ttu-id="6e5dc-120">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="6e5dc-120">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="6e5dc-121">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="6e5dc-121">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="6e5dc-122">Obter contagens de usuários dos serviços</span><span class="sxs-lookup"><span data-stu-id="6e5dc-122">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="6e5dc-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="6e5dc-123">Stream</span></span>          | [<span data-ttu-id="6e5dc-124">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="6e5dc-124">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="6e5dc-125">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="6e5dc-125">Get the count of users by activity type and service.</span></span> |


