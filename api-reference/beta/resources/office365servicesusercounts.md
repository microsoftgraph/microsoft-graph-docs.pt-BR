---
title: tipo de recurso de office365ServicesUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573890"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="2db15-103">tipo de recurso de office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="2db15-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2db15-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2db15-104">Properties</span></span>

| <span data-ttu-id="2db15-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2db15-105">Property</span></span>                 | <span data-ttu-id="2db15-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="2db15-106">Type</span></span>   | <span data-ttu-id="2db15-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="2db15-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2db15-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2db15-108">reportRefreshDate</span></span>        | <span data-ttu-id="2db15-109">Data</span><span class="sxs-lookup"><span data-stu-id="2db15-109">Date</span></span>   | <span data-ttu-id="2db15-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2db15-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="2db15-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="2db15-111">exchangeActive</span></span>           | <span data-ttu-id="2db15-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-112">Int64</span></span>  | <span data-ttu-id="2db15-113">O número de usuários ativos em Exchange.</span><span class="sxs-lookup"><span data-stu-id="2db15-113">The number of active users on Exchange.</span></span> <span data-ttu-id="2db15-114">Qualquer usuário que pode ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="2db15-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="2db15-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="2db15-115">exchangeInactive</span></span>         | <span data-ttu-id="2db15-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-116">Int64</span></span>  | <span data-ttu-id="2db15-117">O número de usuários inativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="2db15-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="2db15-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="2db15-118">oneDriveActive</span></span>           | <span data-ttu-id="2db15-119">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-119">Int64</span></span>  | <span data-ttu-id="2db15-120">O número de usuários ativos em OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2db15-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="2db15-121">Qualquer usuário que são exibidos ou editados arquivos, arquivos compartilhados interna ou externamente ou sincronizados arquivos é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="2db15-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="2db15-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="2db15-122">oneDriveInactive</span></span>         | <span data-ttu-id="2db15-123">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-123">Int64</span></span>  | <span data-ttu-id="2db15-124">O número de usuários inativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2db15-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="2db15-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="2db15-125">sharePointActive</span></span>         | <span data-ttu-id="2db15-126">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-126">Int64</span></span>  | <span data-ttu-id="2db15-127">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2db15-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="2db15-128">Qualquer usuário que exibidos ou editados arquivos, internamente de arquivos compartilhados ou sincronizados arquivos externamente ou exibidos páginas do SharePoint é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="2db15-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="2db15-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="2db15-129">sharePointInactive</span></span>       | <span data-ttu-id="2db15-130">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-130">Int64</span></span>  | <span data-ttu-id="2db15-131">O número de usuários inativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2db15-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="2db15-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="2db15-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="2db15-133">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-133">Int64</span></span>  | <span data-ttu-id="2db15-134">O número de usuários ativos em Skype para negócios.</span><span class="sxs-lookup"><span data-stu-id="2db15-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="2db15-135">Qualquer usuário que organizou participou de conferências ou ingressou sessões ponto a ponto é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="2db15-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="2db15-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="2db15-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="2db15-137">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-137">Int64</span></span>  | <span data-ttu-id="2db15-138">O número de usuários inativos em Skype para negócios.</span><span class="sxs-lookup"><span data-stu-id="2db15-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="2db15-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="2db15-139">yammerActive</span></span>             | <span data-ttu-id="2db15-140">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-140">Int64</span></span>  | <span data-ttu-id="2db15-141">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="2db15-141">The number of active users on Yammer.</span></span> <span data-ttu-id="2db15-142">Qualquer usuário que pode postar, ler ou like mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="2db15-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="2db15-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="2db15-143">yammerInactive</span></span>           | <span data-ttu-id="2db15-144">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-144">Int64</span></span>  | <span data-ttu-id="2db15-145">O número de usuários inativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="2db15-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="2db15-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="2db15-146">teamsActive</span></span>              | <span data-ttu-id="2db15-147">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-147">Int64</span></span>  | <span data-ttu-id="2db15-148">O número de usuários ativos em Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2db15-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="2db15-149">Qualquer usuário que as mensagens postadas no canais de equipe, mensagens enviadas em sessões de bate-papo privado ou participou chamadas ou reuniões é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="2db15-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="2db15-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="2db15-150">teamsInactive</span></span>            | <span data-ttu-id="2db15-151">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-151">Int64</span></span>  | <span data-ttu-id="2db15-152">O número de usuários inativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2db15-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="2db15-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="2db15-153">office365Active</span></span>          | <span data-ttu-id="2db15-154">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-154">Int64</span></span>  | <span data-ttu-id="2db15-155">O número de usuários ativos no Office 365.</span><span class="sxs-lookup"><span data-stu-id="2db15-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="2db15-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="2db15-156">office365Inactive</span></span>        | <span data-ttu-id="2db15-157">Int64</span><span class="sxs-lookup"><span data-stu-id="2db15-157">Int64</span></span>  | <span data-ttu-id="2db15-158">O número de usuários inativos no Office 365.</span><span class="sxs-lookup"><span data-stu-id="2db15-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="2db15-159">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2db15-159">reportPeriod</span></span>             | <span data-ttu-id="2db15-160">String</span><span class="sxs-lookup"><span data-stu-id="2db15-160">String</span></span> | <span data-ttu-id="2db15-161">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="2db15-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2db15-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2db15-162">JSON representation</span></span>

<span data-ttu-id="2db15-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2db15-163">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```
