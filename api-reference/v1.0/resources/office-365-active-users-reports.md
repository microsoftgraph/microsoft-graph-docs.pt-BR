---
title: Relatórios de usuários ativos do Microsoft 365
description: Você pode usar os relatórios do Microsoft 365 active Users para saber quantas licenças de produto estão sendo usadas por indivíduos em sua organização e detalhar as informações sobre quais usuários estão usando quais produtos. Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 041bbe180df2225383d704002d06359334fb8d84
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898160"
---
# <a name="microsoft-365-active-users-reports"></a><span data-ttu-id="f6bcb-104">Relatórios de usuários ativos do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f6bcb-104">Microsoft 365 active users reports</span></span>

<span data-ttu-id="f6bcb-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6bcb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6bcb-106">Você pode usar os relatórios do Microsoft 365 active Users para saber quantas licenças de produto estão sendo usadas por indivíduos em sua organização e detalhar as informações sobre quais usuários estão usando quais produtos.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-106">You can use the Microsoft 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="f6bcb-107">Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-107">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="f6bcb-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="f6bcb-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="f6bcb-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="f6bcb-109">Reports</span></span>
| <span data-ttu-id="f6bcb-110">Função</span><span class="sxs-lookup"><span data-stu-id="f6bcb-110">Function</span></span>                                 | <span data-ttu-id="f6bcb-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f6bcb-111">Return Type</span></span> | <span data-ttu-id="f6bcb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6bcb-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="f6bcb-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="f6bcb-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="f6bcb-114">Stream</span><span class="sxs-lookup"><span data-stu-id="f6bcb-114">Stream</span></span>      | <span data-ttu-id="f6bcb-115">Obtenha detalhes sobre usuários ativos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-115">Get details about Microsoft 365 active users.</span></span> |
| [<span data-ttu-id="f6bcb-116">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="f6bcb-116">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="f6bcb-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="f6bcb-117">Stream</span></span>      | <span data-ttu-id="f6bcb-118">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-118">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="f6bcb-119">Obter contagens de usuários dos serviços</span><span class="sxs-lookup"><span data-stu-id="f6bcb-119">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="f6bcb-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="f6bcb-120">Stream</span></span>      | <span data-ttu-id="f6bcb-121">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-121">Get the count of users by activity type and service.</span></span> |
