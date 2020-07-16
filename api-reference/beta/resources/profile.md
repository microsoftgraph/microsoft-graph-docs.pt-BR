---
title: tipo de recurso Profile
description: Representa propriedades que são descritivas de um usuário e que são mostradas em compartilhamento, as experiências de pessoas entre o Microsoft 365 e serviços e experiências de terceiros por meio do Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1f80dfccbd662e1e398c0d4b79b0086575a83e2b
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050874"
---
# <a name="profile-resource-type"></a><span data-ttu-id="ee539-103">tipo de recurso Profile</span><span class="sxs-lookup"><span data-stu-id="ee539-103">profile resource type</span></span>

<span data-ttu-id="ee539-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee539-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee539-105">Representa propriedades que são descritivas de um usuário em um locatário, por exemplo, aniversários e atividades de educação.</span><span class="sxs-lookup"><span data-stu-id="ee539-105">Represents properties that are descriptive of a user in a tenant, for example, anniversaries and education activities.</span></span> <span data-ttu-id="ee539-106">Essas propriedades são discadas em Shared, experiências de pessoas entre o Microsoft 365 e serviços e experiências de terceiros por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ee539-106">These properties are surfaced in shared, people experiences across Microsoft 365 and third-party services and experiences via Microsoft Graph.</span></span> 

