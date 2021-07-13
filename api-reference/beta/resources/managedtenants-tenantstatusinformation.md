---
title: Tipo de recurso tenantStatusInformation
description: Representa informações de status de integração para um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3e01ac003cda223788e0fc8e6dae01f18667da11
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401991"
---
# <a name="tenantstatusinformation-resource-type"></a><span data-ttu-id="d8ad6-103">Tipo de recurso tenantStatusInformation</span><span class="sxs-lookup"><span data-stu-id="d8ad6-103">tenantStatusInformation resource type</span></span>

<span data-ttu-id="d8ad6-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="d8ad6-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8ad6-105">Representa informações de status de integração para um locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-105">Represents onboarding status information for a managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="d8ad6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8ad6-106">Properties</span></span>
|<span data-ttu-id="d8ad6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8ad6-107">Property</span></span>|<span data-ttu-id="d8ad6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8ad6-108">Type</span></span>|<span data-ttu-id="d8ad6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8ad6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8ad6-110">delegatedPrivilegeStatus</span><span class="sxs-lookup"><span data-stu-id="d8ad6-110">delegatedPrivilegeStatus</span></span>|<span data-ttu-id="d8ad6-111">delegatedPrivilegeStatus</span><span class="sxs-lookup"><span data-stu-id="d8ad6-111">delegatedPrivilegeStatus</span></span>|<span data-ttu-id="d8ad6-112">O status da relação de privilégio de administrador delegada entre a entidade de gerenciamento e o locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-112">The status of the delegated admin privilege relationship between the managing entity and the managed tenant.</span></span> <span data-ttu-id="d8ad6-113">Os valores possíveis são: `none`, `delegatedAdminPrivileges`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-113">Possible values are: `none`, `delegatedAdminPrivileges`, `unknownFutureValue`.</span></span> <span data-ttu-id="d8ad6-114">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-114">Optional.</span></span> <span data-ttu-id="d8ad6-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-115">Read-only.</span></span>|
|<span data-ttu-id="d8ad6-116">lastDelegatedPrivilegeRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="d8ad6-116">lastDelegatedPrivilegeRefreshDateTime</span></span>|<span data-ttu-id="d8ad6-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8ad6-117">DateTimeOffset</span></span>|<span data-ttu-id="d8ad6-118">A data e a hora em que o status dos privilégios de administrador delegado foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-118">The date and time the delegated admin privileges status was updated.</span></span> <span data-ttu-id="d8ad6-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-119">Optional.</span></span> <span data-ttu-id="d8ad6-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-120">Read-only.</span></span>|
|<span data-ttu-id="d8ad6-121">offboardedByUserId</span><span class="sxs-lookup"><span data-stu-id="d8ad6-121">offboardedByUserId</span></span>|<span data-ttu-id="d8ad6-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8ad6-122">String</span></span>|<span data-ttu-id="d8ad6-123">O identificador da conta que desarmou o locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-123">The identifier for the account that offboarded the managed tenant.</span></span> <span data-ttu-id="d8ad6-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-124">Optional.</span></span> <span data-ttu-id="d8ad6-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-125">Read-only.</span></span>|
|<span data-ttu-id="d8ad6-126">offboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8ad6-126">offboardedDateTime</span></span>|<span data-ttu-id="d8ad6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8ad6-127">DateTimeOffset</span></span>|<span data-ttu-id="d8ad6-128">A data e a hora em que o locatário gerenciado foi desligado.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-128">The date and time when the managed tenant was offboarded.</span></span> <span data-ttu-id="d8ad6-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-129">Optional.</span></span> <span data-ttu-id="d8ad6-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-130">Read-only.</span></span>|
|<span data-ttu-id="d8ad6-131">onboardedByUserId</span><span class="sxs-lookup"><span data-stu-id="d8ad6-131">onboardedByUserId</span></span>|<span data-ttu-id="d8ad6-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8ad6-132">String</span></span>|<span data-ttu-id="d8ad6-133">O identificador da conta que integrava o locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-133">The identifier for the account that onboarded the managed tenant.</span></span> <span data-ttu-id="d8ad6-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-134">Optional.</span></span> <span data-ttu-id="d8ad6-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-135">Read-only.</span></span>|
|<span data-ttu-id="d8ad6-136">onboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8ad6-136">onboardedDateTime</span></span>|<span data-ttu-id="d8ad6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8ad6-137">DateTimeOffset</span></span>|<span data-ttu-id="d8ad6-138">A data e a hora em que o locatário gerenciado foi internado.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-138">The date and time when the managed tenant was onboarded.</span></span> <span data-ttu-id="d8ad6-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-139">Optional.</span></span> <span data-ttu-id="d8ad6-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-140">Read-only.</span></span>|
|<span data-ttu-id="d8ad6-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="d8ad6-141">onboardingStatus</span></span>|<span data-ttu-id="d8ad6-142">tenantOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="d8ad6-142">tenantOnboardingStatus</span></span>|<span data-ttu-id="d8ad6-143">O status de integração do locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-143">The onboarding status for the managed tenant..</span></span> <span data-ttu-id="d8ad6-144">Os valores possíveis são: `ineligible`, `inProcess`, `active`, `inactive`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-144">Possible values are: `ineligible`, `inProcess`, `active`, `inactive`, `unknownFutureValue`.</span></span> <span data-ttu-id="d8ad6-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-145">Optional.</span></span> <span data-ttu-id="d8ad6-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-146">Read-only.</span></span>|
|<span data-ttu-id="d8ad6-147">workloadStatuses</span><span class="sxs-lookup"><span data-stu-id="d8ad6-147">workloadStatuses</span></span>|<span data-ttu-id="d8ad6-148">[coleção microsoft.graph.managedTenants.workloadStatus](../resources/managedtenants-workloadstatus.md)</span><span class="sxs-lookup"><span data-stu-id="d8ad6-148">[microsoft.graph.managedTenants.workloadStatus](../resources/managedtenants-workloadstatus.md) collection</span></span>|<span data-ttu-id="d8ad6-149">A coleção de estatuetas de carga de trabalho para o locatário gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-149">The collection of workload statues for the managed tenant.</span></span> <span data-ttu-id="d8ad6-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-150">Optional.</span></span> <span data-ttu-id="d8ad6-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8ad6-152">Relações</span><span class="sxs-lookup"><span data-stu-id="d8ad6-152">Relationships</span></span>
<span data-ttu-id="d8ad6-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8ad6-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8ad6-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8ad6-154">JSON representation</span></span>
<span data-ttu-id="d8ad6-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8ad6-155">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantStatusInformation",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "onboardedByUserId": "String",
  "offboardedDateTime": "String (timestamp)",
  "offboardedByUserId": "String",
  "delegatedPrivilegeStatus": "String",
  "lastDelegatedPrivilegeRefreshDateTime": "String (timestamp)",
  "workloadStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
    }
  ]
}
```
