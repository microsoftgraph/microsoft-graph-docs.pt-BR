---
title: tipo de recurso office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 176e960c7d9ae8dd1bc29600ad7b64e45e2940fa
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805211"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="4e472-103">tipo de recurso office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="4e472-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4e472-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e472-104">Properties</span></span>

| <span data-ttu-id="4e472-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e472-105">Property</span></span>                          | <span data-ttu-id="4e472-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e472-106">Type</span></span>    | <span data-ttu-id="4e472-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e472-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="4e472-108">groupId</span><span class="sxs-lookup"><span data-stu-id="4e472-108">groupId</span></span>                           | <span data-ttu-id="4e472-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e472-109">String</span></span>  | <span data-ttu-id="4e472-110">A ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="4e472-110">The group id.</span></span>          |
| <span data-ttu-id="4e472-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4e472-111">reportRefreshDate</span></span>                 | <span data-ttu-id="4e472-112">Data</span><span class="sxs-lookup"><span data-stu-id="4e472-112">Date</span></span>    | <span data-ttu-id="4e472-113">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4e472-113">The latest date of the content.</span></span>          |
| <span data-ttu-id="4e472-114">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="4e472-114">groupDisplayName</span></span>                  | <span data-ttu-id="4e472-115">String</span><span class="sxs-lookup"><span data-stu-id="4e472-115">String</span></span>  | <span data-ttu-id="4e472-116">O nome de exibição do grupo.</span><span class="sxs-lookup"><span data-stu-id="4e472-116">The display name of the group.</span></span>           |
| <span data-ttu-id="4e472-117">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4e472-117">isDeleted</span></span>                         | <span data-ttu-id="4e472-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e472-118">Boolean</span></span> | <span data-ttu-id="4e472-119">Se este usuário foi excluído ou excluído por software.</span><span class="sxs-lookup"><span data-stu-id="4e472-119">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="4e472-120">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4e472-120">ownerPrincipalName</span></span>                | <span data-ttu-id="4e472-121">String</span><span class="sxs-lookup"><span data-stu-id="4e472-121">String</span></span>  | <span data-ttu-id="4e472-122">O nome principal do proprietário do grupo.</span><span class="sxs-lookup"><span data-stu-id="4e472-122">The group owner principal name.</span></span>          |
| <span data-ttu-id="4e472-123">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="4e472-123">lastActivityDate</span></span>                  | <span data-ttu-id="4e472-124">Data</span><span class="sxs-lookup"><span data-stu-id="4e472-124">Date</span></span>    | <span data-ttu-id="4e472-125">A data da última atividade dos seguintes cenários: caixa de correio de grupo recebidas emails; arquivos de usuário exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint; páginas do SharePoint exibidas pelo usuário; mensagens postadas, lidas ou curtidas pelo usuário em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="4e472-125">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="4e472-126">groupType</span><span class="sxs-lookup"><span data-stu-id="4e472-126">groupType</span></span>                         | <span data-ttu-id="4e472-127">String</span><span class="sxs-lookup"><span data-stu-id="4e472-127">String</span></span>  | <span data-ttu-id="4e472-128">O tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="4e472-128">The group type.</span></span> <span data-ttu-id="4e472-129">Os valores possíveis são: **Public** ou **Private**.</span><span class="sxs-lookup"><span data-stu-id="4e472-129">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="4e472-130">memberCount</span><span class="sxs-lookup"><span data-stu-id="4e472-130">memberCount</span></span>                       | <span data-ttu-id="4e472-131">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-131">Int64</span></span>   | <span data-ttu-id="4e472-132">A contagem de membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="4e472-132">The group member count.</span></span>                  |
| <span data-ttu-id="4e472-133">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="4e472-133">externalMemberCount</span></span>               | <span data-ttu-id="4e472-134">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-134">Int64</span></span>   | <span data-ttu-id="4e472-135">A contagem de membros externos de grupo.</span><span class="sxs-lookup"><span data-stu-id="4e472-135">The group external member count.</span></span>         |
| <span data-ttu-id="4e472-136">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="4e472-136">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="4e472-137">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-137">Int64</span></span>   | <span data-ttu-id="4e472-138">O número de emails que a caixa de correio de grupo recebeu.</span><span class="sxs-lookup"><span data-stu-id="4e472-138">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="4e472-139">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="4e472-139">sharePointActiveFileCount</span></span>         | <span data-ttu-id="4e472-140">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-140">Int64</span></span>   | <span data-ttu-id="4e472-141">O número de arquivos ativos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4e472-141">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="4e472-142">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="4e472-142">yammerPostedMessageCount</span></span>          | <span data-ttu-id="4e472-143">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-143">Int64</span></span>   | <span data-ttu-id="4e472-144">O número de mensagens postadas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="4e472-144">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="4e472-145">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="4e472-145">yammerReadMessageCount</span></span>            | <span data-ttu-id="4e472-146">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-146">Int64</span></span>   | <span data-ttu-id="4e472-147">O número de mensagens lidas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="4e472-147">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="4e472-148">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="4e472-148">yammerLikedMessageCount</span></span>           | <span data-ttu-id="4e472-149">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-149">Int64</span></span>   | <span data-ttu-id="4e472-150">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="4e472-150">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="4e472-151">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="4e472-151">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="4e472-152">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-152">Int64</span></span>   | <span data-ttu-id="4e472-153">O número de itens na caixa de correio do grupo.</span><span class="sxs-lookup"><span data-stu-id="4e472-153">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="4e472-154">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="4e472-154">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="4e472-155">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-155">Int64</span></span>   | <span data-ttu-id="4e472-156">O armazenamento usado da caixa de correio do grupo.</span><span class="sxs-lookup"><span data-stu-id="4e472-156">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="4e472-157">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="4e472-157">sharePointTotalFileCount</span></span>          | <span data-ttu-id="4e472-158">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-158">Int64</span></span>   | <span data-ttu-id="4e472-159">O número total de arquivos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4e472-159">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="4e472-160">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="4e472-160">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="4e472-161">Int64</span><span class="sxs-lookup"><span data-stu-id="4e472-161">Int64</span></span>   | <span data-ttu-id="4e472-162">O armazenamento usado pelo site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4e472-162">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="4e472-163">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4e472-163">reportPeriod</span></span>                      | <span data-ttu-id="4e472-164">String</span><span class="sxs-lookup"><span data-stu-id="4e472-164">String</span></span>  | <span data-ttu-id="4e472-165">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="4e472-165">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="4e472-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e472-166">JSON representation</span></span>

<span data-ttu-id="4e472-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e472-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
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
