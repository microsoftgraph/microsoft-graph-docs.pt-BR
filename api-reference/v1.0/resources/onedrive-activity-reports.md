---
title: Relatórios de atividades do OneDrive
description: Use os relatórios de atividades do OneDrive para obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive. Esses relatórios podem ajudar você a entender o nível de colaboração acontecendo, mostrando o número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0399b7e3d320efbc98c3cf25cd2830a4749d8df5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534167"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="787af-104">Relatórios de atividades do OneDrive</span><span class="sxs-lookup"><span data-stu-id="787af-104">OneDrive activity reports</span></span>

<span data-ttu-id="787af-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="787af-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="787af-106">Use os relatórios de atividades do OneDrive para obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="787af-106">Use the OneDrive activity reports to get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="787af-107">Esses relatórios podem ajudar você a entender o nível de colaboração acontecendo, mostrando o número de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="787af-107">These reports can help you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="787af-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="787af-108">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="787af-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="787af-109">Reports</span></span>

| <span data-ttu-id="787af-110">Função</span><span class="sxs-lookup"><span data-stu-id="787af-110">Function</span></span>                                 | <span data-ttu-id="787af-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="787af-111">Return Type</span></span> | <span data-ttu-id="787af-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="787af-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="787af-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="787af-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="787af-114">Stream</span><span class="sxs-lookup"><span data-stu-id="787af-114">Stream</span></span>      | <span data-ttu-id="787af-115">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="787af-115">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="787af-116">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="787af-116">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="787af-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="787af-117">Stream</span></span>      | <span data-ttu-id="787af-118">Obtenha a tendência no número de usuários ativos do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="787af-118">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="787af-119">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="787af-119">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="787af-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="787af-120">Stream</span></span>      | <span data-ttu-id="787af-121">Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="787af-121">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |

