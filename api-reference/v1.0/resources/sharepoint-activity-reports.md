---
title: Relatório de atividades do SharePoint
description: Você pode usar os relatórios de atividades do SharePoint para obter as atividades de cada usuário licenciado para usar o SharePoint examinando sua interação com arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 80723ffd868d4b936dadb5fcbebcf4f373d2a4de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009153"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="fe65a-104">Relatório de atividades do SharePoint</span><span class="sxs-lookup"><span data-stu-id="fe65a-104">SharePoint activity reports</span></span>

<span data-ttu-id="fe65a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe65a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe65a-106">Você pode usar os relatórios de atividades do SharePoint para obter as atividades de cada usuário licenciado para usar o SharePoint examinando sua interação com arquivos.</span><span class="sxs-lookup"><span data-stu-id="fe65a-106">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="fe65a-107">Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="fe65a-107">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="fe65a-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-SharePoint Activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="fe65a-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="fe65a-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="fe65a-109">Reports</span></span>

| <span data-ttu-id="fe65a-110">Função</span><span class="sxs-lookup"><span data-stu-id="fe65a-110">Function</span></span>                                 | <span data-ttu-id="fe65a-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fe65a-111">Return Type</span></span> | <span data-ttu-id="fe65a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe65a-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="fe65a-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="fe65a-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="fe65a-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="fe65a-114">Stream</span></span>      | <span data-ttu-id="fe65a-115">Obtenha dados sobre as atividades do SharePoint por usuário.</span><span class="sxs-lookup"><span data-stu-id="fe65a-115">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="fe65a-116">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="fe65a-116">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="fe65a-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="fe65a-117">Stream</span></span>      | <span data-ttu-id="fe65a-118">Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fe65a-118">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="fe65a-119">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="fe65a-119">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="fe65a-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="fe65a-120">Stream</span></span>      | <span data-ttu-id="fe65a-121">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="fe65a-121">Get the trend in the number of active users.</span></span> <span data-ttu-id="fe65a-122">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="fe65a-122">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="fe65a-123">Obter páginas</span><span class="sxs-lookup"><span data-stu-id="fe65a-123">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="fe65a-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="fe65a-124">Stream</span></span>      | <span data-ttu-id="fe65a-125">Obtenha o número de páginas exclusivas visitadas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="fe65a-125">Get the number of unique pages visited by users.</span></span> |

