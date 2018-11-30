---
title: Tipo de recurso sharedPCAccountManagerPolicy
description: Política do gerenciador de conta de PC compartilhado. Aplica-se somente quando o gerenciador de contas está habilitado.
ms.openlocfilehash: 87e0ec0b4a6fa38a7c4093cca2b4551a9607f448
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037315"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="f9e24-104">Tipo de recurso sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f9e24-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="f9e24-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9e24-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9e24-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9e24-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9e24-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f9e24-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9e24-108">Política do gerenciador de conta de PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f9e24-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="f9e24-109">Aplica-se somente quando o gerenciador de contas está habilitado.</span><span class="sxs-lookup"><span data-stu-id="f9e24-109">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="f9e24-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9e24-110">Properties</span></span>
|<span data-ttu-id="f9e24-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9e24-111">Property</span></span>|<span data-ttu-id="f9e24-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9e24-112">Type</span></span>|<span data-ttu-id="f9e24-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9e24-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9e24-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="f9e24-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="f9e24-115">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="f9e24-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="f9e24-116">Configura quando as contas são excluídas.</span><span class="sxs-lookup"><span data-stu-id="f9e24-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="f9e24-117">Os valores possíveis são: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="f9e24-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="f9e24-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="f9e24-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="f9e24-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f9e24-119">Int32</span></span>|<span data-ttu-id="f9e24-120">Define a porcentagem de espaço em disco disponível que um computador deve ter antes de parar de excluir contas do computador compartilhadas em cache.</span><span class="sxs-lookup"><span data-stu-id="f9e24-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="f9e24-121">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="f9e24-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="f9e24-122">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="f9e24-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="f9e24-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="f9e24-123">inactiveThresholdDays</span></span>|<span data-ttu-id="f9e24-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f9e24-124">Int32</span></span>|<span data-ttu-id="f9e24-125">Especifica quando as contas começarão a ser excluídas quando não forem conectadas durante o período especificado, fornecido como um número de dias.</span><span class="sxs-lookup"><span data-stu-id="f9e24-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="f9e24-126">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="f9e24-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="f9e24-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="f9e24-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="f9e24-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f9e24-128">Int32</span></span>|<span data-ttu-id="f9e24-129">Define a porcentagem de espaço em disco restante em um computador antes que contas em cache sejam excluídas para liberar espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="f9e24-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="f9e24-130">Contas inativas há mais tempo serão excluídas primeiro.</span><span class="sxs-lookup"><span data-stu-id="f9e24-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="f9e24-131">Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="f9e24-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="f9e24-132">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="f9e24-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9e24-133">Relações</span><span class="sxs-lookup"><span data-stu-id="f9e24-133">Relationships</span></span>
<span data-ttu-id="f9e24-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9e24-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9e24-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9e24-135">JSON Representation</span></span>
<span data-ttu-id="f9e24-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9e24-136">Here is a JSON representation of the resource.</span></span>
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





