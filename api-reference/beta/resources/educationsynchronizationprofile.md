---
title: tipo de recurso educationSynchronizationProfile
description: Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD). Este recurso fornece uma representação programática usada no School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c498abb711a336f3627ef0b63e6c742e633ea05a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289932"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="5d433-104">tipo de recurso educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="5d433-104">educationSynchronizationProfile resource type</span></span>

<span data-ttu-id="5d433-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d433-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d433-106">Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="5d433-106">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="5d433-107">Este recurso fornece uma representação programática usada no [School Data Sync](https://sds.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="5d433-107">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="5d433-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5d433-108">Methods</span></span>

| <span data-ttu-id="5d433-109">Método</span><span class="sxs-lookup"><span data-stu-id="5d433-109">Method</span></span> | <span data-ttu-id="5d433-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5d433-110">Return Type</span></span> | <span data-ttu-id="5d433-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d433-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="5d433-112">Listar perfis de sincronização</span><span class="sxs-lookup"><span data-stu-id="5d433-112">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md) | <span data-ttu-id="5d433-113">coleção **educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="5d433-113">**educationSynchronizationProfile** collection</span></span> | <span data-ttu-id="5d433-114">Obtenha uma lista de todos os perfis de sincronização no locatário.</span><span class="sxs-lookup"><span data-stu-id="5d433-114">Get a list of all the synchronization profiles in the tenant.</span></span> |
| [<span data-ttu-id="5d433-115">Obter perfil de sincronização</span><span class="sxs-lookup"><span data-stu-id="5d433-115">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md) | <span data-ttu-id="5d433-116">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="5d433-116">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="5d433-117">Recupere um perfil específico dado o identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="5d433-117">Retrieve a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="5d433-118">Criar perfil de sincronização</span><span class="sxs-lookup"><span data-stu-id="5d433-118">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md) | <span data-ttu-id="5d433-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d433-119">None</span></span> | <span data-ttu-id="5d433-120">Criar um novo perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="5d433-120">Create a new synchronization profile.</span></span> |
| [<span data-ttu-id="5d433-121">Excluir perfil de sincronização</span><span class="sxs-lookup"><span data-stu-id="5d433-121">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md) | <span data-ttu-id="5d433-122">**educationSynchronizationProfile**</span><span class="sxs-lookup"><span data-stu-id="5d433-122">**educationSynchronizationProfile**</span></span> | <span data-ttu-id="5d433-123">Excluir um perfil específico dado o identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="5d433-123">Delete a specific profile given the profile identifier.</span></span> |
| [<span data-ttu-id="5d433-124">Pausar uma sincronização contínua</span><span class="sxs-lookup"><span data-stu-id="5d433-124">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md) | <span data-ttu-id="5d433-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d433-125">None</span></span> | <span data-ttu-id="5d433-126">Pausar uma sincronização em andamento.</span><span class="sxs-lookup"><span data-stu-id="5d433-126">Pause an ongoing synchronization.</span></span> |
| [<span data-ttu-id="5d433-127">Retomar uma sincronização pausada</span><span class="sxs-lookup"><span data-stu-id="5d433-127">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md) | <span data-ttu-id="5d433-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d433-128">None</span></span> | <span data-ttu-id="5d433-129">Retomar uma sincronização pausada.</span><span class="sxs-lookup"><span data-stu-id="5d433-129">Resume a paused synchronization.</span></span> |
| [<span data-ttu-id="5d433-130">Redefinir uma sincronização</span><span class="sxs-lookup"><span data-stu-id="5d433-130">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md) | <span data-ttu-id="5d433-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d433-131">None</span></span> | <span data-ttu-id="5d433-132">Redefina o estado do perfil e reinicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="5d433-132">Reset the state of the profile and restart synchronization.</span></span> |
| [<span data-ttu-id="5d433-133">Iniciar a sincronização de arquivos carregados</span><span class="sxs-lookup"><span data-stu-id="5d433-133">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) | <span data-ttu-id="5d433-134">coleção [educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)</span><span class="sxs-lookup"><span data-stu-id="5d433-134">[educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md) collection</span></span>| <span data-ttu-id="5d433-135">Verifique os arquivos de origem carregados e inicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="5d433-135">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="5d433-136">Aplica-se somente quando o provedor de dados é [educationCsvDataProvider](educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="5d433-136">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="5d433-137">Obter uma URL de upload</span><span class="sxs-lookup"><span data-stu-id="5d433-137">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="5d433-138">string</span><span class="sxs-lookup"><span data-stu-id="5d433-138">string</span></span> | <span data-ttu-id="5d433-139">Retornar a URL de curta duração para carregar arquivos de dados CSV.</span><span class="sxs-lookup"><span data-stu-id="5d433-139">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="5d433-140">Aplica-se somente quando o provedor de dados é [educationCsvDataProvider](educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="5d433-140">Applies only when the data provider is [educationCsvDataProvider](educationcsvdataprovider.md).</span></span> |
| [<span data-ttu-id="5d433-141">Obter o status de uma sincronização</span><span class="sxs-lookup"><span data-stu-id="5d433-141">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | [<span data-ttu-id="5d433-142">status</span><span class="sxs-lookup"><span data-stu-id="5d433-142">status</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="5d433-143">Retornar o status de um perfil de sincronização específico.</span><span class="sxs-lookup"><span data-stu-id="5d433-143">Return the status of a specific synchronization profile.</span></span> |
| [<span data-ttu-id="5d433-144">Obter erros de sincronização</span><span class="sxs-lookup"><span data-stu-id="5d433-144">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="5d433-145">coleção [educationSynchronizationError](educationsynchronizationerror.md)</span><span class="sxs-lookup"><span data-stu-id="5d433-145">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="5d433-146">Obtenha todos os erros gerados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="5d433-146">Get all the errors generated during synchronization.</span></span> |

## <a name="properties"></a><span data-ttu-id="5d433-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d433-147">Properties</span></span>

| <span data-ttu-id="5d433-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d433-148">Property</span></span> | <span data-ttu-id="5d433-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d433-149">Type</span></span> | <span data-ttu-id="5d433-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d433-150">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5d433-151">**displayName**</span><span class="sxs-lookup"><span data-stu-id="5d433-151">**displayName**</span></span> | <span data-ttu-id="5d433-152">string</span><span class="sxs-lookup"><span data-stu-id="5d433-152">string</span></span> |  <span data-ttu-id="5d433-153">Nome do perfil de configuração para sincronizar identidades.</span><span class="sxs-lookup"><span data-stu-id="5d433-153">Name of the configuration profile for syncing identities.</span></span>         |
| <span data-ttu-id="5d433-154">**DataProvider**</span><span class="sxs-lookup"><span data-stu-id="5d433-154">**dataProvider**</span></span> | [<span data-ttu-id="5d433-155">educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="5d433-155">educationSynchronizationDataProvider</span></span>](educationsynchronizationdataprovider.md) |  <span data-ttu-id="5d433-156">O provedor de dados usado para o perfil.</span><span class="sxs-lookup"><span data-stu-id="5d433-156">The data provider used for the profile.</span></span>         |
| <span data-ttu-id="5d433-157">**identitySynchronizationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="5d433-157">**identitySynchronizationConfiguration**</span></span> | [<span data-ttu-id="5d433-158">educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5d433-158">educationIdentitySynchronizationConfiguration</span></span>](educationidentitysynchronizationconfiguration.md) | <span data-ttu-id="5d433-159">[Criação](educationidentitycreationconfiguration.md) de identidade ou configuração de [correspondência](educationidentitymatchingconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5d433-159">Identity [creation](educationidentitycreationconfiguration.md) or [matching](educationidentitymatchingconfiguration.md) configuration .</span></span>        |
| <span data-ttu-id="5d433-160">**licensesToAssign**</span><span class="sxs-lookup"><span data-stu-id="5d433-160">**licensesToAssign**</span></span> | <span data-ttu-id="5d433-161">coleção [educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5d433-161">[educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md) collection</span></span>|  <span data-ttu-id="5d433-162">Configuração da instalação da licença.</span><span class="sxs-lookup"><span data-stu-id="5d433-162">License setup configuration.</span></span>        |
| <span data-ttu-id="5d433-163">**state**</span><span class="sxs-lookup"><span data-stu-id="5d433-163">**state**</span></span> | <span data-ttu-id="5d433-164">educationSynchronizationProfileState</span><span class="sxs-lookup"><span data-stu-id="5d433-164">educationSynchronizationProfileState</span></span> |  <span data-ttu-id="5d433-165">O estado do perfil.</span><span class="sxs-lookup"><span data-stu-id="5d433-165">The state of the profile.</span></span> <span data-ttu-id="5d433-166">Os valores possíveis são: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span><span class="sxs-lookup"><span data-stu-id="5d433-166">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span>          |

## <a name="relationships"></a><span data-ttu-id="5d433-167">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="5d433-167">Relationships</span></span>

| <span data-ttu-id="5d433-168">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d433-168">Property</span></span> | <span data-ttu-id="5d433-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d433-169">Type</span></span> | <span data-ttu-id="5d433-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d433-170">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5d433-171">**errors**</span><span class="sxs-lookup"><span data-stu-id="5d433-171">**errors**</span></span> | <span data-ttu-id="5d433-172">coleção [educationSynchronizationError](educationsynchronizationerror.md)</span><span class="sxs-lookup"><span data-stu-id="5d433-172">[educationSynchronizationError](educationsynchronizationerror.md) collection</span></span>| <span data-ttu-id="5d433-173">Todos os erros associados a este perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="5d433-173">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="5d433-174">**profileStatus**</span><span class="sxs-lookup"><span data-stu-id="5d433-174">**profileStatus**</span></span> | [<span data-ttu-id="5d433-175">educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="5d433-175">educationSynchronizationProfileStatus</span></span>](educationsynchronizationprofilestatus.md) | <span data-ttu-id="5d433-176">O status da sincronização.</span><span class="sxs-lookup"><span data-stu-id="5d433-176">The synchronization status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5d433-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d433-177">JSON representation</span></span>
<span data-ttu-id="5d433-178">Veja a seguir uma representação JSON do recurso **educationSynchronizationProfile** .</span><span class="sxs-lookup"><span data-stu-id="5d433-178">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
    "id": "String",
    "displayName": "String",
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSynchronizationProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationSynchronizationProfile/dataProvider:\r\n      Referenced type microsoft.graph.educationSynchronizationDataProvider is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->