---
title: Relatórios de uso do aplicativo de email
description: Você pode ver quantos aplicativos de email são usados para se conectar ao Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: efa7a747ae26da8f34c32d9473a84f95b7433ee0
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982702"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="dc99e-104">Relatórios de uso do aplicativo de email</span><span class="sxs-lookup"><span data-stu-id="dc99e-104">Email app usage reports</span></span>

<span data-ttu-id="dc99e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc99e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc99e-106">Você pode ver quantos aplicativos de email são usados para se conectar ao Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="dc99e-106">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="dc99e-107">Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.</span><span class="sxs-lookup"><span data-stu-id="dc99e-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="dc99e-108">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - Uso de aplicativos de email.](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)</span><span class="sxs-lookup"><span data-stu-id="dc99e-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="dc99e-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="dc99e-109">Reports</span></span>

| <span data-ttu-id="dc99e-110">Função</span><span class="sxs-lookup"><span data-stu-id="dc99e-110">Function</span></span>                                 | <span data-ttu-id="dc99e-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="dc99e-111">CSV return type</span></span> | <span data-ttu-id="dc99e-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="dc99e-112">JSON return type</span></span>                         | <span data-ttu-id="dc99e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc99e-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="dc99e-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="dc99e-114">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="dc99e-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="dc99e-115">Stream</span></span>          | [<span data-ttu-id="dc99e-116">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="dc99e-116">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="dc99e-117">Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.</span><span class="sxs-lookup"><span data-stu-id="dc99e-117">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="dc99e-118">Obter contagens de usuários do aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc99e-118">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="dc99e-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="dc99e-119">Stream</span></span>          | [<span data-ttu-id="dc99e-120">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="dc99e-120">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="dc99e-121">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="dc99e-121">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="dc99e-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="dc99e-122">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="dc99e-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="dc99e-123">Stream</span></span>          | [<span data-ttu-id="dc99e-124">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="dc99e-124">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="dc99e-125">Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="dc99e-125">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="dc99e-126">Obter contagens de usuários das versões</span><span class="sxs-lookup"><span data-stu-id="dc99e-126">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="dc99e-127">Fluxo</span><span class="sxs-lookup"><span data-stu-id="dc99e-127">Stream</span></span>          | [<span data-ttu-id="dc99e-128">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="dc99e-128">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="dc99e-129">Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="dc99e-129">Get the count of unique users by Outlook desktop version.</span></span> |


