---
title: tipo de recurso office365ServicesUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 80bfb483e7e15dcdaffb6a8ba8ed30c8bb508f5c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092353"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="0b39f-103">tipo de recurso office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="0b39f-103">office365ServicesUserCounts resource type</span></span>

<span data-ttu-id="0b39f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b39f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0b39f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b39f-105">Properties</span></span>

| <span data-ttu-id="0b39f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b39f-106">Property</span></span>                 | <span data-ttu-id="0b39f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b39f-107">Type</span></span>   | <span data-ttu-id="0b39f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b39f-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="0b39f-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0b39f-109">reportRefreshDate</span></span>        | <span data-ttu-id="0b39f-110">Data</span><span class="sxs-lookup"><span data-stu-id="0b39f-110">Date</span></span>   | <span data-ttu-id="0b39f-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0b39f-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="0b39f-112">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="0b39f-112">exchangeActive</span></span>           | <span data-ttu-id="0b39f-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-113">Int64</span></span>  | <span data-ttu-id="0b39f-114">O número de usuários ativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b39f-114">The number of active users on Exchange.</span></span> <span data-ttu-id="0b39f-115">Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0b39f-115">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="0b39f-116">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="0b39f-116">exchangeInactive</span></span>         | <span data-ttu-id="0b39f-117">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-117">Int64</span></span>  | <span data-ttu-id="0b39f-118">O número de usuários inativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b39f-118">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="0b39f-119">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="0b39f-119">oneDriveActive</span></span>           | <span data-ttu-id="0b39f-120">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-120">Int64</span></span>  | <span data-ttu-id="0b39f-121">O número de usuários ativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0b39f-121">The number of active users on OneDrive.</span></span> <span data-ttu-id="0b39f-122">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, ou arquivos sincronizados é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0b39f-122">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="0b39f-123">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="0b39f-123">oneDriveInactive</span></span>         | <span data-ttu-id="0b39f-124">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-124">Int64</span></span>  | <span data-ttu-id="0b39f-125">O número de usuários inativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0b39f-125">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="0b39f-126">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="0b39f-126">sharePointActive</span></span>         | <span data-ttu-id="0b39f-127">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-127">Int64</span></span>  | <span data-ttu-id="0b39f-128">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0b39f-128">The number of active users on SharePoint.</span></span> <span data-ttu-id="0b39f-129">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, arquivos sincronizados ou páginas do SharePoint exibidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0b39f-129">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="0b39f-130">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="0b39f-130">sharePointInactive</span></span>       | <span data-ttu-id="0b39f-131">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-131">Int64</span></span>  | <span data-ttu-id="0b39f-132">O número de usuários inativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0b39f-132">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="0b39f-133">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="0b39f-133">skypeForBusinessActive</span></span>   | <span data-ttu-id="0b39f-134">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-134">Int64</span></span>  | <span data-ttu-id="0b39f-135">O número de usuários ativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="0b39f-135">The number of active users on Skype For Business.</span></span> <span data-ttu-id="0b39f-136">Qualquer usuário que organizou ou participou de conferências ou sessões ponto a ponto Unidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0b39f-136">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="0b39f-137">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="0b39f-137">skypeForBusinessInactive</span></span> | <span data-ttu-id="0b39f-138">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-138">Int64</span></span>  | <span data-ttu-id="0b39f-139">O número de usuários inativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="0b39f-139">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="0b39f-140">yammerActive</span><span class="sxs-lookup"><span data-stu-id="0b39f-140">yammerActive</span></span>             | <span data-ttu-id="0b39f-141">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-141">Int64</span></span>  | <span data-ttu-id="0b39f-142">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="0b39f-142">The number of active users on Yammer.</span></span> <span data-ttu-id="0b39f-143">Qualquer usuário que possa postar, ler ou gostar de mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0b39f-143">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="0b39f-144">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="0b39f-144">yammerInactive</span></span>           | <span data-ttu-id="0b39f-145">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-145">Int64</span></span>  | <span data-ttu-id="0b39f-146">O número de usuários inativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="0b39f-146">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="0b39f-147">teamsActive</span><span class="sxs-lookup"><span data-stu-id="0b39f-147">teamsActive</span></span>              | <span data-ttu-id="0b39f-148">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-148">Int64</span></span>  | <span data-ttu-id="0b39f-149">O número de usuários ativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0b39f-149">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="0b39f-150">Qualquer usuário que lançou mensagens em canais de equipe, mensagens enviadas em sessões de chat privadas ou participou de reuniões ou chamadas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0b39f-150">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="0b39f-151">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="0b39f-151">teamsInactive</span></span>            | <span data-ttu-id="0b39f-152">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-152">Int64</span></span>  | <span data-ttu-id="0b39f-153">O número de usuários inativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0b39f-153">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="0b39f-154">office365Active</span><span class="sxs-lookup"><span data-stu-id="0b39f-154">office365Active</span></span>          | <span data-ttu-id="0b39f-155">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-155">Int64</span></span>  | <span data-ttu-id="0b39f-156">O número de usuários ativos no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0b39f-156">The number of active users on Microsoft 365.</span></span>   |
| <span data-ttu-id="0b39f-157">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="0b39f-157">office365Inactive</span></span>        | <span data-ttu-id="0b39f-158">Int64</span><span class="sxs-lookup"><span data-stu-id="0b39f-158">Int64</span></span>  | <span data-ttu-id="0b39f-159">O número de usuários inativos no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0b39f-159">The number of inactive users on Microsoft 365.</span></span>     |
| <span data-ttu-id="0b39f-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0b39f-160">reportPeriod</span></span>             | <span data-ttu-id="0b39f-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b39f-161">String</span></span> | <span data-ttu-id="0b39f-162">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="0b39f-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="0b39f-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b39f-163">JSON representation</span></span>

<span data-ttu-id="0b39f-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b39f-164">The following is a JSON representation of the resource.</span></span>

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


