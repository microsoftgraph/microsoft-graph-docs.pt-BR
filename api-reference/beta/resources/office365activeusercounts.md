---
title: Tipo de recurso office365ActiveUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 67c9b898da9a106685739ebbf78ccef6425c6617
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980735"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="3eb9b-103">Tipo de recurso office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="3eb9b-103">office365ActiveUserCounts resource type</span></span>

<span data-ttu-id="3eb9b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eb9b-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3eb9b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3eb9b-105">Properties</span></span>

| <span data-ttu-id="3eb9b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3eb9b-106">Property</span></span>          | <span data-ttu-id="3eb9b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3eb9b-107">Type</span></span>   | <span data-ttu-id="3eb9b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eb9b-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="3eb9b-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3eb9b-109">reportRefreshDate</span></span> | <span data-ttu-id="3eb9b-110">Data</span><span class="sxs-lookup"><span data-stu-id="3eb9b-110">Date</span></span>   | <span data-ttu-id="3eb9b-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="3eb9b-112">office365</span><span class="sxs-lookup"><span data-stu-id="3eb9b-112">office365</span></span>         | <span data-ttu-id="3eb9b-113">Int64</span><span class="sxs-lookup"><span data-stu-id="3eb9b-113">Int64</span></span>  | <span data-ttu-id="3eb9b-114">O número de usuários ativos no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-114">The number of active users in Microsoft 365.</span></span> <span data-ttu-id="3eb9b-115">Esse número inclui todos os usuários ativos no Exchange, OneDrive, SharePoint, Skype For Business, Yammer e Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-115">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="3eb9b-116">Você pode encontrar a definição de usuário ativo para cada produto na descrição da respectiva propriedade.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-116">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="3eb9b-117">exchange</span><span class="sxs-lookup"><span data-stu-id="3eb9b-117">exchange</span></span>          | <span data-ttu-id="3eb9b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="3eb9b-118">Int64</span></span>  | <span data-ttu-id="3eb9b-119">O número de usuários ativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-119">The number of active users in Exchange.</span></span> <span data-ttu-id="3eb9b-120">Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-120">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="3eb9b-121">oneDrive</span><span class="sxs-lookup"><span data-stu-id="3eb9b-121">oneDrive</span></span>          | <span data-ttu-id="3eb9b-122">Int64</span><span class="sxs-lookup"><span data-stu-id="3eb9b-122">Int64</span></span>  | <span data-ttu-id="3eb9b-123">O número de usuários ativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-123">The number of active users in OneDrive.</span></span> <span data-ttu-id="3eb9b-124">Qualquer usuário que visualizou ou editou arquivos, compartilhou arquivos interna ou externamente ou sincronizou arquivos é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-124">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="3eb9b-125">sharePoint</span><span class="sxs-lookup"><span data-stu-id="3eb9b-125">sharePoint</span></span>        | <span data-ttu-id="3eb9b-126">Int64</span><span class="sxs-lookup"><span data-stu-id="3eb9b-126">Int64</span></span>  | <span data-ttu-id="3eb9b-127">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-127">The number of active users in SharePoint.</span></span> <span data-ttu-id="3eb9b-128">Qualquer usuário que visualizou ou editou arquivos, compartilhou arquivos interna ou externamente, sincronizou arquivos ou visualizou páginas do SharePoint é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="3eb9b-129">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="3eb9b-129">skypeForBusiness</span></span>  | <span data-ttu-id="3eb9b-130">Int64</span><span class="sxs-lookup"><span data-stu-id="3eb9b-130">Int64</span></span>  | <span data-ttu-id="3eb9b-131">O número de usuários ativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-131">The number of active users in Skype For Business.</span></span> <span data-ttu-id="3eb9b-132">Qualquer usuário que organizou ou participou de conferências ou ingressou em sessões ponto a ponto é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-132">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="3eb9b-133">yammer</span><span class="sxs-lookup"><span data-stu-id="3eb9b-133">yammer</span></span>            | <span data-ttu-id="3eb9b-134">Int64</span><span class="sxs-lookup"><span data-stu-id="3eb9b-134">Int64</span></span>  | <span data-ttu-id="3eb9b-135">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-135">The number of active users in Yammer.</span></span> <span data-ttu-id="3eb9b-136">Qualquer usuário que possa postar, ler ou como mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-136">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="3eb9b-137">teams</span><span class="sxs-lookup"><span data-stu-id="3eb9b-137">teams</span></span>             | <span data-ttu-id="3eb9b-138">Int64</span><span class="sxs-lookup"><span data-stu-id="3eb9b-138">Int64</span></span>  | <span data-ttu-id="3eb9b-139">O número de usuários ativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-139">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="3eb9b-140">Qualquer usuário que postou mensagens em canais de equipe, enviou mensagens em sessões de chat privado ou participou de reuniões ou chamadas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-140">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="3eb9b-141">reportDate</span><span class="sxs-lookup"><span data-stu-id="3eb9b-141">reportDate</span></span>        | <span data-ttu-id="3eb9b-142">Data</span><span class="sxs-lookup"><span data-stu-id="3eb9b-142">Date</span></span>   | <span data-ttu-id="3eb9b-143">A data em que um número de usuários estava ativo.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-143">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="3eb9b-144">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3eb9b-144">reportPeriod</span></span>      | <span data-ttu-id="3eb9b-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3eb9b-145">String</span></span> | <span data-ttu-id="3eb9b-146">O número de dias que o relatório abrange.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-146">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="3eb9b-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3eb9b-147">JSON representation</span></span>

<span data-ttu-id="3eb9b-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3eb9b-148">The following is a JSON representation of the resource.</span></span>

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


