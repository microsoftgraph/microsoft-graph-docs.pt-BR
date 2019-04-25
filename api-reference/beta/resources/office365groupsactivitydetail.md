---
title: tipo de recurso office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b467f73ed2a4a5e48cb1243c5b1326591bcd707
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581447"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="bc625-103">tipo de recurso office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="bc625-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bc625-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc625-104">Properties</span></span>

| <span data-ttu-id="bc625-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc625-105">Property</span></span>                          | <span data-ttu-id="bc625-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc625-106">Type</span></span>    | <span data-ttu-id="bc625-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc625-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="bc625-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bc625-108">reportRefreshDate</span></span>                 | <span data-ttu-id="bc625-109">Data</span><span class="sxs-lookup"><span data-stu-id="bc625-109">Date</span></span>    | <span data-ttu-id="bc625-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bc625-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="bc625-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="bc625-111">groupDisplayName</span></span>                  | <span data-ttu-id="bc625-112">String</span><span class="sxs-lookup"><span data-stu-id="bc625-112">String</span></span>  | <span data-ttu-id="bc625-113">O nome de exibição do grupo.</span><span class="sxs-lookup"><span data-stu-id="bc625-113">The display name of the group.</span></span>           |
| <span data-ttu-id="bc625-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="bc625-114">isDeleted</span></span>                         | <span data-ttu-id="bc625-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="bc625-115">Boolean</span></span> | <span data-ttu-id="bc625-116">Se este usuário foi excluído ou excluído por software.</span><span class="sxs-lookup"><span data-stu-id="bc625-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="bc625-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc625-117">ownerPrincipalName</span></span>                | <span data-ttu-id="bc625-118">String</span><span class="sxs-lookup"><span data-stu-id="bc625-118">String</span></span>  | <span data-ttu-id="bc625-119">O nome principal do proprietário do grupo.</span><span class="sxs-lookup"><span data-stu-id="bc625-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="bc625-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="bc625-120">lastActivityDate</span></span>                  | <span data-ttu-id="bc625-121">Data</span><span class="sxs-lookup"><span data-stu-id="bc625-121">Date</span></span>    | <span data-ttu-id="bc625-122">A data da última atividade dos seguintes cenários: caixa de correio de grupo recebidas emails; arquivos de usuário exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint; páginas do SharePoint exibidas pelo usuário; mensagens postadas, lidas ou curtidas pelo usuário em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="bc625-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="bc625-123">groupType</span><span class="sxs-lookup"><span data-stu-id="bc625-123">groupType</span></span>                         | <span data-ttu-id="bc625-124">String</span><span class="sxs-lookup"><span data-stu-id="bc625-124">String</span></span>  | <span data-ttu-id="bc625-125">O tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="bc625-125">The group type.</span></span> <span data-ttu-id="bc625-126">Os valores possíveis são: **Public** ou **Private**.</span><span class="sxs-lookup"><span data-stu-id="bc625-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="bc625-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="bc625-127">memberCount</span></span>                       | <span data-ttu-id="bc625-128">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-128">Int64</span></span>   | <span data-ttu-id="bc625-129">A contagem de membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="bc625-129">The group member count.</span></span>                  |
| <span data-ttu-id="bc625-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="bc625-130">externalMemberCount</span></span>               | <span data-ttu-id="bc625-131">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-131">Int64</span></span>   | <span data-ttu-id="bc625-132">A contagem de membros externos de grupo.</span><span class="sxs-lookup"><span data-stu-id="bc625-132">The group external member count.</span></span>         |
| <span data-ttu-id="bc625-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="bc625-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="bc625-134">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-134">Int64</span></span>   | <span data-ttu-id="bc625-135">O número de emails que a caixa de correio de grupo recebeu.</span><span class="sxs-lookup"><span data-stu-id="bc625-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="bc625-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="bc625-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="bc625-137">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-137">Int64</span></span>   | <span data-ttu-id="bc625-138">O número de arquivos ativos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bc625-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="bc625-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="bc625-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="bc625-140">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-140">Int64</span></span>   | <span data-ttu-id="bc625-141">O número de mensagens postadas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="bc625-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="bc625-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="bc625-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="bc625-143">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-143">Int64</span></span>   | <span data-ttu-id="bc625-144">O número de mensagens lidas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="bc625-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="bc625-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="bc625-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="bc625-146">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-146">Int64</span></span>   | <span data-ttu-id="bc625-147">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="bc625-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="bc625-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="bc625-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="bc625-149">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-149">Int64</span></span>   | <span data-ttu-id="bc625-150">O número de itens na caixa de correio do grupo.</span><span class="sxs-lookup"><span data-stu-id="bc625-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="bc625-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="bc625-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="bc625-152">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-152">Int64</span></span>   | <span data-ttu-id="bc625-153">O armazenamento usado da caixa de correio do grupo.</span><span class="sxs-lookup"><span data-stu-id="bc625-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="bc625-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="bc625-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="bc625-155">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-155">Int64</span></span>   | <span data-ttu-id="bc625-156">O número total de arquivos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bc625-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="bc625-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="bc625-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="bc625-158">Int64</span><span class="sxs-lookup"><span data-stu-id="bc625-158">Int64</span></span>   | <span data-ttu-id="bc625-159">O armazenamento usado pelo site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bc625-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="bc625-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bc625-160">reportPeriod</span></span>                      | <span data-ttu-id="bc625-161">String</span><span class="sxs-lookup"><span data-stu-id="bc625-161">String</span></span>  | <span data-ttu-id="bc625-162">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="bc625-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="bc625-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc625-163">JSON representation</span></span>

<span data-ttu-id="bc625-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc625-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```
