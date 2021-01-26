---
title: Relatórios de usuários ativos do Microsoft 365
description: Você pode usar os relatórios de usuários ativos do Microsoft 365 para descobrir quantas licenças de produto estão sendo usadas por indivíduos em sua organização e fazer buscas drill down para obter informações sobre quais usuários estão usando quais produtos. Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: e795b58eaae7ecd428f1473b277cd6bc65cbf09d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981022"
---
# <a name="microsoft-365-active-users-reports"></a><span data-ttu-id="bb690-104">Relatórios de usuários ativos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="bb690-104">Microsoft 365 active users reports</span></span>

<span data-ttu-id="bb690-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb690-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bb690-106">Você pode usar os relatórios de usuários ativos do Microsoft 365 para descobrir quantas licenças de produto estão sendo usadas por indivíduos em sua organização e fazer buscas drill down para obter informações sobre quais usuários estão usando quais produtos.</span><span class="sxs-lookup"><span data-stu-id="bb690-106">You can use the Microsoft 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="bb690-107">Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="bb690-107">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="bb690-108">**Observação:** Para saber mais sobre os diferentes modos de exibição de relatório e nomes, confira [Relatórios do Microsoft 365 - Usuários Ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d). </span><span class="sxs-lookup"><span data-stu-id="bb690-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="bb690-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="bb690-109">Reports</span></span>
| <span data-ttu-id="bb690-110">Função</span><span class="sxs-lookup"><span data-stu-id="bb690-110">Function</span></span>                                 | <span data-ttu-id="bb690-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bb690-111">Return Type</span></span> | <span data-ttu-id="bb690-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb690-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="bb690-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="bb690-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="bb690-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="bb690-114">Stream</span></span>      | <span data-ttu-id="bb690-115">Obter detalhes sobre usuários ativos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bb690-115">Get details about Microsoft 365 active users.</span></span> |
| [<span data-ttu-id="bb690-116">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="bb690-116">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="bb690-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="bb690-117">Stream</span></span>      | <span data-ttu-id="bb690-118">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="bb690-118">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="bb690-119">Obter contagens de usuários dos serviços</span><span class="sxs-lookup"><span data-stu-id="bb690-119">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="bb690-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="bb690-120">Stream</span></span>      | <span data-ttu-id="bb690-121">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="bb690-121">Get the count of users by activity type and service.</span></span> |

