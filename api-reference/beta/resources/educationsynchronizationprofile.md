---
title: tipo de recurso educationSynchronizationProfile
description: Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD). Este recurso fornece uma representação programática usada no School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2db53346ae270f5441637835ec5da0427d9d4ab8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989595"
---
# <a name="educationsynchronizationprofile-resource-type"></a><span data-ttu-id="e006a-104">tipo de recurso educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="e006a-104">educationSynchronizationProfile resource type</span></span>

<span data-ttu-id="e006a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e006a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e006a-106">Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e006a-106">Represents a set of configurations used to synchronize education entities and roster information from a source directory to Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="e006a-107">Este recurso fornece uma representação programática usada no [School Data Sync](https://sds.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="e006a-107">This resource provides a programmatic representation used in [School Data Sync](https://sds.microsoft.com).</span></span>

## <a name="methods"></a><span data-ttu-id="e006a-108">Methods</span><span class="sxs-lookup"><span data-stu-id="e006a-108">Methods</span></span>

| <span data-ttu-id="e006a-109">Método</span><span class="sxs-lookup"><span data-stu-id="e006a-109">Method</span></span>                                                                    | <span data-ttu-id="e006a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e006a-110">Return Type</span></span>                                                 | <span data-ttu-id="e006a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e006a-111">Description</span></span>                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="e006a-112">Listar perfis</span><span class="sxs-lookup"><span data-stu-id="e006a-112">List profiles</span></span>](../api/educationsynchronizationprofile-list.md)           | <span data-ttu-id="e006a-113">coleção [educationSynchronizationProfile]</span><span class="sxs-lookup"><span data-stu-id="e006a-113">[educationSynchronizationProfile] collection</span></span>                | <span data-ttu-id="e006a-114">Obtenha uma lista de todos os perfis de sincronização no locatário.</span><span class="sxs-lookup"><span data-stu-id="e006a-114">Get a list of all the synchronization profiles in the tenant.</span></span>                                                                  |
| [<span data-ttu-id="e006a-115">Obter perfil</span><span class="sxs-lookup"><span data-stu-id="e006a-115">Get profile</span></span>](../api/educationsynchronizationprofile-get.md)              | <span data-ttu-id="e006a-116">[educationSynchronizationProfile]</span><span class="sxs-lookup"><span data-stu-id="e006a-116">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="e006a-117">Recupere um perfil específico dado o identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="e006a-117">Retrieve a specific profile given the profile identifier.</span></span>                                                                      |
| [<span data-ttu-id="e006a-118">Criar perfil</span><span class="sxs-lookup"><span data-stu-id="e006a-118">Create profile</span></span>](../api/educationsynchronizationprofile-post.md)          | <span data-ttu-id="e006a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e006a-119">None</span></span>                                                        | <span data-ttu-id="e006a-120">Criar um novo perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="e006a-120">Create a new synchronization profile.</span></span>                                                                                          |
| [<span data-ttu-id="e006a-121">Excluir perfil</span><span class="sxs-lookup"><span data-stu-id="e006a-121">Delete profile</span></span>](../api/educationsynchronizationprofile-delete.md)        | <span data-ttu-id="e006a-122">[educationSynchronizationProfile]</span><span class="sxs-lookup"><span data-stu-id="e006a-122">[educationSynchronizationProfile]</span></span>                           | <span data-ttu-id="e006a-123">Excluir um perfil específico dado o identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="e006a-123">Delete a specific profile given the profile identifier.</span></span>                                                                        |
| [<span data-ttu-id="e006a-124">Pausar perfil</span><span class="sxs-lookup"><span data-stu-id="e006a-124">Pause profile</span></span>](../api/educationsynchronizationprofile-pause.md)          | <span data-ttu-id="e006a-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e006a-125">None</span></span>                                                        | <span data-ttu-id="e006a-126">Pausar uma sincronização em andamento.</span><span class="sxs-lookup"><span data-stu-id="e006a-126">Pause an ongoing synchronization.</span></span>                                                                                              |
| [<span data-ttu-id="e006a-127">Retomar perfil</span><span class="sxs-lookup"><span data-stu-id="e006a-127">Resume profile</span></span>](../api/educationsynchronizationprofile-resume.md)        | <span data-ttu-id="e006a-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e006a-128">None</span></span>                                                        | <span data-ttu-id="e006a-129">Retomar uma sincronização pausada.</span><span class="sxs-lookup"><span data-stu-id="e006a-129">Resume a paused synchronization.</span></span>                                                                                               |
| [<span data-ttu-id="e006a-130">Redefinir perfil</span><span class="sxs-lookup"><span data-stu-id="e006a-130">Reset profile</span></span>](../api/educationsynchronizationprofile-reset.md)          | <span data-ttu-id="e006a-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e006a-131">None</span></span>                                                        | <span data-ttu-id="e006a-132">Redefina o estado do perfil e reinicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="e006a-132">Reset the state of the profile and restart synchronization.</span></span>                                                                    |
| [<span data-ttu-id="e006a-133">Iniciar perfil CSV</span><span class="sxs-lookup"><span data-stu-id="e006a-133">Start CSV profile</span></span>](../api/educationsynchronizationprofile-start.md)      | <span data-ttu-id="e006a-134">coleção [educationFileSynchronizationVerificationMessage]</span><span class="sxs-lookup"><span data-stu-id="e006a-134">[educationFileSynchronizationVerificationMessage]collection</span></span> | <span data-ttu-id="e006a-135">Verifique os arquivos de origem carregados e inicie a sincronização.</span><span class="sxs-lookup"><span data-stu-id="e006a-135">Verify the uploaded source files and start synchronization.</span></span> <span data-ttu-id="e006a-136">Aplica-se somente quando o provedor de dados é [educationCsvDataProvider].</span><span class="sxs-lookup"><span data-stu-id="e006a-136">Applies only when the data provider is [educationCsvDataProvider].</span></span> |
| [<span data-ttu-id="e006a-137">Obter URL de upload de CSV</span><span class="sxs-lookup"><span data-stu-id="e006a-137">Get CSV upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md) | <span data-ttu-id="e006a-138">string</span><span class="sxs-lookup"><span data-stu-id="e006a-138">string</span></span>                                                      | <span data-ttu-id="e006a-139">Retornar a URL de curta duração para carregar arquivos de dados CSV.</span><span class="sxs-lookup"><span data-stu-id="e006a-139">Return the short-lived URL to upload CSV data files.</span></span> <span data-ttu-id="e006a-140">Aplica-se somente quando o provedor de dados é [educationCsvDataProvider].</span><span class="sxs-lookup"><span data-stu-id="e006a-140">Applies only when the data provider is [educationCsvDataProvider].</span></span>        |
| [<span data-ttu-id="e006a-141">Obter status</span><span class="sxs-lookup"><span data-stu-id="e006a-141">Get status</span></span>](../api/educationsynchronizationprofilestatus-get.md)         | <span data-ttu-id="e006a-142">[educationsynchronizationProfileStatus]</span><span class="sxs-lookup"><span data-stu-id="e006a-142">[educationsynchronizationProfileStatus]</span></span>                     | <span data-ttu-id="e006a-143">Retornar o status de um perfil de sincronização específico.</span><span class="sxs-lookup"><span data-stu-id="e006a-143">Return the status of a specific synchronization profile.</span></span>                                                                       |
| [<span data-ttu-id="e006a-144">Obter erros</span><span class="sxs-lookup"><span data-stu-id="e006a-144">Get errors</span></span>](../api/educationsynchronizationerrors-get.md)                | <span data-ttu-id="e006a-145">coleção [educationSynchronizationError]</span><span class="sxs-lookup"><span data-stu-id="e006a-145">[educationSynchronizationError] collection</span></span>                  | <span data-ttu-id="e006a-146">Obtenha todos os erros gerados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="e006a-146">Get all the errors generated during synchronization.</span></span>                                                                           |

