---
title: Relatórios de uso do aplicativo de email
description: Você pode ver quantos aplicativos de email são usados para se conectar ao Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 03d33080a1d37512431c1922c217a8abe83a4828
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055516"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="dda2c-104">Relatórios de uso do aplicativo de email</span><span class="sxs-lookup"><span data-stu-id="dda2c-104">Email app usage reports</span></span>

<span data-ttu-id="dda2c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dda2c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dda2c-106">Você pode ver quantos aplicativos de email são usados para se conectar ao Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="dda2c-106">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="dda2c-107">Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.</span><span class="sxs-lookup"><span data-stu-id="dda2c-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="dda2c-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="dda2c-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="dda2c-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="dda2c-109">Reports</span></span>

| <span data-ttu-id="dda2c-110">Função</span><span class="sxs-lookup"><span data-stu-id="dda2c-110">Function</span></span>                                 | <span data-ttu-id="dda2c-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="dda2c-111">CSV return type</span></span> | <span data-ttu-id="dda2c-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="dda2c-112">JSON return type</span></span>                         | <span data-ttu-id="dda2c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="dda2c-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="dda2c-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="dda2c-114">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="dda2c-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="dda2c-115">Stream</span></span>          | [<span data-ttu-id="dda2c-116">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="dda2c-116">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="dda2c-117">Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.</span><span class="sxs-lookup"><span data-stu-id="dda2c-117">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="dda2c-118">Obter contagens de usuários do aplicativo</span><span class="sxs-lookup"><span data-stu-id="dda2c-118">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="dda2c-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="dda2c-119">Stream</span></span>          | [<span data-ttu-id="dda2c-120">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="dda2c-120">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="dda2c-121">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="dda2c-121">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="dda2c-122">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="dda2c-122">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="dda2c-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="dda2c-123">Stream</span></span>          | [<span data-ttu-id="dda2c-124">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="dda2c-124">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="dda2c-125">Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="dda2c-125">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="dda2c-126">Obter contagens de usuários das versões</span><span class="sxs-lookup"><span data-stu-id="dda2c-126">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="dda2c-127">Fluxo</span><span class="sxs-lookup"><span data-stu-id="dda2c-127">Stream</span></span>          | [<span data-ttu-id="dda2c-128">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="dda2c-128">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="dda2c-129">Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="dda2c-129">Get the count of unique users by Outlook desktop version.</span></span> |