<span data-ttu-id="ee539-107">Programaticamente, essas propriedades são expressas como [relações](#relationships) do recurso de **perfil** .</span><span class="sxs-lookup"><span data-stu-id="ee539-107">Programmatically, these properties are expressed as [relationships](#relationships) of the **profile** resource.</span></span> <span data-ttu-id="ee539-108">Para obter uma destas propriedades de navegação ou criar uma instância dessas propriedades para o usuário, use o método GET ou POST correspondente nessa propriedade, quando aplicável.</span><span class="sxs-lookup"><span data-stu-id="ee539-108">To get one of these navigation properties or create an instance of these properties for the user, use the corresponding GET or POST method on that property, where applicable.</span></span> <span data-ttu-id="ee539-109">Consulte os [métodos](#methods) listados abaixo.</span><span class="sxs-lookup"><span data-stu-id="ee539-109">See the [methods](#methods) listed below.</span></span>

## <a name="methods"></a><span data-ttu-id="ee539-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="ee539-110">Methods</span></span>

| <span data-ttu-id="ee539-111">Método</span><span class="sxs-lookup"><span data-stu-id="ee539-111">Method</span></span>                                                                     | <span data-ttu-id="ee539-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ee539-112">Return Type</span></span>                                                    | <span data-ttu-id="ee539-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee539-113">Description</span></span>                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [<span data-ttu-id="ee539-114">Obter perfil</span><span class="sxs-lookup"><span data-stu-id="ee539-114">Get profile</span></span>](../api/profile-get.md)                                       | [<span data-ttu-id="ee539-115">perfil</span><span class="sxs-lookup"><span data-stu-id="ee539-115">profile</span></span>](profile.md)                                          | <span data-ttu-id="ee539-116">Leia as propriedades e as relações do objeto de perfil.</span><span class="sxs-lookup"><span data-stu-id="ee539-116">Read properties and relationships of the profile object.</span></span>                                         |
| [<span data-ttu-id="ee539-117">Excluir perfil</span><span class="sxs-lookup"><span data-stu-id="ee539-117">Delete profile</span></span>](../api/profile-delete.md)                                 | <span data-ttu-id="ee539-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee539-118">None</span></span>                                                           | <span data-ttu-id="ee539-119">Excluir um objeto de **perfil** .</span><span class="sxs-lookup"><span data-stu-id="ee539-119">Delete a **profile** object.</span></span>                                                                 |
| [<span data-ttu-id="ee539-120">Listar conta</span><span class="sxs-lookup"><span data-stu-id="ee539-120">List account</span></span>](../api/profile-list-account.md)                             | <span data-ttu-id="ee539-121">coleção [userAccountInformation](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-121">[userAccountInformation](useraccountinformation.md) collection</span></span> | <span data-ttu-id="ee539-122">Obtenha uma coleção de objetos **userAccountInformation** .</span><span class="sxs-lookup"><span data-stu-id="ee539-122">Get a **userAccountInformation** object collection.</span></span>                                          |
| [<span data-ttu-id="ee539-123">Criar personAnniversary</span><span class="sxs-lookup"><span data-stu-id="ee539-123">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)           | [<span data-ttu-id="ee539-124">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="ee539-124">personAnniversary</span></span>](personanniversary.md)                      | <span data-ttu-id="ee539-125">Crie um novo **personAnniversary** postando na coleção de datas comemorativas.</span><span class="sxs-lookup"><span data-stu-id="ee539-125">Create a new **personAnniversary** by posting to the anniversaries collection.</span></span>               |
| [<span data-ttu-id="ee539-126">Listar aniversários</span><span class="sxs-lookup"><span data-stu-id="ee539-126">List anniversaries</span></span>](../api/profile-list-anniversaries.md)                 | <span data-ttu-id="ee539-127">coleção [personAnniversary](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-127">[personAnniversary](personanniversary.md) collection</span></span>           | <span data-ttu-id="ee539-128">Obtenha uma coleção de objetos **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="ee539-128">Get a **personAnniversary** object collection.</span></span>                                               |
| [<span data-ttu-id="ee539-129">Criar educationalActivity</span><span class="sxs-lookup"><span data-stu-id="ee539-129">Create educationalActivity</span></span>](../api/profile-post-educationalactivities.md) | [<span data-ttu-id="ee539-130">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="ee539-130">educationalActivity</span></span>](educationalactivity.md)                  | <span data-ttu-id="ee539-131">Crie um novo **educationalActivity** postando na coleção **educationalActivities** .</span><span class="sxs-lookup"><span data-stu-id="ee539-131">Create a new **educationalActivity** by posting to the **educationalActivities** collection.</span></span> |
| [<span data-ttu-id="ee539-132">Listar educationalActivities</span><span class="sxs-lookup"><span data-stu-id="ee539-132">List educationalActivities</span></span>](../api/profile-list-educationalactivities.md) | <span data-ttu-id="ee539-133">coleção [educationalActivity](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-133">[educationalActivity](educationalactivity.md) collection</span></span>       | <span data-ttu-id="ee539-134">Obtenha uma coleção de objetos **educationalActivity** .</span><span class="sxs-lookup"><span data-stu-id="ee539-134">Get an **educationalActivity** object collection.</span></span>                                            |
| [<span data-ttu-id="ee539-135">Criar email</span><span class="sxs-lookup"><span data-stu-id="ee539-135">Create itemEmail</span></span>](../api/profile-post-emails.md)                          | [<span data-ttu-id="ee539-136">Email</span><span class="sxs-lookup"><span data-stu-id="ee539-136">itemEmail</span></span>](itememail.md)                                      | <span data-ttu-id="ee539-137">Crie um novo **email** postando na coleção emails.</span><span class="sxs-lookup"><span data-stu-id="ee539-137">Create a new **itemEmail** by posting to the emails collection.</span></span>                              |
| [<span data-ttu-id="ee539-138">Listar emails</span><span class="sxs-lookup"><span data-stu-id="ee539-138">List emails</span></span>](../api/profile-list-emails.md)                               | <span data-ttu-id="ee539-139">coleção [email](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-139">[itemEmail](itememail.md) collection</span></span>                           | <span data-ttu-id="ee539-140">Obter uma coleção de objetos de **email** .</span><span class="sxs-lookup"><span data-stu-id="ee539-140">Get an **itemEmail** object collection.</span></span>                                                      |
| [<span data-ttu-id="ee539-141">Criar personInterest</span><span class="sxs-lookup"><span data-stu-id="ee539-141">Create personInterest</span></span>](../api/profile-post-interests.md)                  | [<span data-ttu-id="ee539-142">personInterest</span><span class="sxs-lookup"><span data-stu-id="ee539-142">personInterest</span></span>](personinterest.md)                            | <span data-ttu-id="ee539-143">Crie um novo **personInterest** postando na coleção interesses.</span><span class="sxs-lookup"><span data-stu-id="ee539-143">Create a new **personInterest** by posting to the interests collection.</span></span>                      |
| [<span data-ttu-id="ee539-144">Listar interesses</span><span class="sxs-lookup"><span data-stu-id="ee539-144">List interests</span></span>](../api/profile-list-interests.md)                         | <span data-ttu-id="ee539-145">coleção [personInterest](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-145">[personInterest](personinterest.md) collection</span></span>                 | <span data-ttu-id="ee539-146">Obtenha uma coleção de objetos **personInterest** .</span><span class="sxs-lookup"><span data-stu-id="ee539-146">Get a **personInterest** object collection.</span></span>                                                  |
| [<span data-ttu-id="ee539-147">Criar languageProficiency</span><span class="sxs-lookup"><span data-stu-id="ee539-147">Create languageProficiency</span></span>](../api/profile-post-languages.md)             | [<span data-ttu-id="ee539-148">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="ee539-148">languageProficiency</span></span>](languageproficiency.md)                  | <span data-ttu-id="ee539-149">Crie um novo **languageProficiency** postando na coleção de idiomas.</span><span class="sxs-lookup"><span data-stu-id="ee539-149">Create a new **languageProficiency** by posting to the languages collection.</span></span>                 |
| [<span data-ttu-id="ee539-150">Idiomas de lista</span><span class="sxs-lookup"><span data-stu-id="ee539-150">List languages</span></span>](../api/profile-list-languages.md)                         | <span data-ttu-id="ee539-151">coleção [languageProficiency](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-151">[languageProficiency](languageproficiency.md) collection</span></span>       | <span data-ttu-id="ee539-152">Obtenha uma coleção de objetos **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="ee539-152">Get a **languageProficiency** object collection.</span></span>                                             |
| [<span data-ttu-id="ee539-153">Nomes da lista</span><span class="sxs-lookup"><span data-stu-id="ee539-153">List names</span></span>](../api/profile-list-names.md)                                 | <span data-ttu-id="ee539-154">coleção [PersonName](personname.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-154">[personName](personname.md) collection</span></span>                         | <span data-ttu-id="ee539-155">Obtenha uma coleção de objetos **PersonName** .</span><span class="sxs-lookup"><span data-stu-id="ee539-155">Get a **personName** object collection.</span></span>                                                      |
| [<span data-ttu-id="ee539-156">Criar PersonName</span><span class="sxs-lookup"><span data-stu-id="ee539-156">Create personName</span></span>](../api/profile-post-names.md)                          | [<span data-ttu-id="ee539-157">personName</span><span class="sxs-lookup"><span data-stu-id="ee539-157">personName</span></span>](personName.md)                                    | <span data-ttu-id="ee539-158">Crie um novo objeto **PersonName** postando na coleção names.</span><span class="sxs-lookup"><span data-stu-id="ee539-158">Create a new **personName** object by posting to the names collection.</span></span>                       |
| [<span data-ttu-id="ee539-159">Listar sites</span><span class="sxs-lookup"><span data-stu-id="ee539-159">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="ee539-160">coleção [personWebsite](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-160">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="ee539-161">Obtenha uma coleção de objetos **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="ee539-161">Get a **personWebsite** object collection.</span></span>                                                   |
| [<span data-ttu-id="ee539-162">Criar um número de telefone</span><span class="sxs-lookup"><span data-stu-id="ee539-162">Create itemPhone</span></span>](../api/profile-post-phones.md)                          | [<span data-ttu-id="ee539-163">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="ee539-163">itemPhone</span></span>](itemphone.md)                                      | <span data-ttu-id="ee539-164">Criar um novo meu telefone postando na coleção phones.</span><span class="sxs-lookup"><span data-stu-id="ee539-164">Create a new itemPhone by posting to the phones collection.</span></span>                                  |
| [<span data-ttu-id="ee539-165">Listar telefones</span><span class="sxs-lookup"><span data-stu-id="ee539-165">List phones</span></span>](../api/profile-list-phones.md)                               | <span data-ttu-id="ee539-166">coleção [Multiphone](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-166">[itemPhone](itemphone.md) collection</span></span>                           | <span data-ttu-id="ee539-167">Obter uma coleção de objetos de **Multiphone** .</span><span class="sxs-lookup"><span data-stu-id="ee539-167">Get a **itemPhone** object collection.</span></span>                                                       |
| [<span data-ttu-id="ee539-168">Criar workPosition</span><span class="sxs-lookup"><span data-stu-id="ee539-168">Create workPosition</span></span>](../api/profile-post-positions.md)                    | [<span data-ttu-id="ee539-169">workPosition</span><span class="sxs-lookup"><span data-stu-id="ee539-169">workPosition</span></span>](workposition.md)                                | <span data-ttu-id="ee539-170">Crie um novo workPosition postando na coleção Positions.</span><span class="sxs-lookup"><span data-stu-id="ee539-170">Create a new workPosition by posting to the positions collection.</span></span>                            |
| [<span data-ttu-id="ee539-171">Listar posições</span><span class="sxs-lookup"><span data-stu-id="ee539-171">List positions</span></span>](../api/profile-list-positions.md)                         | <span data-ttu-id="ee539-172">coleção [workPosition](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-172">[workPosition](workposition.md) collection</span></span>                     | <span data-ttu-id="ee539-173">Obtenha uma coleção de objetos **workPosition** .</span><span class="sxs-lookup"><span data-stu-id="ee539-173">Get a **workPosition** object collection.</span></span>                                                    |
| [<span data-ttu-id="ee539-174">Criar projectParticipation</span><span class="sxs-lookup"><span data-stu-id="ee539-174">Create projectParticipation</span></span>](../api/profile-post-projects.md)             | [<span data-ttu-id="ee539-175">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="ee539-175">projectParticipation</span></span>](projectparticipation.md)                | <span data-ttu-id="ee539-176">Criar um novo **projectParticipation** postando na coleção Projects.</span><span class="sxs-lookup"><span data-stu-id="ee539-176">Create a new **projectParticipation** by posting to the projects collection.</span></span>                 |
| [<span data-ttu-id="ee539-177">Listar projetos</span><span class="sxs-lookup"><span data-stu-id="ee539-177">List projects</span></span>](../api/profile-list-projects.md)                           | <span data-ttu-id="ee539-178">coleção [projectParticipation](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-178">[projectParticipation](projectparticipation.md) collection</span></span>     | <span data-ttu-id="ee539-179">Obtenha uma coleção de objetos **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="ee539-179">Get a **projectParticipation** object collection.</span></span>                                            |
| [<span data-ttu-id="ee539-180">Criar skillProficiency</span><span class="sxs-lookup"><span data-stu-id="ee539-180">Create skillProficiency</span></span>](../api/profile-post-skills.md)                   | [<span data-ttu-id="ee539-181">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="ee539-181">skillProficiency</span></span>](skillproficiency.md)                        | <span data-ttu-id="ee539-182">Crie um novo **skillProficiency** postando na coleção de habilidades.</span><span class="sxs-lookup"><span data-stu-id="ee539-182">Create a new **skillProficiency** by posting to the skills collection.</span></span>                       |
| [<span data-ttu-id="ee539-183">Listar qualificações</span><span class="sxs-lookup"><span data-stu-id="ee539-183">List skills</span></span>](../api/profile-list-skills.md)                               | <span data-ttu-id="ee539-184">coleção [skillProficiency](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-184">[skillProficiency](skillproficiency.md) collection</span></span>             | <span data-ttu-id="ee539-185">Obtenha uma coleção de objetos **skillProficiency** .</span><span class="sxs-lookup"><span data-stu-id="ee539-185">Get a **skillProficiency** object collection.</span></span>                                                |
| [<span data-ttu-id="ee539-186">Criar conta da</span><span class="sxs-lookup"><span data-stu-id="ee539-186">Create webAccount</span></span>](../api/profile-post-webaccounts.md)                    | [<span data-ttu-id="ee539-187">conta da</span><span class="sxs-lookup"><span data-stu-id="ee539-187">webAccount</span></span>](webaccount.md)                                    | <span data-ttu-id="ee539-188">Crie uma nova **conta da webaccount** postando na coleção webaccounts.</span><span class="sxs-lookup"><span data-stu-id="ee539-188">Create a new **webAccount** by posting to the webAccounts collection.</span></span>                        |
| [<span data-ttu-id="ee539-189">Listar contas da webaccount</span><span class="sxs-lookup"><span data-stu-id="ee539-189">List webAccounts</span></span>](../api/profile-list-webaccounts.md)                     | <span data-ttu-id="ee539-190">coleção [Webaccount](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-190">[webAccount](webaccount.md) collection</span></span>                         | <span data-ttu-id="ee539-191">Obtenha uma coleção de objetos **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="ee539-191">Get a **webAccount** object collection.</span></span>                                                      |
| [<span data-ttu-id="ee539-192">Criar personWebsite</span><span class="sxs-lookup"><span data-stu-id="ee539-192">Create personWebsite</span></span>](../api/profile-post-websites.md)                    | [<span data-ttu-id="ee539-193">personWebsite</span><span class="sxs-lookup"><span data-stu-id="ee539-193">personWebsite</span></span>](personwebsite.md)                              | <span data-ttu-id="ee539-194">Crie um novo **personWebsite** postando na coleção sites.</span><span class="sxs-lookup"><span data-stu-id="ee539-194">Create a new **personWebsite** by posting to the websites collection.</span></span>                        |
| [<span data-ttu-id="ee539-195">Listar sites</span><span class="sxs-lookup"><span data-stu-id="ee539-195">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="ee539-196">coleção [personWebsite](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-196">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="ee539-197">Obtenha uma coleção de objetos **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="ee539-197">Get a **personWebsite** object collection.</span></span>                                                   |

## <a name="properties"></a><span data-ttu-id="ee539-198">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee539-198">Properties</span></span>

| <span data-ttu-id="ee539-199">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee539-199">Property</span></span>     | <span data-ttu-id="ee539-200">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee539-200">Type</span></span>        | <span data-ttu-id="ee539-201">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee539-201">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee539-202">id</span><span class="sxs-lookup"><span data-stu-id="ee539-202">id</span></span>            |<span data-ttu-id="ee539-203">String</span><span class="sxs-lookup"><span data-stu-id="ee539-203">String</span></span>       | <span data-ttu-id="ee539-204">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-204">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="ee539-205">Relações</span><span class="sxs-lookup"><span data-stu-id="ee539-205">Relationships</span></span>

| <span data-ttu-id="ee539-206">Relação</span><span class="sxs-lookup"><span data-stu-id="ee539-206">Relationship</span></span>          | <span data-ttu-id="ee539-207">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee539-207">Type</span></span>                                                         | <span data-ttu-id="ee539-208">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee539-208">Description</span></span>                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="ee539-209">Count</span><span class="sxs-lookup"><span data-stu-id="ee539-209">account</span></span>                |<span data-ttu-id="ee539-210">coleção [userAccountInformation](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-210">[userAccountInformation](useraccountinformation.md) collection</span></span>| <span data-ttu-id="ee539-211">Representa informações especificamente associadas à conta de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ee539-211">Represents information specifically tied to a user's account.</span></span> <span data-ttu-id="ee539-212">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-212">Read-only.</span></span> <span data-ttu-id="ee539-213">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-213">Nullable.</span></span>                                                             |
|<span data-ttu-id="ee539-214">datas especiais</span><span class="sxs-lookup"><span data-stu-id="ee539-214">anniversaries</span></span>          |<span data-ttu-id="ee539-215">coleção [personAnniversary](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-215">[personAnniversary](personanniversary.md) collection</span></span>          | <span data-ttu-id="ee539-216">Representa os detalhes de datas significativas associadas a uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="ee539-216">Represents the details of meaningful dates associated with a person.</span></span> <span data-ttu-id="ee539-217">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-217">Read-only.</span></span> <span data-ttu-id="ee539-218">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-218">Nullable.</span></span>                                                      |
|<span data-ttu-id="ee539-219">educationalActivities</span><span class="sxs-lookup"><span data-stu-id="ee539-219">educationalActivities</span></span>  |<span data-ttu-id="ee539-220">coleção [educationalActivity](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-220">[educationalActivity](educationalactivity.md) collection</span></span>      | <span data-ttu-id="ee539-221">Representa os dados que um usuário forneceu relacionados ao Undergraduate, graduado, dograduação ou outras atividades educacionais.</span><span class="sxs-lookup"><span data-stu-id="ee539-221">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span> <span data-ttu-id="ee539-222">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-222">Read-only.</span></span> <span data-ttu-id="ee539-223">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-223">Nullable.</span></span>|
|<span data-ttu-id="ee539-224">email</span><span class="sxs-lookup"><span data-stu-id="ee539-224">emails</span></span>                 |<span data-ttu-id="ee539-225">coleção [email](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-225">[itemEmail](itememail.md) collection</span></span>                          | <span data-ttu-id="ee539-226">Representa informações detalhadas sobre endereços de email associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="ee539-226">Represents detailed information about email addresses associated with the user.</span></span> <span data-ttu-id="ee539-227">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-227">Read-only.</span></span> <span data-ttu-id="ee539-228">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-228">Nullable.</span></span>                                           |
|<span data-ttu-id="ee539-229">interests</span><span class="sxs-lookup"><span data-stu-id="ee539-229">interests</span></span>              |<span data-ttu-id="ee539-230">coleção [personInterest](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-230">[personInterest](personinterest.md) collection</span></span>                | <span data-ttu-id="ee539-231">Fornece informações detalhadas sobre os interesses que o usuário tenha associado a si mesmos em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="ee539-231">Provides detailed information about interests the user has associated with themselves in various services.</span></span> <span data-ttu-id="ee539-232">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-232">Read-only.</span></span> <span data-ttu-id="ee539-233">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-233">Nullable.</span></span>                |
|<span data-ttu-id="ee539-234">Idiomas</span><span class="sxs-lookup"><span data-stu-id="ee539-234">languages</span></span>              |<span data-ttu-id="ee539-235">coleção [languageProficiency](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-235">[languageProficiency](languageproficiency.md) collection</span></span>      | <span data-ttu-id="ee539-236">Representa informações detalhadas sobre os idiomas que um usuário adicionou ao perfil.</span><span class="sxs-lookup"><span data-stu-id="ee539-236">Represents detailed information about languages that a user has added to their profile.</span></span> <span data-ttu-id="ee539-237">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-237">Read-only.</span></span> <span data-ttu-id="ee539-238">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-238">Nullable.</span></span>                                   |
|<span data-ttu-id="ee539-239">telefones</span><span class="sxs-lookup"><span data-stu-id="ee539-239">phones</span></span>                 |<span data-ttu-id="ee539-240">coleção [Multiphone](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-240">[itemPhone](itemphone.md) collection</span></span>                          | <span data-ttu-id="ee539-241">Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="ee539-241">Represents detailed information about phone numbers associated with a user in various services.</span></span> <span data-ttu-id="ee539-242">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-242">Read-only.</span></span> <span data-ttu-id="ee539-243">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-243">Nullable.</span></span>                           |
|<span data-ttu-id="ee539-244">as</span><span class="sxs-lookup"><span data-stu-id="ee539-244">positions</span></span>              |<span data-ttu-id="ee539-245">coleção [workPosition](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-245">[workPosition](workposition.md) collection</span></span>                    | <span data-ttu-id="ee539-246">Representa informações detalhadas sobre posições de trabalho associadas ao perfil de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ee539-246">Represents detailed information about work positions associated with a user's profile.</span></span> <span data-ttu-id="ee539-247">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-247">Read-only.</span></span> <span data-ttu-id="ee539-248">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-248">Nullable.</span></span>                                    |
|<span data-ttu-id="ee539-249">Projetos</span><span class="sxs-lookup"><span data-stu-id="ee539-249">projects</span></span>               |<span data-ttu-id="ee539-250">coleção [projectParticipation](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-250">[projectParticipation](projectparticipation.md) collection</span></span>    | <span data-ttu-id="ee539-251">Representa informações detalhadas sobre os projetos associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="ee539-251">Represents detailed information about projects associated with a user.</span></span> <span data-ttu-id="ee539-252">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-252">Read-only.</span></span> <span data-ttu-id="ee539-253">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-253">Nullable.</span></span>                                                    |
|<span data-ttu-id="ee539-254">skills</span><span class="sxs-lookup"><span data-stu-id="ee539-254">skills</span></span>                 |<span data-ttu-id="ee539-255">coleção [skillProficiency](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-255">[skillProficiency](skillproficiency.md) collection</span></span>            | <span data-ttu-id="ee539-256">Representa informações detalhadas sobre as habilidades associadas a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="ee539-256">Represents detailed information about skills associated with a user in various services.</span></span> <span data-ttu-id="ee539-257">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-257">Read-only.</span></span> <span data-ttu-id="ee539-258">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-258">Nullable.</span></span>                                  |
|<span data-ttu-id="ee539-259">contas da</span><span class="sxs-lookup"><span data-stu-id="ee539-259">webAccounts</span></span>            |<span data-ttu-id="ee539-260">coleção [Webaccount](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-260">[webAccount](webaccount.md) collection</span></span>                        | <span data-ttu-id="ee539-261">Representa contas da Web que o usuário indicou que usa ou adicionou ao perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="ee539-261">Represents web accounts the user has indicated they use or has added to their user profile.</span></span> <span data-ttu-id="ee539-262">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-262">Read-only.</span></span> <span data-ttu-id="ee539-263">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-263">Nullable.</span></span>                               |
|<span data-ttu-id="ee539-264">websites</span><span class="sxs-lookup"><span data-stu-id="ee539-264">websites</span></span>               |<span data-ttu-id="ee539-265">coleção [personWebsite](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="ee539-265">[personWebsite](personwebsite.md) collection</span></span>                  | <span data-ttu-id="ee539-266">Representa informações detalhadas sobre sites associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="ee539-266">Represents detailed information about websites associated with a user in various services.</span></span> <span data-ttu-id="ee539-267">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee539-267">Read-only.</span></span> <span data-ttu-id="ee539-268">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ee539-268">Nullable.</span></span>                                |

## <a name="json-representation"></a><span data-ttu-id="ee539-269">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee539-269">JSON representation</span></span>

<span data-ttu-id="ee539-270">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee539-270">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "String (identifier)"
}
```

<!--
{
    "id": "profileId",
    "anniversaries": [],
    "websites": [],
    "educationalActivities": [
        {
            "endMonthYear": null,
            "startMonthYear": null,
            "completionMonthYear": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "c3a9f515-4a15-456b-9bf7-690dcd7f05d7",
            "program": {
                "abbreviation": null,
                "description": null,
                "displayName": "",
                "grade": null,
                "notes": null,
                "webUrl": null
            },
            "institution": {
                "description": null,
                "displayName": "Colorado State University",
                "location": null,
                "webUrl": null
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "emails": [
        {
            "address": "john.doe@contoso.com",
            "displayName": null,
            "type": "main",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "046452c0-c893-4fd1-a7ca-57e2ccf13861",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "interests": [
        {
            "categories": [],
            "description": null,
            "displayName": "Microsoft Graph",
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0c568cf5-5e44-4b3e-aefd-6b46ca00a880",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "languages": [
        {
            "displayName": "English (United States)",
            "tag": "en-US",
            "proficiency": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "3d34dc2e-fc84-43ff-98f6-884467caba72",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],

    "names": [
        {
            "displayName": "John Doe",
            "first": "John",
            "initials": "JD",
            "last": "Doe",
            "languageTag": null,
            "maiden": null,
            "middle": null,
            "nickname": null,
            "suffix": null,
            "title": null,
            "pronunciation": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "b79302ca-7f05-4c89-96ce-b89d5855eb0e",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "phones": [
        {
            "displayName": null,
            "type": "business",
            "number": "+47 (9) 387654321",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d22aef2c-f332-4958-aac3-8d1d710a9e32",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "positions": [
        {
            "categories": [],
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0f4d49c8-76cb-4d56-9f92-a10e182ba0e1",
            "detail": {
                "description": null,
                "endMonthYear": "0001-01-01",
                "jobTitle": "Associate Architect",
                "startMonthYear": "0001-01-01",
                "summary": null,
                "company": {
                    "displayName": "Contoso Corporation",
                    "pronunciation": null,
                    "department": "Architecture",
                    "officeLocation": "",
                    "webUrl": null,
                    "address": {
                        "type": "business",
                        "postOfficeBox": null,
                        "street": "",
                        "city": "Oslo",
                        "state": "",
                        "countryOrRegion": "",
                        "postalCode": ""
                    }
                }
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "projects": [
        {
            "categories": [],
            "client": null,
            "displayName": "Profile on Graph",
            "detail": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d6d84567-513a-47be-9be2-99fee6a12777",
            "colleagues": [],
            "sponsors": [],
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "skills": [
        {
            "categories": [],
            "displayName": "REST API Design",
            "proficiency": null,
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "9cd979f9-7a43-4dd1-a628-42bb07bd0974",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "webAccounts": []
}
-->


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
