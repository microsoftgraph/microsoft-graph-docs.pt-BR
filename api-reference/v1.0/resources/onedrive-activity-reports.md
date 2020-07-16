---
title: Relatórios de atividades do OneDrive
description: Use os relatórios de atividades do OneDrive para obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive. Esses relatórios podem ajudar você a entender o nível de colaboração acontecendo, mostrando o número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 24a2e74e9e117c13fa49efc6fba4323f75716ffe
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898146"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="37a70-104">Relatórios de atividades do OneDrive</span><span class="sxs-lookup"><span data-stu-id="37a70-104">OneDrive activity reports</span></span>

<span data-ttu-id="37a70-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37a70-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37a70-106">Use os relatórios de atividades do OneDrive para obter a atividade de cada usuário licenciado para usar o OneDrive examinando sua interação com arquivos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="37a70-106">Use the OneDrive activity reports to get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="37a70-107">Esses relatórios podem ajudar você a entender o nível de colaboração acontecendo, mostrando o número de arquivos compartilhados.</span><span class="sxs-lookup"><span data-stu-id="37a70-107">These reports can help you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="37a70-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-onedrive for Business Activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="37a70-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="37a70-109">Relatórios</span><span class="sxs-lookup"><span data-stu-id="37a70-109">Reports</span></span>

| <span data-ttu-id="37a70-110">Função</span><span class="sxs-lookup"><span data-stu-id="37a70-110">Function</span></span>                                 | <span data-ttu-id="37a70-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="37a70-111">Return Type</span></span> | <span data-ttu-id="37a70-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a70-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="37a70-113">Obter dados de usuário</span><span class="sxs-lookup"><span data-stu-id="37a70-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="37a70-114">Stream</span><span class="sxs-lookup"><span data-stu-id="37a70-114">Stream</span></span>      | <span data-ttu-id="37a70-115">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="37a70-115">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="37a70-116">Obter contagens de usuários</span><span class="sxs-lookup"><span data-stu-id="37a70-116">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="37a70-117">Fluxo</span><span class="sxs-lookup"><span data-stu-id="37a70-117">Stream</span></span>      | <span data-ttu-id="37a70-118">Obtenha a tendência no número de usuários ativos do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="37a70-118">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="37a70-119">Obter contagens de arquivo</span><span class="sxs-lookup"><span data-stu-id="37a70-119">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="37a70-120">Fluxo</span><span class="sxs-lookup"><span data-stu-id="37a70-120">Stream</span></span>      | <span data-ttu-id="37a70-121">Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="37a70-121">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |

