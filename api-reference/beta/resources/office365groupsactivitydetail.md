---
title: tipo de recurso office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: dfc45c4973194d26c1830f8c36d3bf3b407d2e3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009500"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="48096-103">tipo de recurso office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="48096-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="48096-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48096-104">Properties</span></span>

| <span data-ttu-id="48096-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48096-105">Property</span></span>                          | <span data-ttu-id="48096-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="48096-106">Type</span></span>    | <span data-ttu-id="48096-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="48096-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="48096-108">groupId</span><span class="sxs-lookup"><span data-stu-id="48096-108">groupId</span></span>                           | <span data-ttu-id="48096-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48096-109">String</span></span>  | <span data-ttu-id="48096-110">A ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="48096-110">The group id.</span></span>          |
| <span data-ttu-id="48096-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="48096-111">reportRefreshDate</span></span>                 | <span data-ttu-id="48096-112">Data</span><span class="sxs-lookup"><span data-stu-id="48096-112">Date</span></span>    | <span data-ttu-id="48096-113">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="48096-113">The latest date of the content.</span></span>          |
| <span data-ttu-id="48096-114">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="48096-114">groupDisplayName</span></span>                  | <span data-ttu-id="48096-115">String</span><span class="sxs-lookup"><span data-stu-id="48096-115">String</span></span>  | <span data-ttu-id="48096-116">O nome de exibição do grupo.</span><span class="sxs-lookup"><span data-stu-id="48096-116">The display name of the group.</span></span>           |
| <span data-ttu-id="48096-117">isDeleted</span><span class="sxs-lookup"><span data-stu-id="48096-117">isDeleted</span></span>                         | <span data-ttu-id="48096-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="48096-118">Boolean</span></span> | <span data-ttu-id="48096-119">Se este usuário foi excluído ou excluído por software.</span><span class="sxs-lookup"><span data-stu-id="48096-119">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="48096-120">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="48096-120">ownerPrincipalName</span></span>                | <span data-ttu-id="48096-121">String</span><span class="sxs-lookup"><span data-stu-id="48096-121">String</span></span>  | <span data-ttu-id="48096-122">O nome principal do proprietário do grupo.</span><span class="sxs-lookup"><span data-stu-id="48096-122">The group owner principal name.</span></span>          |
| <span data-ttu-id="48096-123">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="48096-123">lastActivityDate</span></span>                  | <span data-ttu-id="48096-124">Data</span><span class="sxs-lookup"><span data-stu-id="48096-124">Date</span></span>    | <span data-ttu-id="48096-125">A data da última atividade dos seguintes cenários: caixa de correio de grupo recebidas emails; arquivos de usuário exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint; páginas do SharePoint exibidas pelo usuário; mensagens postadas, lidas ou curtidas pelo usuário em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="48096-125">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="48096-126">groupType</span><span class="sxs-lookup"><span data-stu-id="48096-126">groupType</span></span>                         | <span data-ttu-id="48096-127">String</span><span class="sxs-lookup"><span data-stu-id="48096-127">String</span></span>  | <span data-ttu-id="48096-128">O tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="48096-128">The group type.</span></span> <span data-ttu-id="48096-129">Os valores possíveis são: **Public** ou **Private**.</span><span class="sxs-lookup"><span data-stu-id="48096-129">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="48096-130">memberCount</span><span class="sxs-lookup"><span data-stu-id="48096-130">memberCount</span></span>                       | <span data-ttu-id="48096-131">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-131">Int64</span></span>   | <span data-ttu-id="48096-132">A contagem de membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="48096-132">The group member count.</span></span>                  |
| <span data-ttu-id="48096-133">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="48096-133">externalMemberCount</span></span>               | <span data-ttu-id="48096-134">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-134">Int64</span></span>   | <span data-ttu-id="48096-135">A contagem de membros externos de grupo.</span><span class="sxs-lookup"><span data-stu-id="48096-135">The group external member count.</span></span>         |
| <span data-ttu-id="48096-136">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="48096-136">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="48096-137">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-137">Int64</span></span>   | <span data-ttu-id="48096-138">O número de emails que a caixa de correio de grupo recebeu.</span><span class="sxs-lookup"><span data-stu-id="48096-138">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="48096-139">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="48096-139">sharePointActiveFileCount</span></span>         | <span data-ttu-id="48096-140">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-140">Int64</span></span>   | <span data-ttu-id="48096-141">O número de arquivos ativos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="48096-141">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="48096-142">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="48096-142">yammerPostedMessageCount</span></span>          | <span data-ttu-id="48096-143">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-143">Int64</span></span>   | <span data-ttu-id="48096-144">O número de mensagens postadas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="48096-144">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="48096-145">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="48096-145">yammerReadMessageCount</span></span>            | <span data-ttu-id="48096-146">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-146">Int64</span></span>   | <span data-ttu-id="48096-147">O número de mensagens lidas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="48096-147">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="48096-148">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="48096-148">yammerLikedMessageCount</span></span>           | <span data-ttu-id="48096-149">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-149">Int64</span></span>   | <span data-ttu-id="48096-150">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="48096-150">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="48096-151">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="48096-151">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="48096-152">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-152">Int64</span></span>   | <span data-ttu-id="48096-153">O número de itens na caixa de correio do grupo.</span><span class="sxs-lookup"><span data-stu-id="48096-153">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="48096-154">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="48096-154">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="48096-155">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-155">Int64</span></span>   | <span data-ttu-id="48096-156">O armazenamento usado da caixa de correio do grupo.</span><span class="sxs-lookup"><span data-stu-id="48096-156">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="48096-157">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="48096-157">sharePointTotalFileCount</span></span>          | <span data-ttu-id="48096-158">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-158">Int64</span></span>   | <span data-ttu-id="48096-159">O número total de arquivos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="48096-159">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="48096-160">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="48096-160">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="48096-161">Int64</span><span class="sxs-lookup"><span data-stu-id="48096-161">Int64</span></span>   | <span data-ttu-id="48096-162">O armazenamento usado pelo site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="48096-162">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="48096-163">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="48096-163">reportPeriod</span></span>                      | <span data-ttu-id="48096-164">String</span><span class="sxs-lookup"><span data-stu-id="48096-164">String</span></span>  | <span data-ttu-id="48096-165">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="48096-165">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="48096-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48096-166">JSON representation</span></span>

<span data-ttu-id="48096-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48096-167">The following is a JSON representation of the resource.</span></span>

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
