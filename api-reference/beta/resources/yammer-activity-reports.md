---
title: Relatórios de atividades do Yammer
description: Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d5953d8bd53158b2ec0532deb47c48028ba1b8c9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523795"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="c8829-103">Relatórios de atividades do Yammer</span><span class="sxs-lookup"><span data-stu-id="c8829-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8829-104">Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.</span><span class="sxs-lookup"><span data-stu-id="c8829-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="c8829-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="c8829-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="c8829-106">Relatórios</span><span class="sxs-lookup"><span data-stu-id="c8829-106">Reports</span></span>

| <span data-ttu-id="c8829-107">Função</span><span class="sxs-lookup"><span data-stu-id="c8829-107">Function</span></span>                                 | <span data-ttu-id="c8829-108">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="c8829-108">CSV return type</span></span> | <span data-ttu-id="c8829-109">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="c8829-109">JSON return type</span></span>                         | <span data-ttu-id="c8829-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8829-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="c8829-111">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="c8829-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="c8829-112">Fluxo</span><span class="sxs-lookup"><span data-stu-id="c8829-112">Stream</span></span>          | [<span data-ttu-id="c8829-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c8829-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="c8829-114">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="c8829-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="c8829-115">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="c8829-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="c8829-116">Fluxo</span><span class="sxs-lookup"><span data-stu-id="c8829-116">Stream</span></span>          | [<span data-ttu-id="c8829-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="c8829-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="c8829-118">Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas.</span><span class="sxs-lookup"><span data-stu-id="c8829-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="c8829-119">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="c8829-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="c8829-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="c8829-120">Stream</span></span>          | [<span data-ttu-id="c8829-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="c8829-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="c8829-122">Obtenha as tendências do número de usuários exclusivos que lançaram, ler e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="c8829-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
