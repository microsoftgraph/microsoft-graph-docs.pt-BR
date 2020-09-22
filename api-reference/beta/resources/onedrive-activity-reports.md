---
title: Relatórios de atividades do OneDrive
description: Você pode obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive. Ele também ajuda você a entender o nível de colaboração em andamento, mostrando o número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 656d722a9d63e460cd4b62e87a0b2fd8483e37c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092332"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="76e49-104">Relatórios de atividades do OneDrive</span><span class="sxs-lookup"><span data-stu-id="76e49-104">OneDrive activity reports</span></span>

<span data-ttu-id="76e49-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76e49-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76e49-106">Você pode obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="76e49-106">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="76e49-107">Ele também ajuda você a entender o nível de colaboração em andamento, mostrando o número de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="76e49-107">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="76e49-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-onedrive for Business Activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="76e49-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="76e49-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="76e49-109">Reports</span></span>

| <span data-ttu-id="76e49-110">Função</span><span class="sxs-lookup"><span data-stu-id="76e49-110">Function</span></span>                                 | <span data-ttu-id="76e49-111">Tipo de retorno CSV</span><span class="sxs-lookup"><span data-stu-id="76e49-111">CSV return type</span></span> | <span data-ttu-id="76e49-112">Tipo de retorno JSON</span><span class="sxs-lookup"><span data-stu-id="76e49-112">JSON return type</span></span>                         | <span data-ttu-id="76e49-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="76e49-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="76e49-114">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="76e49-114">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="76e49-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="76e49-115">Stream</span></span>          | [<span data-ttu-id="76e49-116">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="76e49-116">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="76e49-117">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="76e49-117">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="76e49-118">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="76e49-118">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="76e49-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="76e49-119">Stream</span></span>          | [<span data-ttu-id="76e49-120">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="76e49-120">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="76e49-121">Obtenha a tendência no número de usuários ativos do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="76e49-121">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="76e49-122">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="76e49-122">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="76e49-123">Fluxo</span><span class="sxs-lookup"><span data-stu-id="76e49-123">Stream</span></span>          | [<span data-ttu-id="76e49-124">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="76e49-124">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="76e49-125">Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="76e49-125">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |


