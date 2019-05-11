---
title: Tipo de recurso sharedPCAccountManagerPolicy
description: Política do gerenciador de conta de PC compartilhado. Aplica-se somente quando o gerenciador de contas está habilitado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f604df505bea11c59d1e0e3c0acdb5b638295449
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944716"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="6c762-104">Tipo de recurso sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="6c762-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="6c762-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c762-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c762-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c762-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c762-107">Política do gerenciador de conta de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="6c762-107">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="6c762-108">Aplica-se somente quando o gerenciador de contas está habilitado.</span><span class="sxs-lookup"><span data-stu-id="6c762-108">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="6c762-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c762-109">Properties</span></span>
|<span data-ttu-id="6c762-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c762-110">Property</span></span>|<span data-ttu-id="6c762-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c762-111">Type</span></span>|<span data-ttu-id="6c762-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c762-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c762-113">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="6c762-113">accountDeletionPolicy</span></span>|[<span data-ttu-id="6c762-114">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="6c762-114">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="6c762-115">Configura quando as contas são excluídas.</span><span class="sxs-lookup"><span data-stu-id="6c762-115">Configures when accounts are deleted.</span></span> <span data-ttu-id="6c762-116">Os valores possíveis são: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="6c762-116">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="6c762-117">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="6c762-117">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="6c762-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6c762-118">Int32</span></span>|<span data-ttu-id="6c762-119">Define a porcentagem de espaço em disco disponível que um computador deve ter antes de parar de excluir contas do computador compartilhadas em cache.</span><span class="sxs-lookup"><span data-stu-id="6c762-119">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="6c762-120">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="6c762-120">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="6c762-121">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="6c762-121">Valid values 0 to 100</span></span>|
|<span data-ttu-id="6c762-122">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="6c762-122">inactiveThresholdDays</span></span>|<span data-ttu-id="6c762-123">Int32</span><span class="sxs-lookup"><span data-stu-id="6c762-123">Int32</span></span>|<span data-ttu-id="6c762-124">Especifica quando as contas começarão a ser excluídas quando não forem conectadas durante o período especificado, fornecido como um número de dias.</span><span class="sxs-lookup"><span data-stu-id="6c762-124">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="6c762-125">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="6c762-125">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="6c762-126">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="6c762-126">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="6c762-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6c762-127">Int32</span></span>|<span data-ttu-id="6c762-128">Define a porcentagem de espaço em disco restante em um computador antes que contas em cache sejam excluídas para liberar espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="6c762-128">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="6c762-129">Contas inativas há mais tempo serão excluídas primeiro.</span><span class="sxs-lookup"><span data-stu-id="6c762-129">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="6c762-130">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="6c762-130">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="6c762-131">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="6c762-131">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c762-132">Relações</span><span class="sxs-lookup"><span data-stu-id="6c762-132">Relationships</span></span>
<span data-ttu-id="6c762-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c762-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c762-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c762-134">JSON Representation</span></span>
<span data-ttu-id="6c762-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c762-135">Here is a JSON representation of the resource.</span></span>
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




