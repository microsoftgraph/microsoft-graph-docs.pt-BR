---
title: tipo de recurso educationSynchronizationProfile
description: Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD). Este recurso fornece uma representação programática usada no School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 05babeebb25130350e64d98ccfc408381547829e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790912"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="c6161-104">tipo de recurso educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="c6161-104">educationSynchronizationProfile resource type</span></span>

<span data-ttu-id="c6161-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6161-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6161-106">Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c6161-106">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="c6161-107">Este recurso fornece uma representação programática usada no [School Data Sync](https://sds.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="c6161-107">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="c6161-108">Methods</span><span class="sxs-lookup"><span data-stu-id="c6161-108">Methods</span></span>

| <span data-ttu-id="c6161-109">Método</span><span class="sxs-lookup"><span data-stu-id="c6161-109">Method</span></span>                                                                    | <span data-ttu-id="c6161-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c6161-110">Return Type</span></span>                                                 | <span data-ttu-id="c6161-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6161-111">Description</span></span>                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="c6161-112">Listar perfis</span><span class="sxs-lookup"><span data-stu-id="c6161-112">List profiles</span></span>](../api/educationsynchronizationprofile-list.md)           | <span data-ttu-id="c6161-113">coleção [educationSynchronizationProfile]</span><span class="sxs-lookup"><span data-stu-id="c6161-113">[educationSynchronizationProfile] collection</span></span>                | <span data-ttu-id="c6161-114">Obtenha uma lista de todos os perfis de sincronização no locatário.</span><span class="sxs-lookup"><span data-stu-id="c6161-114">Get a list of all the synchronization profiles in the tenant.</span></span>                                                                  |
| [<span data-ttu-id="c6161-115">Obter perfil</span><span class="sxs-lookup"><span data-stu-id="c6161-115">Get profile</span></span>](../api/educationsynchronizationprofile-get.md)              | <span data-ttu-id="c6161-116">[educationSynchronizationProfile]</span><span class="sxs-lookup"><span data-stu-id="c6161-116">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="c6161-117">Recupere um perfil específico dado o identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="c6161-117">Retrieve a specific profile given the profile identifier.</span></span>                                                                      |
| [<span data-ttu-id="c6161-118">Criar perfil</span><span class="sxs-lookup"><span data-stu-id="c6161-118">Create profile</span></span>](../api/educationsynchronizationprofile-post.md)          | <span data-ttu-id="c6161-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c6161-119">None</span></span>                                                        | <span data-ttu-id="c6161-120">Criar um novo perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c6161-120">Create a new synchronization profile.</span></span>                                                                                          |
| [<span data-ttu-id="c6161-121">Excluir perfil</span><span class="sxs-lookup"><span data-stu-id="c6161-121">Delete profile</span></span>](../api/educationsynchronizationprofile-delete.md)        | <span data-ttu-id="c6161-122">[educationSynchronizationProfile]</span><span class="sxs-lookup"><span data-stu-id="c6161-122">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="c6161-123">Excluir um perfil específico dado o identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="c6161-123">Delete a specific profile given the profile identifier.</span></span>                                                                        |
| [<span data-ttu-id="c6161-124">Pausar perfil</span><span class="sxs-lookup"><span data-stu-id="c6161-124">Pause profile</span></span>](../api/educationsynchronizationprofile-pause.md)          | <span data-ttu-id="c6161-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c6161-125">None</span></span>                                                        | <span data-ttu-id="c6161-126">Pausar uma sincronização em andamento.</span><span class="sxs-lookup"><span data-stu-id="c6161-126">Pause an ongoing synchronization.</span></span>                                                                                              |
| [<span data-ttu-id="c6161-127">Retomar perfil</span><span class="sxs-lookup"><span data-stu-id="c6161-127">Resume profile</span></span>](../api/educationsynchronizationprofile-resume.md)        | <span data-ttu-id="c6161-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c6161-128">None</span></span>                                                        | <span data-ttu-id="c6161-129">Retomar uma sincronização pausada.</span><span class="sxs-lookup"><span data-stu-id="c6161-129">Resume a paused synchronization.</span></span>                                                                                               |
| [<span data-ttu-id="c6161-130">Redefinir perfil</span><span class="sxs-lookup"><span data-stu-id="c6161-130">Reset profile</span></span>](../api/educationsynchronizationprofile-reset.md)          | <span data-ttu-id="c6161-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c6161-131">None</span></span>                                                        | <span data-ttu-id="c6161-132">Redefina o estado do perfil e reinicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="c6161-132">Reset the state of the profile and restart synchronization.</span></span>                                                                    |
| [<span data-ttu-id="c6161-133">Iniciar perfil CSV</span><span class="sxs-lookup"><span data-stu-id="c6161-133">Start CSV profile</span></span>](../api/educationsynchronizationprofile-start.md)      | <span data-ttu-id="c6161-134">coleção [educationFileSynchronizationVerificationMessage]</span><span class="sxs-lookup"><span data-stu-id="c6161-134">[educationFileSynchronizationVerificationMessage]collection</span></span> | <span data-ttu-id="c6161-135">Verifique os arquivos de origem carregados e inicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="c6161-135">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="c6161-136">Aplica-se somente quando o provedor de dados é [educationCsvDataProvider].</span><span class="sxs-lookup"><span data-stu-id="c6161-136">Applies only when the data provider is [educationCsvDataProvider].</span></span> |
| [<span data-ttu-id="c6161-137">Obter URL de upload de CSV</span><span class="sxs-lookup"><span data-stu-id="c6161-137">Get CSV upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="c6161-138">string</span><span class="sxs-lookup"><span data-stu-id="c6161-138">string</span></span>                                                      | <span data-ttu-id="c6161-139">Retornar a URL de curta duração para carregar arquivos de dados CSV.</span><span class="sxs-lookup"><span data-stu-id="c6161-139">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="c6161-140">Aplica-se somente quando o provedor de dados é [educationCsvDataProvider].</span><span class="sxs-lookup"><span data-stu-id="c6161-140">Applies only when the data provider is [educationCsvDataProvider].</span></span>        |
| [<span data-ttu-id="c6161-141">Obter status</span><span class="sxs-lookup"><span data-stu-id="c6161-141">Get status</span></span>](../api/educationsynchronizationprofilestatus-get.md)         | <span data-ttu-id="c6161-142">[educationsynchronizationProfileStatus]</span><span class="sxs-lookup"><span data-stu-id="c6161-142">[educationsynchronizationProfileStatus]</span></span>                     | <span data-ttu-id="c6161-143">Retornar o status de um perfil de sincronização específico.</span><span class="sxs-lookup"><span data-stu-id="c6161-143">Return the status of a specific synchronization profile.</span></span>                                                                       |
| [<span data-ttu-id="c6161-144">Obter erros</span><span class="sxs-lookup"><span data-stu-id="c6161-144">Get errors</span></span>](../api/educationsynchronizationerrors-get.md)                | <span data-ttu-id="c6161-145">coleção [educationSynchronizationError]</span><span class="sxs-lookup"><span data-stu-id="c6161-145">[educationSynchronizationError] collection</span></span>                  | <span data-ttu-id="c6161-146">Obtenha todos os erros gerados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="c6161-146">Get all the errors generated during synchronization.</span></span>                                                                           |

## <a name="properties"></a><span data-ttu-id="c6161-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6161-147">Properties</span></span>

| <span data-ttu-id="c6161-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6161-148">Property</span></span>                             | <span data-ttu-id="c6161-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6161-149">Type</span></span>                                                   | <span data-ttu-id="c6161-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6161-150">Description</span></span>                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c6161-151">displayName</span><span class="sxs-lookup"><span data-stu-id="c6161-151">displayName</span></span>                          | <span data-ttu-id="c6161-152">string</span><span class="sxs-lookup"><span data-stu-id="c6161-152">string</span></span>                                                 | <span data-ttu-id="c6161-153">Nome do perfil de configuração para sincronizar identidades.</span><span class="sxs-lookup"><span data-stu-id="c6161-153">Name of the configuration profile for syncing identities.</span></span>                                                                         |
| <span data-ttu-id="c6161-154">DataProvider</span><span class="sxs-lookup"><span data-stu-id="c6161-154">dataProvider</span></span>                         | <span data-ttu-id="c6161-155">[educationSynchronizationDataProvider]</span><span class="sxs-lookup"><span data-stu-id="c6161-155">[educationSynchronizationDataProvider]</span></span>                 | <span data-ttu-id="c6161-156">O provedor de dados usado para o perfil.</span><span class="sxs-lookup"><span data-stu-id="c6161-156">The data provider used for the profile.</span></span>                                                                                           |
| <span data-ttu-id="c6161-157">identitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="c6161-157">identitySynchronizationConfiguration</span></span> | <span data-ttu-id="c6161-158">[educationIdentitySynchronizationConfiguration]</span><span class="sxs-lookup"><span data-stu-id="c6161-158">[educationIdentitySynchronizationConfiguration]</span></span>        | <span data-ttu-id="c6161-159">Determina como o perfil deve [criar usuários novos][fullsync] ou [correspondentes existentes][dirsync] do AAD.</span><span class="sxs-lookup"><span data-stu-id="c6161-159">Determines how the Profile should [create new][fullsync] or [match existing][dirsync] AAD Users.</span></span>                                  |
| <span data-ttu-id="c6161-160">licensesToAssign</span><span class="sxs-lookup"><span data-stu-id="c6161-160">licensesToAssign</span></span>                     | <span data-ttu-id="c6161-161">coleção [educationSynchronizationLicenseAssignment]</span><span class="sxs-lookup"><span data-stu-id="c6161-161">[educationSynchronizationLicenseAssignment] collection</span></span> | <span data-ttu-id="c6161-162">Configuração da instalação da licença.</span><span class="sxs-lookup"><span data-stu-id="c6161-162">License setup configuration.</span></span>                                                                                                      |
| <span data-ttu-id="c6161-163">state</span><span class="sxs-lookup"><span data-stu-id="c6161-163">state</span></span>                                | <span data-ttu-id="c6161-164">educationSynchronizationProfileState</span><span class="sxs-lookup"><span data-stu-id="c6161-164">educationSynchronizationProfileState</span></span>                   | <span data-ttu-id="c6161-165">O estado do perfil.</span><span class="sxs-lookup"><span data-stu-id="c6161-165">The state of the profile.</span></span> <span data-ttu-id="c6161-166">Os valores possíveis são: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span><span class="sxs-lookup"><span data-stu-id="c6161-166">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c6161-167">Relações</span><span class="sxs-lookup"><span data-stu-id="c6161-167">Relationships</span></span>

| <span data-ttu-id="c6161-168">Relação</span><span class="sxs-lookup"><span data-stu-id="c6161-168">Relationship</span></span>  | <span data-ttu-id="c6161-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6161-169">Type</span></span>                                       | <span data-ttu-id="c6161-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6161-170">Description</span></span>                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| <span data-ttu-id="c6161-171">erros</span><span class="sxs-lookup"><span data-stu-id="c6161-171">errors</span></span>        | <span data-ttu-id="c6161-172">coleção [educationSynchronizationError]</span><span class="sxs-lookup"><span data-stu-id="c6161-172">[educationSynchronizationError] collection</span></span> | <span data-ttu-id="c6161-173">Todos os erros associados a este perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c6161-173">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="c6161-174">profileStatus</span><span class="sxs-lookup"><span data-stu-id="c6161-174">profileStatus</span></span> | <span data-ttu-id="c6161-175">[educationSynchronizationProfileStatus]</span><span class="sxs-lookup"><span data-stu-id="c6161-175">[educationSynchronizationProfileStatus]</span></span>    | <span data-ttu-id="c6161-176">O status da sincronização.</span><span class="sxs-lookup"><span data-stu-id="c6161-176">The synchronization status.</span></span>                              |

## <a name="data-providers"></a><span data-ttu-id="c6161-177">Provedores de dados</span><span class="sxs-lookup"><span data-stu-id="c6161-177">Data Providers</span></span>

<span data-ttu-id="c6161-178">Cada [educationSynchronizationProfile] deve especificar um dos provedores de dados a seguir para usar como a fonte de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c6161-178">Each [educationSynchronizationProfile] must specify one of the follow data providers to use as the synchronization source.</span></span>

| <span data-ttu-id="c6161-179">Data Provider</span><span class="sxs-lookup"><span data-stu-id="c6161-179">Data Provider</span></span>                       | <span data-ttu-id="c6161-180">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6161-180">Description</span></span>                                                                                        |
| :---------------------------------- | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c6161-181">[educationCsvDataProvider]</span><span class="sxs-lookup"><span data-stu-id="c6161-181">[educationCsvDataProvider]</span></span>          | <span data-ttu-id="c6161-182">Arquivos CSV carregados para a [URL SAS](../api/educationsynchronizationprofile-uploadurl.md) do perfil</span><span class="sxs-lookup"><span data-stu-id="c6161-182">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="c6161-183">educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="c6161-183">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="c6161-184">API do OneRoster v 1.1</span><span class="sxs-lookup"><span data-stu-id="c6161-184">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="c6161-185">[educationPowerSchoolDataProvider]</span><span class="sxs-lookup"><span data-stu-id="c6161-185">[educationPowerSchoolDataProvider]</span></span>  | <span data-ttu-id="c6161-186">API da PowerSchool</span><span class="sxs-lookup"><span data-stu-id="c6161-186">PowerSchool API</span></span>                                                                                    |

## <a name="json-representation"></a><span data-ttu-id="c6161-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6161-187">JSON representation</span></span>

<span data-ttu-id="c6161-188">Veja a seguir uma representação JSON do recurso **educationSynchronizationProfile** .</span><span class="sxs-lookup"><span data-stu-id="c6161-188">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

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
  "state": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileState"
  },
  "profileStatus": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
  },
  "errors": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
    }
  ],
  "dataProvider": {
    "@odata.type": "microsoft.graph.educationCsvDataProvider"
  },
  "identitySynchronizationConfiguration": {
    "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
  },
  "licensesToAssign": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
    }
  ],
  "handleSpecialCharacterConstraint": "Boolean"
}
```

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationsynchronizationprofilestatus]: educationsynchronizationProfileStatus.md
[educationsynchronizationerror]: educationSynchronizationError.md
[educationfilesynchronizationverificationmessage]: educationFileSynchronizationVerificationMessage.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationidentitysynchronizationconfiguration]: educationIdentitySynchronizationConfiguration.md
[educationsynchronizationlicenseassignment]: educationSynchronizationLicenseAssignment.md
[fullsync]: educationidentitycreationconfiguration.md
[dirsync]: educationidentitycreationconfiguration.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md

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