## <a name="properties"></a><span data-ttu-id="e006a-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e006a-147">Properties</span></span>

| <span data-ttu-id="e006a-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e006a-148">Property</span></span>                             | <span data-ttu-id="e006a-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="e006a-149">Type</span></span>                                                   | <span data-ttu-id="e006a-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="e006a-150">Description</span></span>                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e006a-151">id</span><span class="sxs-lookup"><span data-stu-id="e006a-151">id</span></span>                                   | <span data-ttu-id="e006a-152">String</span><span class="sxs-lookup"><span data-stu-id="e006a-152">String</span></span>                                                 | <span data-ttu-id="e006a-153">O identificador exclusivo do recurso.</span><span class="sxs-lookup"><span data-stu-id="e006a-153">The unique identifier for the resource.</span></span> <span data-ttu-id="e006a-154">(somente leitura)</span><span class="sxs-lookup"><span data-stu-id="e006a-154">(read-only)</span></span>                                                                               |
| <span data-ttu-id="e006a-155">displayName</span><span class="sxs-lookup"><span data-stu-id="e006a-155">displayName</span></span>                          | <span data-ttu-id="e006a-156">String</span><span class="sxs-lookup"><span data-stu-id="e006a-156">String</span></span>                                                 | <span data-ttu-id="e006a-157">Nome do perfil de configuração para sincronizar identidades.</span><span class="sxs-lookup"><span data-stu-id="e006a-157">Name of the configuration profile for syncing identities.</span></span>                                                                         |
| <span data-ttu-id="e006a-158">DataProvider</span><span class="sxs-lookup"><span data-stu-id="e006a-158">dataProvider</span></span>                         | <span data-ttu-id="e006a-159">[educationSynchronizationDataProvider]</span><span class="sxs-lookup"><span data-stu-id="e006a-159">[educationSynchronizationDataProvider]</span></span>                 | <span data-ttu-id="e006a-160">O provedor de dados usado para o perfil.</span><span class="sxs-lookup"><span data-stu-id="e006a-160">The data provider used for the profile.</span></span>                                                                                           |
| <span data-ttu-id="e006a-161">expirationDate</span><span class="sxs-lookup"><span data-stu-id="e006a-161">expirationDate</span></span>                       | <span data-ttu-id="e006a-162">Data</span><span class="sxs-lookup"><span data-stu-id="e006a-162">Date</span></span>                                                   | <span data-ttu-id="e006a-163">A data em que o perfil deve ser considerado expirado e parar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="e006a-163">The date the profile should be considered expired and cease syncing.</span></span> <span data-ttu-id="e006a-164">Quando `null` .</span><span class="sxs-lookup"><span data-stu-id="e006a-164">When `null`.</span></span> <span data-ttu-id="e006a-165">o perfil nunca expirará.</span><span class="sxs-lookup"><span data-stu-id="e006a-165">the profile will never expire.</span></span> <span data-ttu-id="e006a-166">(opcional)</span><span class="sxs-lookup"><span data-stu-id="e006a-166">(optional)</span></span>       |
| <span data-ttu-id="e006a-167">handleSpecialCharacterConstraint</span><span class="sxs-lookup"><span data-stu-id="e006a-167">handleSpecialCharacterConstraint</span></span>     | <span data-ttu-id="e006a-168">Bool</span><span class="sxs-lookup"><span data-stu-id="e006a-168">Bool</span></span>                                                   | <span data-ttu-id="e006a-169">Determina se a escola de sincronização de dados deve substituir automaticamente caracteres especiais não suportados durante a sincronização da origem.</span><span class="sxs-lookup"><span data-stu-id="e006a-169">Determines if School Data Sync should automatically replace unsupported special characters while syncing from source.</span></span>             |
| <span data-ttu-id="e006a-170">identitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e006a-170">identitySynchronizationConfiguration</span></span> | <span data-ttu-id="e006a-171">[educationIdentitySynchronizationConfiguration]</span><span class="sxs-lookup"><span data-stu-id="e006a-171">[educationIdentitySynchronizationConfiguration]</span></span>        | <span data-ttu-id="e006a-172">Determina como o perfil deve [criar usuários novos][fullsync] ou [correspondentes existentes][dirsync] do AAD.</span><span class="sxs-lookup"><span data-stu-id="e006a-172">Determines how the Profile should [create new][fullsync] or [match existing][dirsync] AAD Users.</span></span>                                  |
| <span data-ttu-id="e006a-173">licensesToAssign</span><span class="sxs-lookup"><span data-stu-id="e006a-173">licensesToAssign</span></span>                     | <span data-ttu-id="e006a-174">coleção [educationSynchronizationLicenseAssignment]</span><span class="sxs-lookup"><span data-stu-id="e006a-174">[educationSynchronizationLicenseAssignment] collection</span></span> | <span data-ttu-id="e006a-175">Configuração da instalação da licença.</span><span class="sxs-lookup"><span data-stu-id="e006a-175">License setup configuration.</span></span>                                                                                                      |
| <span data-ttu-id="e006a-176">state</span><span class="sxs-lookup"><span data-stu-id="e006a-176">state</span></span>                                | <span data-ttu-id="e006a-177">educationSynchronizationProfileState</span><span class="sxs-lookup"><span data-stu-id="e006a-177">educationSynchronizationProfileState</span></span>                   | <span data-ttu-id="e006a-178">O estado do perfil.</span><span class="sxs-lookup"><span data-stu-id="e006a-178">The state of the profile.</span></span> <span data-ttu-id="e006a-179">Os valores possíveis são: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span><span class="sxs-lookup"><span data-stu-id="e006a-179">Possible values are: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e006a-180">Relações</span><span class="sxs-lookup"><span data-stu-id="e006a-180">Relationships</span></span>

