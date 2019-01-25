---
title: Relatórios de atividades do OneDrive
description: Você pode obter a atividade de todos os usuários licenciados para usar o OneDrive examinando sua interação com os arquivos no OneDrive. Ele também ajuda a entender o nível de colaboração em andamento, mostrando o número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 9075bd042a0c27debc8017a007351428191e9d43
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519224"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="83f59-104">Relatórios de atividades do OneDrive</span><span class="sxs-lookup"><span data-stu-id="83f59-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83f59-105">Você pode obter a atividade de todos os usuários licenciados para usar o OneDrive examinando sua interação com os arquivos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="83f59-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="83f59-106">Ele também ajuda a entender o nível de colaboração em andamento, mostrando o número de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="83f59-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="83f59-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="83f59-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="83f59-108">Relatórios</span><span class="sxs-lookup"><span data-stu-id="83f59-108">Reports</span></span>

| <span data-ttu-id="83f59-109">Função</span><span class="sxs-lookup"><span data-stu-id="83f59-109">Function</span></span>                                 | <span data-ttu-id="83f59-110">Tipo de retorno de CSV</span><span class="sxs-lookup"><span data-stu-id="83f59-110">CSV return type</span></span> | <span data-ttu-id="83f59-111">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="83f59-111">JSON return type</span></span>                         | <span data-ttu-id="83f59-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="83f59-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="83f59-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="83f59-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="83f59-114">Stream</span><span class="sxs-lookup"><span data-stu-id="83f59-114">Stream</span></span>          | [<span data-ttu-id="83f59-115">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="83f59-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="83f59-116">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="83f59-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="83f59-117">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="83f59-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="83f59-118">Fluxo</span><span class="sxs-lookup"><span data-stu-id="83f59-118">Stream</span></span>          | [<span data-ttu-id="83f59-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="83f59-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="83f59-120">Obtenha a tendência no número de usuários ativos do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="83f59-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="83f59-121">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="83f59-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="83f59-122">Stream</span><span class="sxs-lookup"><span data-stu-id="83f59-122">Stream</span></span>          | [<span data-ttu-id="83f59-123">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="83f59-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="83f59-124">Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="83f59-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
