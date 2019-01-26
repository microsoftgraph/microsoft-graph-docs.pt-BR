---
title: tipo de recurso de office365ActiveUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bbc51e4859b005c01b0f8d2cfb2db3ca902d60e2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572203"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="590f3-103">tipo de recurso de office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="590f3-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="590f3-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="590f3-104">Properties</span></span>

| <span data-ttu-id="590f3-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="590f3-105">Property</span></span>          | <span data-ttu-id="590f3-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="590f3-106">Type</span></span>   | <span data-ttu-id="590f3-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="590f3-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="590f3-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="590f3-108">reportRefreshDate</span></span> | <span data-ttu-id="590f3-109">Data</span><span class="sxs-lookup"><span data-stu-id="590f3-109">Date</span></span>   | <span data-ttu-id="590f3-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="590f3-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="590f3-111">office365</span><span class="sxs-lookup"><span data-stu-id="590f3-111">office365</span></span>         | <span data-ttu-id="590f3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="590f3-112">Int64</span></span>  | <span data-ttu-id="590f3-113">O número de usuários ativos no Office 365.</span><span class="sxs-lookup"><span data-stu-id="590f3-113">The number of active users in Office 365.</span></span> <span data-ttu-id="590f3-114">Esse número inclui todos os usuários ativos no Exchange, OneDrive, SharePoint, Skype For Business, Yammer e Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="590f3-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="590f3-115">Você pode encontrar a definição de usuário ativo para cada produto na descrição do respectivas propriedades.</span><span class="sxs-lookup"><span data-stu-id="590f3-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="590f3-116">Exchange</span><span class="sxs-lookup"><span data-stu-id="590f3-116">exchange</span></span>          | <span data-ttu-id="590f3-117">Int64</span><span class="sxs-lookup"><span data-stu-id="590f3-117">Int64</span></span>  | <span data-ttu-id="590f3-118">O número de usuários ativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="590f3-118">The number of active users in Exchange.</span></span> <span data-ttu-id="590f3-119">Qualquer usuário que pode ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="590f3-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="590f3-120">oneDrive</span><span class="sxs-lookup"><span data-stu-id="590f3-120">oneDrive</span></span>          | <span data-ttu-id="590f3-121">Int64</span><span class="sxs-lookup"><span data-stu-id="590f3-121">Int64</span></span>  | <span data-ttu-id="590f3-122">O número de usuários ativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="590f3-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="590f3-123">Qualquer usuário que são exibidos ou editados arquivos, arquivos compartilhados interna ou externamente ou sincronizados arquivos é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="590f3-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="590f3-124">sharePoint</span><span class="sxs-lookup"><span data-stu-id="590f3-124">sharePoint</span></span>        | <span data-ttu-id="590f3-125">Int64</span><span class="sxs-lookup"><span data-stu-id="590f3-125">Int64</span></span>  | <span data-ttu-id="590f3-126">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="590f3-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="590f3-127">Qualquer usuário que exibidos ou editados arquivos, internamente de arquivos compartilhados ou sincronizados arquivos externamente ou exibidos páginas do SharePoint é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="590f3-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="590f3-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="590f3-128">skypeForBusiness</span></span>  | <span data-ttu-id="590f3-129">Int64</span><span class="sxs-lookup"><span data-stu-id="590f3-129">Int64</span></span>  | <span data-ttu-id="590f3-130">O número de usuários ativos em Skype para negócios.</span><span class="sxs-lookup"><span data-stu-id="590f3-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="590f3-131">Qualquer usuário que organizou participou de conferências ou ingressou sessões ponto a ponto é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="590f3-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="590f3-132">Yammer</span><span class="sxs-lookup"><span data-stu-id="590f3-132">yammer</span></span>            | <span data-ttu-id="590f3-133">Int64</span><span class="sxs-lookup"><span data-stu-id="590f3-133">Int64</span></span>  | <span data-ttu-id="590f3-134">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="590f3-134">The number of active users in Yammer.</span></span> <span data-ttu-id="590f3-135">Qualquer usuário que pode postar, ler ou like mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="590f3-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="590f3-136">equipes</span><span class="sxs-lookup"><span data-stu-id="590f3-136">teams</span></span>             | <span data-ttu-id="590f3-137">Int64</span><span class="sxs-lookup"><span data-stu-id="590f3-137">Int64</span></span>  | <span data-ttu-id="590f3-138">O número de usuários ativos em Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="590f3-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="590f3-139">Qualquer usuário que as mensagens postadas no canais de equipe, mensagens enviadas em sessões de bate-papo privado ou participou chamadas ou reuniões é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="590f3-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="590f3-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="590f3-140">reportDate</span></span>        | <span data-ttu-id="590f3-141">Data</span><span class="sxs-lookup"><span data-stu-id="590f3-141">Date</span></span>   | <span data-ttu-id="590f3-142">A data em que um número de usuários estava ativo.</span><span class="sxs-lookup"><span data-stu-id="590f3-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="590f3-143">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="590f3-143">reportPeriod</span></span>      | <span data-ttu-id="590f3-144">String</span><span class="sxs-lookup"><span data-stu-id="590f3-144">String</span></span> | <span data-ttu-id="590f3-145">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="590f3-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="590f3-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="590f3-146">JSON representation</span></span>

<span data-ttu-id="590f3-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="590f3-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
