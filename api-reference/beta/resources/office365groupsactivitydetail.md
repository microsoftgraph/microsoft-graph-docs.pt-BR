---
title: tipo de recurso de office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2968a3a5459f286e4aac69e2fd606adc1b38e39b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951821"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="09690-103">tipo de recurso de office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="09690-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="09690-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09690-104">Properties</span></span>

| <span data-ttu-id="09690-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09690-105">Property</span></span>                          | <span data-ttu-id="09690-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="09690-106">Type</span></span>    | <span data-ttu-id="09690-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="09690-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="09690-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="09690-108">reportRefreshDate</span></span>                 | <span data-ttu-id="09690-109">Data</span><span class="sxs-lookup"><span data-stu-id="09690-109">Date</span></span>    | <span data-ttu-id="09690-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="09690-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="09690-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="09690-111">groupDisplayName</span></span>                  | <span data-ttu-id="09690-112">String</span><span class="sxs-lookup"><span data-stu-id="09690-112">String</span></span>  | <span data-ttu-id="09690-113">O nome de exibição do grupo.</span><span class="sxs-lookup"><span data-stu-id="09690-113">The display name of the group.</span></span>           |
| <span data-ttu-id="09690-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="09690-114">isDeleted</span></span>                         | <span data-ttu-id="09690-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="09690-115">Boolean</span></span> | <span data-ttu-id="09690-116">Se esse usuário tiver sido excluído ou suave excluído.</span><span class="sxs-lookup"><span data-stu-id="09690-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="09690-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="09690-117">ownerPrincipalName</span></span>                | <span data-ttu-id="09690-118">String</span><span class="sxs-lookup"><span data-stu-id="09690-118">String</span></span>  | <span data-ttu-id="09690-119">O nome de entidade do proprietário do grupo.</span><span class="sxs-lookup"><span data-stu-id="09690-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="09690-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="09690-120">lastActivityDate</span></span>                  | <span data-ttu-id="09690-121">Data</span><span class="sxs-lookup"><span data-stu-id="09690-121">Date</span></span>    | <span data-ttu-id="09690-122">A data da última atividade para os seguintes cenários: email da caixa de correio recebida; de grupo usuário exibido, editado, compartilhados ou sincronizados arquivos na biblioteca de documentos do SharePoint; usuário exibir páginas do SharePoint; usuário postados, ler ou curtidas mensagens no Yammer grupos.</span><span class="sxs-lookup"><span data-stu-id="09690-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="09690-123">groupType</span><span class="sxs-lookup"><span data-stu-id="09690-123">groupType</span></span>                         | <span data-ttu-id="09690-124">String</span><span class="sxs-lookup"><span data-stu-id="09690-124">String</span></span>  | <span data-ttu-id="09690-125">O tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="09690-125">The group type.</span></span> <span data-ttu-id="09690-126">Os valores possíveis são: **pública** ou **privada**.</span><span class="sxs-lookup"><span data-stu-id="09690-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="09690-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="09690-127">memberCount</span></span>                       | <span data-ttu-id="09690-128">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-128">Int64</span></span>   | <span data-ttu-id="09690-129">A contagem de membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="09690-129">The group member count.</span></span>                  |
| <span data-ttu-id="09690-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="09690-130">externalMemberCount</span></span>               | <span data-ttu-id="09690-131">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-131">Int64</span></span>   | <span data-ttu-id="09690-132">A contagem de externo membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="09690-132">The group external member count.</span></span>         |
| <span data-ttu-id="09690-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="09690-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="09690-134">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-134">Int64</span></span>   | <span data-ttu-id="09690-135">O número de email que recebeu a caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="09690-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="09690-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="09690-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="09690-137">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-137">Int64</span></span>   | <span data-ttu-id="09690-138">O número de arquivos ativos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="09690-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="09690-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="09690-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="09690-140">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-140">Int64</span></span>   | <span data-ttu-id="09690-141">O número de mensagens postadas em grupos de Yammer.</span><span class="sxs-lookup"><span data-stu-id="09690-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="09690-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="09690-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="09690-143">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-143">Int64</span></span>   | <span data-ttu-id="09690-144">O número de mensagens lidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="09690-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="09690-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="09690-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="09690-146">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-146">Int64</span></span>   | <span data-ttu-id="09690-147">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="09690-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="09690-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="09690-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="09690-149">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-149">Int64</span></span>   | <span data-ttu-id="09690-150">O número de itens na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="09690-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="09690-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="09690-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="09690-152">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-152">Int64</span></span>   | <span data-ttu-id="09690-153">O armazenamento utilizado da caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="09690-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="09690-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="09690-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="09690-155">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-155">Int64</span></span>   | <span data-ttu-id="09690-156">O número total de arquivos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="09690-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="09690-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="09690-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="09690-158">Int64</span><span class="sxs-lookup"><span data-stu-id="09690-158">Int64</span></span>   | <span data-ttu-id="09690-159">O armazenamento usado pelo site do grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="09690-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="09690-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="09690-160">reportPeriod</span></span>                      | <span data-ttu-id="09690-161">String</span><span class="sxs-lookup"><span data-stu-id="09690-161">String</span></span>  | <span data-ttu-id="09690-162">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="09690-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="09690-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09690-163">JSON representation</span></span>

<span data-ttu-id="09690-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09690-164">The following is a JSON representation of the resource.</span></span>

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
