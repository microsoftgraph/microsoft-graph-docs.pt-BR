---
title: Tipo de recurso sharedPCAccountManagerPolicy
description: Política do gerenciador de conta de PC compartilhado. Aplica-se somente quando o gerenciador de contas está habilitado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ec508868d09264d633d920aeb22dfbdf328daf6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529393"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="00bb1-104">Tipo de recurso sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="00bb1-104">sharedPCAccountManagerPolicy resource type</span></span>

<span data-ttu-id="00bb1-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="00bb1-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00bb1-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="00bb1-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00bb1-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00bb1-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00bb1-108">Política do gerenciador de conta de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="00bb1-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="00bb1-109">Aplica-se somente quando o gerenciador de contas está habilitado.</span><span class="sxs-lookup"><span data-stu-id="00bb1-109">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="00bb1-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00bb1-110">Properties</span></span>
|<span data-ttu-id="00bb1-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00bb1-111">Property</span></span>|<span data-ttu-id="00bb1-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="00bb1-112">Type</span></span>|<span data-ttu-id="00bb1-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="00bb1-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00bb1-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="00bb1-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="00bb1-115">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="00bb1-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="00bb1-116">Configura quando as contas são excluídas.</span><span class="sxs-lookup"><span data-stu-id="00bb1-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="00bb1-117">Os valores possíveis são: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="00bb1-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="00bb1-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="00bb1-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="00bb1-119">Int32</span><span class="sxs-lookup"><span data-stu-id="00bb1-119">Int32</span></span>|<span data-ttu-id="00bb1-120">Define a porcentagem de espaço em disco disponível que um computador deve ter antes de parar de excluir contas do computador compartilhadas em cache.</span><span class="sxs-lookup"><span data-stu-id="00bb1-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="00bb1-121">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="00bb1-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="00bb1-122">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="00bb1-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="00bb1-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="00bb1-123">inactiveThresholdDays</span></span>|<span data-ttu-id="00bb1-124">Int32</span><span class="sxs-lookup"><span data-stu-id="00bb1-124">Int32</span></span>|<span data-ttu-id="00bb1-125">Especifica quando as contas começarão a ser excluídas quando não forem conectadas durante o período especificado, fornecido como um número de dias.</span><span class="sxs-lookup"><span data-stu-id="00bb1-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="00bb1-126">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="00bb1-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="00bb1-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="00bb1-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="00bb1-128">Int32</span><span class="sxs-lookup"><span data-stu-id="00bb1-128">Int32</span></span>|<span data-ttu-id="00bb1-129">Define a porcentagem de espaço em disco restante em um computador antes que contas em cache sejam excluídas para liberar espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="00bb1-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="00bb1-130">Contas inativas há mais tempo serão excluídas primeiro.</span><span class="sxs-lookup"><span data-stu-id="00bb1-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="00bb1-131">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="00bb1-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="00bb1-132">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="00bb1-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="00bb1-133">Relações</span><span class="sxs-lookup"><span data-stu-id="00bb1-133">Relationships</span></span>
<span data-ttu-id="00bb1-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00bb1-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00bb1-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00bb1-135">JSON Representation</span></span>
<span data-ttu-id="00bb1-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00bb1-136">Here is a JSON representation of the resource.</span></span>
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