| <span data-ttu-id="e006a-181">Relação</span><span class="sxs-lookup"><span data-stu-id="e006a-181">Relationship</span></span>  | <span data-ttu-id="e006a-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="e006a-182">Type</span></span>                                       | <span data-ttu-id="e006a-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="e006a-183">Description</span></span>                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| <span data-ttu-id="e006a-184">erros</span><span class="sxs-lookup"><span data-stu-id="e006a-184">errors</span></span>        | <span data-ttu-id="e006a-185">coleção [educationSynchronizationError]</span><span class="sxs-lookup"><span data-stu-id="e006a-185">[educationSynchronizationError] collection</span></span> | <span data-ttu-id="e006a-186">Todos os erros associados a este perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="e006a-186">All errors associated with this synchronization profile.</span></span> |
| <span data-ttu-id="e006a-187">profileStatus</span><span class="sxs-lookup"><span data-stu-id="e006a-187">profileStatus</span></span> | <span data-ttu-id="e006a-188">[educationSynchronizationProfileStatus]</span><span class="sxs-lookup"><span data-stu-id="e006a-188">[educationSynchronizationProfileStatus]</span></span>    | <span data-ttu-id="e006a-189">O status da sincronização.</span><span class="sxs-lookup"><span data-stu-id="e006a-189">The synchronization status.</span></span>                              |

