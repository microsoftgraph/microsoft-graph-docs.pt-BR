---
title: tipo de recurso office365ServicesUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 8600e79d425d15746fd7015adea98eb49a8a3c82
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896550"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="53b19-103">tipo de recurso office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="53b19-103">office365ServicesUserCounts resource type</span></span>

<span data-ttu-id="53b19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53b19-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="53b19-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53b19-105">Properties</span></span>

| <span data-ttu-id="53b19-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53b19-106">Property</span></span>                 | <span data-ttu-id="53b19-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="53b19-107">Type</span></span>   | <span data-ttu-id="53b19-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="53b19-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="53b19-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="53b19-109">reportRefreshDate</span></span>        | <span data-ttu-id="53b19-110">Data</span><span class="sxs-lookup"><span data-stu-id="53b19-110">Date</span></span>   | <span data-ttu-id="53b19-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="53b19-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="53b19-112">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="53b19-112">exchangeActive</span></span>           | <span data-ttu-id="53b19-113">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-113">Int64</span></span>  | <span data-ttu-id="53b19-114">O número de usuários ativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="53b19-114">The number of active users on Exchange.</span></span> <span data-ttu-id="53b19-115">Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="53b19-115">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="53b19-116">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="53b19-116">exchangeInactive</span></span>         | <span data-ttu-id="53b19-117">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-117">Int64</span></span>  | <span data-ttu-id="53b19-118">O número de usuários inativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="53b19-118">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="53b19-119">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="53b19-119">oneDriveActive</span></span>           | <span data-ttu-id="53b19-120">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-120">Int64</span></span>  | <span data-ttu-id="53b19-121">O número de usuários ativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="53b19-121">The number of active users on OneDrive.</span></span> <span data-ttu-id="53b19-122">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, ou arquivos sincronizados é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="53b19-122">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="53b19-123">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="53b19-123">oneDriveInactive</span></span>         | <span data-ttu-id="53b19-124">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-124">Int64</span></span>  | <span data-ttu-id="53b19-125">O número de usuários inativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="53b19-125">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="53b19-126">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="53b19-126">sharePointActive</span></span>         | <span data-ttu-id="53b19-127">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-127">Int64</span></span>  | <span data-ttu-id="53b19-128">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="53b19-128">The number of active users on SharePoint.</span></span> <span data-ttu-id="53b19-129">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, arquivos sincronizados ou páginas do SharePoint exibidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="53b19-129">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="53b19-130">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="53b19-130">sharePointInactive</span></span>       | <span data-ttu-id="53b19-131">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-131">Int64</span></span>  | <span data-ttu-id="53b19-132">O número de usuários inativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="53b19-132">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="53b19-133">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="53b19-133">skypeForBusinessActive</span></span>   | <span data-ttu-id="53b19-134">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-134">Int64</span></span>  | <span data-ttu-id="53b19-135">O número de usuários ativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="53b19-135">The number of active users on Skype For Business.</span></span> <span data-ttu-id="53b19-136">Qualquer usuário que organizou ou participou de conferências ou sessões ponto a ponto Unidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="53b19-136">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="53b19-137">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="53b19-137">skypeForBusinessInactive</span></span> | <span data-ttu-id="53b19-138">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-138">Int64</span></span>  | <span data-ttu-id="53b19-139">O número de usuários inativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="53b19-139">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="53b19-140">yammerActive</span><span class="sxs-lookup"><span data-stu-id="53b19-140">yammerActive</span></span>             | <span data-ttu-id="53b19-141">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-141">Int64</span></span>  | <span data-ttu-id="53b19-142">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="53b19-142">The number of active users on Yammer.</span></span> <span data-ttu-id="53b19-143">Qualquer usuário que possa postar, ler ou gostar de mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="53b19-143">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="53b19-144">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="53b19-144">yammerInactive</span></span>           | <span data-ttu-id="53b19-145">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-145">Int64</span></span>  | <span data-ttu-id="53b19-146">O número de usuários inativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="53b19-146">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="53b19-147">teamsActive</span><span class="sxs-lookup"><span data-stu-id="53b19-147">teamsActive</span></span>              | <span data-ttu-id="53b19-148">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-148">Int64</span></span>  | <span data-ttu-id="53b19-149">O número de usuários ativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="53b19-149">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="53b19-150">Qualquer usuário que lançou mensagens em canais de equipe, mensagens enviadas em sessões de chat privadas ou participou de reuniões ou chamadas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="53b19-150">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="53b19-151">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="53b19-151">teamsInactive</span></span>            | <span data-ttu-id="53b19-152">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-152">Int64</span></span>  | <span data-ttu-id="53b19-153">O número de usuários inativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="53b19-153">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="53b19-154">office365Active</span><span class="sxs-lookup"><span data-stu-id="53b19-154">office365Active</span></span>          | <span data-ttu-id="53b19-155">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-155">Int64</span></span>  | <span data-ttu-id="53b19-156">O número de usuários ativos no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="53b19-156">The number of active users on Microsoft 365.</span></span>   |
| <span data-ttu-id="53b19-157">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="53b19-157">office365Inactive</span></span>        | <span data-ttu-id="53b19-158">Int64</span><span class="sxs-lookup"><span data-stu-id="53b19-158">Int64</span></span>  | <span data-ttu-id="53b19-159">O número de usuários inativos no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="53b19-159">The number of inactive users on Microsoft 365.</span></span>     |
| <span data-ttu-id="53b19-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="53b19-160">reportPeriod</span></span>             | <span data-ttu-id="53b19-161">String</span><span class="sxs-lookup"><span data-stu-id="53b19-161">String</span></span> | <span data-ttu-id="53b19-162">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="53b19-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="53b19-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53b19-163">JSON representation</span></span>

<span data-ttu-id="53b19-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53b19-164">The following is a JSON representation of the resource.</span></span>

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
