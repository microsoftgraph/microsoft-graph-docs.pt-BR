---
title: Tipo de recurso sharedPCAccountManagerPolicy
description: Política do gerenciador de conta de PC compartilhado. Aplica-se somente quando o gerenciador de contas está habilitado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d548dd5f6df7a052ae08f580657fbbd16e48f50f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367978"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="1a643-104">Tipo de recurso sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="1a643-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="1a643-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a643-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a643-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a643-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a643-107">Política do gerenciador de conta de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1a643-107">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="1a643-108">Aplica-se somente quando o gerenciador de contas está habilitado.</span><span class="sxs-lookup"><span data-stu-id="1a643-108">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="1a643-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a643-109">Properties</span></span>
|<span data-ttu-id="1a643-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a643-110">Property</span></span>|<span data-ttu-id="1a643-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a643-111">Type</span></span>|<span data-ttu-id="1a643-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a643-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a643-113">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="1a643-113">accountDeletionPolicy</span></span>|[<span data-ttu-id="1a643-114">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="1a643-114">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="1a643-115">Configura quando as contas são excluídas.</span><span class="sxs-lookup"><span data-stu-id="1a643-115">Configures when accounts are deleted.</span></span> <span data-ttu-id="1a643-116">Os valores possíveis são: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="1a643-116">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="1a643-117">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="1a643-117">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="1a643-118">Int32</span><span class="sxs-lookup"><span data-stu-id="1a643-118">Int32</span></span>|<span data-ttu-id="1a643-119">Define a porcentagem de espaço em disco disponível que um computador deve ter antes de parar de excluir contas do computador compartilhadas em cache.</span><span class="sxs-lookup"><span data-stu-id="1a643-119">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="1a643-120">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="1a643-120">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="1a643-121">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="1a643-121">Valid values 0 to 100</span></span>|
|<span data-ttu-id="1a643-122">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="1a643-122">inactiveThresholdDays</span></span>|<span data-ttu-id="1a643-123">Int32</span><span class="sxs-lookup"><span data-stu-id="1a643-123">Int32</span></span>|<span data-ttu-id="1a643-124">Especifica quando as contas começarão a ser excluídas quando não forem conectadas durante o período especificado, fornecido como um número de dias.</span><span class="sxs-lookup"><span data-stu-id="1a643-124">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="1a643-125">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="1a643-125">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="1a643-126">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="1a643-126">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="1a643-127">Int32</span><span class="sxs-lookup"><span data-stu-id="1a643-127">Int32</span></span>|<span data-ttu-id="1a643-128">Define a porcentagem de espaço em disco restante em um computador antes que contas em cache sejam excluídas para liberar espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="1a643-128">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="1a643-129">Contas inativas há mais tempo serão excluídas primeiro.</span><span class="sxs-lookup"><span data-stu-id="1a643-129">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="1a643-130">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="1a643-130">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="1a643-131">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="1a643-131">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a643-132">Relações</span><span class="sxs-lookup"><span data-stu-id="1a643-132">Relationships</span></span>
<span data-ttu-id="1a643-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a643-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a643-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a643-134">JSON Representation</span></span>
<span data-ttu-id="1a643-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a643-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```