## <a name="data-providers"></a><span data-ttu-id="e006a-190">Provedores de dados</span><span class="sxs-lookup"><span data-stu-id="e006a-190">Data Providers</span></span>

<span data-ttu-id="e006a-191">Cada [educationSynchronizationProfile] deve especificar um dos provedores de dados a seguir para usar como a fonte de sincronização.</span><span class="sxs-lookup"><span data-stu-id="e006a-191">Each [educationSynchronizationProfile] must specify one of the follow data providers to use as the synchronization source.</span></span>

| <span data-ttu-id="e006a-192">Data Provider</span><span class="sxs-lookup"><span data-stu-id="e006a-192">Data Provider</span></span>                                                             | <span data-ttu-id="e006a-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="e006a-193">Description</span></span>                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e006a-194">[educationCsvDataProvider]</span><span class="sxs-lookup"><span data-stu-id="e006a-194">[educationCsvDataProvider]</span></span>                                                | <span data-ttu-id="e006a-195">Arquivos CSV carregados para a [URL SAS](../api/educationsynchronizationprofile-uploadurl.md) do perfil</span><span class="sxs-lookup"><span data-stu-id="e006a-195">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="e006a-196">educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="e006a-196">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="e006a-197">API do OneRoster v 1.1</span><span class="sxs-lookup"><span data-stu-id="e006a-197">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="e006a-198">[educationPowerSchoolDataProvider]</span><span class="sxs-lookup"><span data-stu-id="e006a-198">[educationPowerSchoolDataProvider]</span></span>                                        | <span data-ttu-id="e006a-199">API da PowerSchool</span><span class="sxs-lookup"><span data-stu-id="e006a-199">PowerSchool API</span></span>                                                                                    |

## <a name="json-representation"></a><span data-ttu-id="e006a-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e006a-200">JSON representation</span></span>

<span data-ttu-id="e006a-201">Veja a seguir uma representação JSON do recurso **educationSynchronizationProfile** .</span><span class="sxs-lookup"><span data-stu-id="e006a-201">The following is a JSON representation of the **educationSynchronizationProfile** resource.</span></span>

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
  "handleSpecialCharacterConstraint": "Boolean",
  "expirationDate": "Date"
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


