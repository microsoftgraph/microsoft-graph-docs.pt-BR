---
title: Relatórios de uso do aplicativo de email
description: Use os relatórios de uso do aplicativo de email para ver quantos aplicativos de email são usados para se conectar ao Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 9ea3418dd065758fb2d623c9995b78126ea3d475
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532984"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="1829f-104">Relatórios de uso do aplicativo de email</span><span class="sxs-lookup"><span data-stu-id="1829f-104">Email app usage reports</span></span>

<span data-ttu-id="1829f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1829f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1829f-106">Use os relatórios de uso do aplicativo de email para ver quantos aplicativos de email são usados para se conectar ao Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1829f-106">Use the email app usage reports to see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="1829f-107">Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.</span><span class="sxs-lookup"><span data-stu-id="1829f-107">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="1829f-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="1829f-108">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="1829f-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="1829f-109">Reports</span></span>

| <span data-ttu-id="1829f-110">Função</span><span class="sxs-lookup"><span data-stu-id="1829f-110">Function</span></span>                                 | <span data-ttu-id="1829f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1829f-111">Return Type</span></span> | <span data-ttu-id="1829f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1829f-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="1829f-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="1829f-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="1829f-114">Stream</span><span class="sxs-lookup"><span data-stu-id="1829f-114">Stream</span></span>      | <span data-ttu-id="1829f-115">Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.</span><span class="sxs-lookup"><span data-stu-id="1829f-115">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="1829f-116">Obter contagens de usuários do aplicativo</span><span class="sxs-lookup"><span data-stu-id="1829f-116">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="1829f-117">Stream</span><span class="sxs-lookup"><span data-stu-id="1829f-117">Stream</span></span>      | <span data-ttu-id="1829f-118">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="1829f-118">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="1829f-119">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="1829f-119">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="1829f-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="1829f-120">Stream</span></span>      | <span data-ttu-id="1829f-121">Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="1829f-121">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="1829f-122">Obter contagens de usuários das versões</span><span class="sxs-lookup"><span data-stu-id="1829f-122">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="1829f-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="1829f-123">Stream</span></span>      | <span data-ttu-id="1829f-124">Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="1829f-124">Get the count of unique users by Outlook desktop version.</span></span> |
