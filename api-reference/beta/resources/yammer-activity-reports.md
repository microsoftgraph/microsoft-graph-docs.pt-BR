---
title: Relatórios de atividades do Yammer
description: Você pode compreender o nível de participação da sua organização com o Yammer por quanto atividade é gerada entre a organização e o número de usuários exclusivos que postar, like e ler mensagens no Yammer.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 252748b639f256467b2a01336488e1df086c69cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509935"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="d320b-103">Relatórios de atividades do Yammer</span><span class="sxs-lookup"><span data-stu-id="d320b-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d320b-104">Você pode compreender o nível de participação da sua organização com o Yammer por quanto atividade é gerada entre a organização e o número de usuários exclusivos que postar, like e ler mensagens no Yammer.</span><span class="sxs-lookup"><span data-stu-id="d320b-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="d320b-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="d320b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="d320b-106">Relatórios</span><span class="sxs-lookup"><span data-stu-id="d320b-106">Reports</span></span>

| <span data-ttu-id="d320b-107">Função</span><span class="sxs-lookup"><span data-stu-id="d320b-107">Function</span></span>                                 | <span data-ttu-id="d320b-108">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="d320b-108">CSV return type</span></span> | <span data-ttu-id="d320b-109">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="d320b-109">JSON return type</span></span>                         | <span data-ttu-id="d320b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d320b-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="d320b-111">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="d320b-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="d320b-112">Stream</span><span class="sxs-lookup"><span data-stu-id="d320b-112">Stream</span></span>          | [<span data-ttu-id="d320b-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d320b-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="d320b-114">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="d320b-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="d320b-115">Obter contagens de atividade</span><span class="sxs-lookup"><span data-stu-id="d320b-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="d320b-116">Fluxo</span><span class="sxs-lookup"><span data-stu-id="d320b-116">Stream</span></span>          | [<span data-ttu-id="d320b-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="d320b-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="d320b-118">Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas.</span><span class="sxs-lookup"><span data-stu-id="d320b-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="d320b-119">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="d320b-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="d320b-120">Stream</span><span class="sxs-lookup"><span data-stu-id="d320b-120">Stream</span></span>          | [<span data-ttu-id="d320b-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="d320b-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="d320b-122">Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="d320b-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
