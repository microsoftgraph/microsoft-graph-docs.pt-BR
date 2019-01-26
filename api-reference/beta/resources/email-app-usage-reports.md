---
title: Relatórios de uso do aplicativo de email
description: Você pode ver quantos aplicativos de email são usados para conectar ao Exchange Online. Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 7f332359af9a6147894bb69e6d12532a83394bb5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573743"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="93a4e-104">Relatórios de uso do aplicativo de email</span><span class="sxs-lookup"><span data-stu-id="93a4e-104">Email app usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93a4e-105">Você pode ver quantos aplicativos de email são usados para conectar ao Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="93a4e-105">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="93a4e-106">Você também pode ver quais versões de aplicativos do Outlook são usadas, o que permitirá acompanhar os usuários que devem atualizar para versões do Outlook com suporte.</span><span class="sxs-lookup"><span data-stu-id="93a4e-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="93a4e-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="93a4e-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="93a4e-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="93a4e-108">Reports</span></span>

| <span data-ttu-id="93a4e-109">Função</span><span class="sxs-lookup"><span data-stu-id="93a4e-109">Function</span></span>                                 | <span data-ttu-id="93a4e-110">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="93a4e-110">CSV return type</span></span> | <span data-ttu-id="93a4e-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="93a4e-111">JSON return type</span></span>                         | <span data-ttu-id="93a4e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="93a4e-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="93a4e-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="93a4e-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="93a4e-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="93a4e-114">Stream</span></span>          | [<span data-ttu-id="93a4e-115">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="93a4e-115">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="93a4e-116">Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.</span><span class="sxs-lookup"><span data-stu-id="93a4e-116">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="93a4e-117">Obter contagens de usuários do aplicativo</span><span class="sxs-lookup"><span data-stu-id="93a4e-117">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="93a4e-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="93a4e-118">Stream</span></span>          | [<span data-ttu-id="93a4e-119">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="93a4e-119">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="93a4e-120">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="93a4e-120">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="93a4e-121">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="93a4e-121">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="93a4e-122">Fluxo</span><span class="sxs-lookup"><span data-stu-id="93a4e-122">Stream</span></span>          | [<span data-ttu-id="93a4e-123">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="93a4e-123">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="93a4e-124">Obtenha a contagem de usuários únicos conectados ao Exchange Online usando qualquer aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="93a4e-124">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="93a4e-125">Obter contagens de usuários das versões</span><span class="sxs-lookup"><span data-stu-id="93a4e-125">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="93a4e-126">Fluxo</span><span class="sxs-lookup"><span data-stu-id="93a4e-126">Stream</span></span>          | [<span data-ttu-id="93a4e-127">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="93a4e-127">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="93a4e-128">Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="93a4e-128">Get the count of unique users by Outlook desktop version.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-app-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
