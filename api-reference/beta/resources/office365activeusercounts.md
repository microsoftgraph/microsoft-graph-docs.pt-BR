---
title: tipo de recurso office365ActiveUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: b8e3e90424df29218de7a136e4922df59c4af0b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522467"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="0ca60-103">tipo de recurso office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="0ca60-103">office365ActiveUserCounts resource type</span></span>

<span data-ttu-id="0ca60-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ca60-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0ca60-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ca60-105">Properties</span></span>

| <span data-ttu-id="0ca60-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ca60-106">Property</span></span>          | <span data-ttu-id="0ca60-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ca60-107">Type</span></span>   | <span data-ttu-id="0ca60-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ca60-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="0ca60-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0ca60-109">reportRefreshDate</span></span> | <span data-ttu-id="0ca60-110">Data</span><span class="sxs-lookup"><span data-stu-id="0ca60-110">Date</span></span>   | <span data-ttu-id="0ca60-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0ca60-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="0ca60-112">Office365</span><span class="sxs-lookup"><span data-stu-id="0ca60-112">office365</span></span>         | <span data-ttu-id="0ca60-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0ca60-113">Int64</span></span>  | <span data-ttu-id="0ca60-114">O número de usuários ativos no Office 365.</span><span class="sxs-lookup"><span data-stu-id="0ca60-114">The number of active users in Office 365.</span></span> <span data-ttu-id="0ca60-115">Esse número inclui todos os usuários ativos no Exchange, OneDrive, SharePoint, Skype for Business, Yammer e Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0ca60-115">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="0ca60-116">Você pode encontrar a definição de usuário ativo para cada produto na respectiva descrição da propriedade.</span><span class="sxs-lookup"><span data-stu-id="0ca60-116">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="0ca60-117">câmbio</span><span class="sxs-lookup"><span data-stu-id="0ca60-117">exchange</span></span>          | <span data-ttu-id="0ca60-118">Int64</span><span class="sxs-lookup"><span data-stu-id="0ca60-118">Int64</span></span>  | <span data-ttu-id="0ca60-119">O número de usuários ativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ca60-119">The number of active users in Exchange.</span></span> <span data-ttu-id="0ca60-120">Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0ca60-120">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="0ca60-121">oneDrive</span><span class="sxs-lookup"><span data-stu-id="0ca60-121">oneDrive</span></span>          | <span data-ttu-id="0ca60-122">Int64</span><span class="sxs-lookup"><span data-stu-id="0ca60-122">Int64</span></span>  | <span data-ttu-id="0ca60-123">O número de usuários ativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0ca60-123">The number of active users in OneDrive.</span></span> <span data-ttu-id="0ca60-124">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, ou arquivos sincronizados é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0ca60-124">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="0ca60-125">Do</span><span class="sxs-lookup"><span data-stu-id="0ca60-125">sharePoint</span></span>        | <span data-ttu-id="0ca60-126">Int64</span><span class="sxs-lookup"><span data-stu-id="0ca60-126">Int64</span></span>  | <span data-ttu-id="0ca60-127">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0ca60-127">The number of active users in SharePoint.</span></span> <span data-ttu-id="0ca60-128">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, arquivos sincronizados ou páginas do SharePoint exibidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0ca60-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="0ca60-129">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="0ca60-129">skypeForBusiness</span></span>  | <span data-ttu-id="0ca60-130">Int64</span><span class="sxs-lookup"><span data-stu-id="0ca60-130">Int64</span></span>  | <span data-ttu-id="0ca60-131">O número de usuários ativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="0ca60-131">The number of active users in Skype For Business.</span></span> <span data-ttu-id="0ca60-132">Qualquer usuário que organizou ou participou de conferências ou sessões ponto a ponto Unidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0ca60-132">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="0ca60-133">Yammer</span><span class="sxs-lookup"><span data-stu-id="0ca60-133">yammer</span></span>            | <span data-ttu-id="0ca60-134">Int64</span><span class="sxs-lookup"><span data-stu-id="0ca60-134">Int64</span></span>  | <span data-ttu-id="0ca60-135">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="0ca60-135">The number of active users in Yammer.</span></span> <span data-ttu-id="0ca60-136">Qualquer usuário que possa postar, ler ou gostar de mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0ca60-136">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="0ca60-137">Teams</span><span class="sxs-lookup"><span data-stu-id="0ca60-137">teams</span></span>             | <span data-ttu-id="0ca60-138">Int64</span><span class="sxs-lookup"><span data-stu-id="0ca60-138">Int64</span></span>  | <span data-ttu-id="0ca60-139">O número de usuários ativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0ca60-139">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="0ca60-140">Qualquer usuário que lançou mensagens em canais de equipe, mensagens enviadas em sessões de chat privadas ou participou de reuniões ou chamadas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="0ca60-140">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="0ca60-141">reportDate</span><span class="sxs-lookup"><span data-stu-id="0ca60-141">reportDate</span></span>        | <span data-ttu-id="0ca60-142">Data</span><span class="sxs-lookup"><span data-stu-id="0ca60-142">Date</span></span>   | <span data-ttu-id="0ca60-143">A data em que um número de usuários estava ativo.</span><span class="sxs-lookup"><span data-stu-id="0ca60-143">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="0ca60-144">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0ca60-144">reportPeriod</span></span>      | <span data-ttu-id="0ca60-145">String</span><span class="sxs-lookup"><span data-stu-id="0ca60-145">String</span></span> | <span data-ttu-id="0ca60-146">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="0ca60-146">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="0ca60-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ca60-147">JSON representation</span></span>

<span data-ttu-id="0ca60-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ca60-148">The following is a JSON representation of the resource.</span></span>

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
