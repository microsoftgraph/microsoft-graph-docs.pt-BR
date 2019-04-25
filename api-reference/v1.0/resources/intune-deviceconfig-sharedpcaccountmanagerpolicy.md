---
title: Tipo de recurso sharedPCAccountManagerPolicy
description: Política do gerenciador de conta de PC compartilhado. Aplica-se somente quando o gerenciador de contas está habilitado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 683915fdf1a0878e72229ed98cca457fbf77082d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534609"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="b99b0-104">Tipo de recurso sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="b99b0-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="b99b0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b99b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b99b0-106">Política do gerenciador de conta de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="b99b0-106">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="b99b0-107">Aplica-se somente quando o gerenciador de contas está habilitado.</span><span class="sxs-lookup"><span data-stu-id="b99b0-107">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="b99b0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b99b0-108">Properties</span></span>
|<span data-ttu-id="b99b0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b99b0-109">Property</span></span>|<span data-ttu-id="b99b0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b99b0-110">Type</span></span>|<span data-ttu-id="b99b0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b99b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b99b0-112">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="b99b0-112">accountDeletionPolicy</span></span>|[<span data-ttu-id="b99b0-113">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="b99b0-113">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="b99b0-114">Configura quando as contas são excluídas.</span><span class="sxs-lookup"><span data-stu-id="b99b0-114">Configures when accounts are deleted.</span></span> <span data-ttu-id="b99b0-115">Os valores possíveis são: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="b99b0-115">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="b99b0-116">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="b99b0-116">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="b99b0-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b99b0-117">Int32</span></span>|<span data-ttu-id="b99b0-118">Define a porcentagem de espaço em disco disponível que um computador deve ter antes de parar de excluir contas do computador compartilhadas em cache.</span><span class="sxs-lookup"><span data-stu-id="b99b0-118">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="b99b0-119">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="b99b0-119">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="b99b0-120">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="b99b0-120">Valid values 0 to 100</span></span>|
|<span data-ttu-id="b99b0-121">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="b99b0-121">inactiveThresholdDays</span></span>|<span data-ttu-id="b99b0-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b99b0-122">Int32</span></span>|<span data-ttu-id="b99b0-123">Especifica quando as contas começarão a ser excluídas quando não forem conectadas durante o período especificado, fornecido como um número de dias.</span><span class="sxs-lookup"><span data-stu-id="b99b0-123">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="b99b0-124">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="b99b0-124">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="b99b0-125">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="b99b0-125">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="b99b0-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b99b0-126">Int32</span></span>|<span data-ttu-id="b99b0-127">Define a porcentagem de espaço em disco restante em um computador antes que contas em cache sejam excluídas para liberar espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="b99b0-127">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="b99b0-128">Contas inativas há mais tempo serão excluídas primeiro.</span><span class="sxs-lookup"><span data-stu-id="b99b0-128">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="b99b0-129">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="b99b0-129">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="b99b0-130">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="b99b0-130">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="b99b0-131">Relações</span><span class="sxs-lookup"><span data-stu-id="b99b0-131">Relationships</span></span>
<span data-ttu-id="b99b0-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b99b0-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b99b0-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b99b0-133">JSON Representation</span></span>
<span data-ttu-id="b99b0-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b99b0-134">Here is a JSON representation of the resource.</span></span>
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



