---
title: Relatório de atividades do SharePoint
description: Você pode usar os relatórios de atividades do SharePoint para obter as atividades de cada usuário licenciado para usar o SharePoint examinando sua interação com arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: defa0efa39a9eea57f9304663e42d0214b4305b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446881"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="38999-104">Relatório de atividades do SharePoint</span><span class="sxs-lookup"><span data-stu-id="38999-104">SharePoint activity reports</span></span>

<span data-ttu-id="38999-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="38999-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38999-106">Você pode usar os relatórios de atividades do SharePoint para obter as atividades de cada usuário licenciado para usar o SharePoint examinando sua interação com arquivos.</span><span class="sxs-lookup"><span data-stu-id="38999-106">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="38999-107">Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="38999-107">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="38999-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="38999-108">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="38999-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="38999-109">Reports</span></span>

| <span data-ttu-id="38999-110">Função</span><span class="sxs-lookup"><span data-stu-id="38999-110">Function</span></span>                                 | <span data-ttu-id="38999-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38999-111">Return Type</span></span> | <span data-ttu-id="38999-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="38999-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="38999-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="38999-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="38999-114">Stream</span><span class="sxs-lookup"><span data-stu-id="38999-114">Stream</span></span>      | <span data-ttu-id="38999-115">Obtenha dados sobre as atividades do SharePoint por usuário.</span><span class="sxs-lookup"><span data-stu-id="38999-115">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="38999-116">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="38999-116">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="38999-117">Stream</span><span class="sxs-lookup"><span data-stu-id="38999-117">Stream</span></span>      | <span data-ttu-id="38999-118">Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="38999-118">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="38999-119">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="38999-119">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="38999-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="38999-120">Stream</span></span>      | <span data-ttu-id="38999-121">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="38999-121">Get the trend in the number of active users.</span></span> <span data-ttu-id="38999-122">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="38999-122">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="38999-123">Obter páginas</span><span class="sxs-lookup"><span data-stu-id="38999-123">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="38999-124">Fluxo</span><span class="sxs-lookup"><span data-stu-id="38999-124">Stream</span></span>      | <span data-ttu-id="38999-125">Obtenha o número de páginas exclusivas visitadas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="38999-125">Get the number of unique pages visited by users.</span></span> |
