---
title: Relatórios de ativações do Office 365
description: Os relatórios de ativação do Office 365 oferecem uma visão de quais usuários ativaram suas assinaturas do Office 365 em pelo menos um dispositivo. Esses relatórios fornecem dados sobre as ativações de assinaturas do Office 365 ProPlus, do Project e do Visio Pro para Office 365, bem como o detalhamento das ativações entre desktops e dispositivos. Esses relatórios podem ajudar a identificar os usuários que podem precisar de suporte adicional para ativar a assinatura do Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: d01f3116f6a6a12753384ec41c2cee609b9b7f8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534183"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="b679f-105">Relatórios de ativações do Office 365</span><span class="sxs-lookup"><span data-stu-id="b679f-105">Office 365 activations reports</span></span>

<span data-ttu-id="b679f-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b679f-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b679f-107">Os relatórios de ativação do Office 365 oferecem uma visão de quais usuários ativaram suas assinaturas do Office 365 em pelo menos um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b679f-107">The Office 365 activation reports can give you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="b679f-108">Esses relatórios fornecem dados sobre as ativações de assinaturas do Office 365 ProPlus, do Project e do Visio Pro para Office 365, bem como o detalhamento das ativações entre desktops e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b679f-108">These reports provide a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="b679f-109">Esses relatórios podem ajudar a identificar os usuários que podem precisar de suporte adicional para ativar a assinatura do Office.</span><span class="sxs-lookup"><span data-stu-id="b679f-109">These reports could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="b679f-110">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="b679f-110">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="b679f-111">Relatórios</span><span class="sxs-lookup"><span data-stu-id="b679f-111">Reports</span></span>
| <span data-ttu-id="b679f-112">Função</span><span class="sxs-lookup"><span data-stu-id="b679f-112">Function</span></span>                                 | <span data-ttu-id="b679f-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b679f-113">Return Type</span></span> | <span data-ttu-id="b679f-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b679f-114">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="b679f-115">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="b679f-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="b679f-116">Stream</span><span class="sxs-lookup"><span data-stu-id="b679f-116">Stream</span></span>      | <span data-ttu-id="b679f-117">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="b679f-117">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="b679f-118">Obter contagens de ativação</span><span class="sxs-lookup"><span data-stu-id="b679f-118">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="b679f-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="b679f-119">Stream</span></span>      | <span data-ttu-id="b679f-120">Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b679f-120">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="b679f-121">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="b679f-121">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="b679f-122">Fluxo</span><span class="sxs-lookup"><span data-stu-id="b679f-122">Stream</span></span>      | <span data-ttu-id="b679f-123">Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office no desktop ou nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b679f-123">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
