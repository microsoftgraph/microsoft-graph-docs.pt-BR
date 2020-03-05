---
title: Relatórios dos usuários ativos do Office 365
description: Você pode usar os relatórios dos usuários ativos do Office 365 para descobrir quantas licenças de produtos estão sendo usadas por indivíduos em sua organização e detalhar informações sobre quais usuários estão usando quais produtos. Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 163eab83bfcb5089ec21d449d90840384c12e4ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447343"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="ce967-104">Relatórios dos usuários ativos do Office 365</span><span class="sxs-lookup"><span data-stu-id="ce967-104">Office 365 active users reports</span></span>

<span data-ttu-id="ce967-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ce967-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce967-106">Você pode usar os relatórios dos usuários ativos do Office 365 para descobrir quantas licenças de produtos estão sendo usadas por indivíduos em sua organização e detalhar informações sobre quais usuários estão usando quais produtos.</span><span class="sxs-lookup"><span data-stu-id="ce967-106">You can use the Office 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="ce967-107">Esses relatórios podem ajudar os administradores a identificar produtos ou usuários subutilizados que possam precisar de treinamento ou informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ce967-107">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="ce967-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="ce967-108">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="ce967-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="ce967-109">Reports</span></span>
| <span data-ttu-id="ce967-110">Função</span><span class="sxs-lookup"><span data-stu-id="ce967-110">Function</span></span>                                 | <span data-ttu-id="ce967-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ce967-111">Return Type</span></span> | <span data-ttu-id="ce967-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce967-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="ce967-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="ce967-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="ce967-114">Stream</span><span class="sxs-lookup"><span data-stu-id="ce967-114">Stream</span></span>      | <span data-ttu-id="ce967-115">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="ce967-115">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="ce967-116">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="ce967-116">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="ce967-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ce967-117">Stream</span></span>      | <span data-ttu-id="ce967-118">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="ce967-118">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="ce967-119">Obter contagens de usuários dos serviços</span><span class="sxs-lookup"><span data-stu-id="ce967-119">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="ce967-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="ce967-120">Stream</span></span>      | <span data-ttu-id="ce967-121">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="ce967-121">Get the count of users by activity type and service.</span></span> |
