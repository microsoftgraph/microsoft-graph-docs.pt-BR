---
title: Tipo de recurso sharedPCAccountManagerPolicy
description: Política do gerenciador de conta de PC compartilhado. Aplica-se somente quando o gerenciador de contas está habilitado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c474f9ab64921e6027bacdf5c2405bf953535778
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724548"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="59e47-104">Tipo de recurso sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="59e47-104">sharedPCAccountManagerPolicy resource type</span></span>

<span data-ttu-id="59e47-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59e47-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59e47-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59e47-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59e47-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59e47-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59e47-108">Política do gerenciador de conta de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="59e47-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="59e47-109">Aplica-se somente quando o gerenciador de contas está habilitado.</span><span class="sxs-lookup"><span data-stu-id="59e47-109">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="59e47-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59e47-110">Properties</span></span>
|<span data-ttu-id="59e47-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59e47-111">Property</span></span>|<span data-ttu-id="59e47-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="59e47-112">Type</span></span>|<span data-ttu-id="59e47-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="59e47-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59e47-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="59e47-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="59e47-115">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="59e47-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="59e47-116">Configura quando as contas são excluídas.</span><span class="sxs-lookup"><span data-stu-id="59e47-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="59e47-117">Os valores possíveis são: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="59e47-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="59e47-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="59e47-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="59e47-119">Int32</span><span class="sxs-lookup"><span data-stu-id="59e47-119">Int32</span></span>|<span data-ttu-id="59e47-120">Define a porcentagem de espaço em disco disponível que um computador deve ter antes de parar de excluir contas do computador compartilhadas em cache.</span><span class="sxs-lookup"><span data-stu-id="59e47-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="59e47-121">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="59e47-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="59e47-122">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="59e47-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="59e47-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="59e47-123">inactiveThresholdDays</span></span>|<span data-ttu-id="59e47-124">Int32</span><span class="sxs-lookup"><span data-stu-id="59e47-124">Int32</span></span>|<span data-ttu-id="59e47-125">Especifica quando as contas começarão a ser excluídas quando não forem conectadas durante o período especificado, fornecido como um número de dias.</span><span class="sxs-lookup"><span data-stu-id="59e47-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="59e47-126">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="59e47-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="59e47-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="59e47-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="59e47-128">Int32</span><span class="sxs-lookup"><span data-stu-id="59e47-128">Int32</span></span>|<span data-ttu-id="59e47-129">Define a porcentagem de espaço em disco restante em um computador antes que contas em cache sejam excluídas para liberar espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="59e47-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="59e47-130">Contas inativas há mais tempo serão excluídas primeiro.</span><span class="sxs-lookup"><span data-stu-id="59e47-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="59e47-131">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="59e47-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="59e47-132">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="59e47-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="59e47-133">Relações</span><span class="sxs-lookup"><span data-stu-id="59e47-133">Relationships</span></span>
<span data-ttu-id="59e47-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59e47-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59e47-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59e47-135">JSON Representation</span></span>
<span data-ttu-id="59e47-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59e47-136">Here is a JSON representation of the resource.</span></span>
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





