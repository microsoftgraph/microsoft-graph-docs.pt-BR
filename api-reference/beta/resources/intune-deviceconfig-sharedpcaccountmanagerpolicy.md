---
title: Tipo de recurso sharedPCAccountManagerPolicy
description: Política do gerenciador de conta de PC compartilhado. Aplica-se somente quando o gerenciador de contas está habilitado.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d6b7e0ab86af78380f85da8ec37c643e662838c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410991"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="b1cd2-104">Tipo de recurso sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="b1cd2-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="b1cd2-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b1cd2-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1cd2-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1cd2-108">Política do gerenciador de conta de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="b1cd2-109">Aplica-se somente quando o gerenciador de contas está habilitado.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-109">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="b1cd2-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1cd2-110">Properties</span></span>
|<span data-ttu-id="b1cd2-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1cd2-111">Property</span></span>|<span data-ttu-id="b1cd2-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1cd2-112">Type</span></span>|<span data-ttu-id="b1cd2-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1cd2-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1cd2-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="b1cd2-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="b1cd2-115">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="b1cd2-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="b1cd2-116">Configura quando as contas são excluídas.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="b1cd2-117">Os valores possíveis são: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="b1cd2-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="b1cd2-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="b1cd2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b1cd2-119">Int32</span></span>|<span data-ttu-id="b1cd2-120">Define a porcentagem de espaço em disco disponível que um computador deve ter antes de parar de excluir contas do computador compartilhadas em cache.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="b1cd2-121">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="b1cd2-122">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="b1cd2-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="b1cd2-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="b1cd2-123">inactiveThresholdDays</span></span>|<span data-ttu-id="b1cd2-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b1cd2-124">Int32</span></span>|<span data-ttu-id="b1cd2-125">Especifica quando as contas começarão a ser excluídas quando não forem conectadas durante o período especificado, fornecido como um número de dias.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="b1cd2-126">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="b1cd2-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="b1cd2-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="b1cd2-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b1cd2-128">Int32</span></span>|<span data-ttu-id="b1cd2-129">Define a porcentagem de espaço em disco restante em um computador antes que contas em cache sejam excluídas para liberar espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="b1cd2-130">Contas inativas há mais tempo serão excluídas primeiro.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="b1cd2-131">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="b1cd2-132">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="b1cd2-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1cd2-133">Relações</span><span class="sxs-lookup"><span data-stu-id="b1cd2-133">Relationships</span></span>
<span data-ttu-id="b1cd2-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1cd2-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1cd2-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1cd2-135">JSON Representation</span></span>
<span data-ttu-id="b1cd2-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1cd2-136">Here is a JSON representation of the resource.</span></span>
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




