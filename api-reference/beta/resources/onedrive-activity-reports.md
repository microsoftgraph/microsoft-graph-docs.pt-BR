---
title: Relatórios de atividades do OneDrive
description: Você pode obter a atividade de todos os usuários licenciados para usar o OneDrive observando sua interação com arquivos no OneDrive. Ele também ajuda você a entender o nível de colaboração que está acontecendo mostrando o número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7d0c069d2787b30f37e634757127b6141843a9ed
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983598"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="4a02b-104">Relatórios de atividades do OneDrive</span><span class="sxs-lookup"><span data-stu-id="4a02b-104">OneDrive activity reports</span></span>

<span data-ttu-id="4a02b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a02b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a02b-106">Você pode obter a atividade de cada usuário licenciado para usar o OneDrive analisando sua interação com arquivos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4a02b-106">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="4a02b-107">Ele também ajuda você a entender o nível de colaboração que está acontecendo mostrando o número de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="4a02b-107">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="4a02b-108">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira relatórios do [Microsoft 365 - atividade do OneDrive for Business.](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)</span><span class="sxs-lookup"><span data-stu-id="4a02b-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="4a02b-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="4a02b-109">Reports</span></span>

| <span data-ttu-id="4a02b-110">Função</span><span class="sxs-lookup"><span data-stu-id="4a02b-110">Function</span></span>                                 | <span data-ttu-id="4a02b-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="4a02b-111">CSV return type</span></span> | <span data-ttu-id="4a02b-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="4a02b-112">JSON return type</span></span>                         | <span data-ttu-id="4a02b-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a02b-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="4a02b-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="4a02b-114">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="4a02b-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="4a02b-115">Stream</span></span>          | [<span data-ttu-id="4a02b-116">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4a02b-116">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="4a02b-117">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="4a02b-117">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="4a02b-118">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="4a02b-118">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="4a02b-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="4a02b-119">Stream</span></span>          | [<span data-ttu-id="4a02b-120">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="4a02b-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="4a02b-121">Obtenha a tendência no número de usuários ativos do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4a02b-121">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="4a02b-122">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="4a02b-122">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="4a02b-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="4a02b-123">Stream</span></span>          | [<span data-ttu-id="4a02b-124">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="4a02b-124">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="4a02b-125">Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4a02b-125">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |


