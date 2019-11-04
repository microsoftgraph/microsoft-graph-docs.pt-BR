---
title: tipo de recurso Profile
description: Representa propriedades que são descritivas de um usuário e que são exibidas em experiências de pessoas compartilhadas entre o Microsoft 365 e serviços e experiências de terceiros por meio do Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 367a2c556b560056bcab44e6c20ae7851e493e48
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950476"
---
# <a name="profile-resource-type"></a><span data-ttu-id="13d8e-103">tipo de recurso Profile</span><span class="sxs-lookup"><span data-stu-id="13d8e-103">profile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13d8e-104">Representa propriedades descritivas de uma pessoa em um locatário.</span><span class="sxs-lookup"><span data-stu-id="13d8e-104">Represents descriptive properties of a person in a tenant.</span></span> <span data-ttu-id="13d8e-105">Essas propriedades são mostradas em experiências de pessoas compartilhadas entre o Microsoft 365 e serviços e experiências de terceiros por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="13d8e-105">These properties are surfaced in shared people experiences across Microsoft 365 and third-party services and experiences via Microsoft Graph.</span></span> 

## <a name="methods"></a><span data-ttu-id="13d8e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="13d8e-106">Methods</span></span>

| <span data-ttu-id="13d8e-107">Método</span><span class="sxs-lookup"><span data-stu-id="13d8e-107">Method</span></span>                                                                     | <span data-ttu-id="13d8e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="13d8e-108">Return Type</span></span>                                                    | <span data-ttu-id="13d8e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="13d8e-109">Description</span></span>                                                                          |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:-------------------------------------------------------------------------------------|
| [<span data-ttu-id="13d8e-110">Obter perfil</span><span class="sxs-lookup"><span data-stu-id="13d8e-110">Get profile</span></span>](../api/profile-get.md)                                       | [<span data-ttu-id="13d8e-111">profile</span><span class="sxs-lookup"><span data-stu-id="13d8e-111">profile</span></span>](profile.md)                                          | <span data-ttu-id="13d8e-112">Leia as propriedades e as relações do objeto de perfil.</span><span class="sxs-lookup"><span data-stu-id="13d8e-112">Read properties and relationships of profile object.</span></span>                                 |
| [<span data-ttu-id="13d8e-113">Excluir perfil</span><span class="sxs-lookup"><span data-stu-id="13d8e-113">Delete profile</span></span>](../api/profile-delete.md)                                         | <span data-ttu-id="13d8e-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13d8e-114">None</span></span>                                                           | <span data-ttu-id="13d8e-115">Excluir um objeto de **perfil** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-115">Delete a **profile** object.</span></span>                                                               |
| [<span data-ttu-id="13d8e-116">Listar conta</span><span class="sxs-lookup"><span data-stu-id="13d8e-116">List account</span></span>](../api/profile-list-account.md)                             | <span data-ttu-id="13d8e-117">coleção [userAccountInformation](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-117">[userAccountInformation](useraccountinformation.md) collection</span></span> | <span data-ttu-id="13d8e-118">Obtenha uma coleção de objetos **userAccountInformation** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-118">Get a **userAccountInformation** object collection.</span></span>                                      |
| [<span data-ttu-id="13d8e-119">Criar personAnniversary</span><span class="sxs-lookup"><span data-stu-id="13d8e-119">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)           | [<span data-ttu-id="13d8e-120">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="13d8e-120">personAnniversary</span></span>](personanniversary.md)                      | <span data-ttu-id="13d8e-121">Crie um novo **personAnniversary** postando na coleção de datas comemorativas.</span><span class="sxs-lookup"><span data-stu-id="13d8e-121">Create a new **personAnniversary** by posting to the anniversaries collection.</span></span>           |
| [<span data-ttu-id="13d8e-122">Listar aniversários</span><span class="sxs-lookup"><span data-stu-id="13d8e-122">List anniversaries</span></span>](../api/profile-list-anniversaries.md)                 | <span data-ttu-id="13d8e-123">coleção [personAnniversary](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-123">[personAnniversary](personanniversary.md) collection</span></span>           | <span data-ttu-id="13d8e-124">Obtenha uma coleção de objetos **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-124">Get a **personAnniversary** object collection.</span></span>                                           |
| [<span data-ttu-id="13d8e-125">Criar educationalActivity</span><span class="sxs-lookup"><span data-stu-id="13d8e-125">Create educationalActivity</span></span>](../api/profile-post-educationalactivities.md) | [<span data-ttu-id="13d8e-126">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="13d8e-126">educationalActivity</span></span>](educationalactivity.md)                  | <span data-ttu-id="13d8e-127">Crie um novo **educationalActivity** postando na coleção **educationalActivities** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-127">Create a new **educationalActivity** by posting to the **educationalActivities** collection.</span></span> |
| [<span data-ttu-id="13d8e-128">Listar educationalActivities</span><span class="sxs-lookup"><span data-stu-id="13d8e-128">List educationalActivities</span></span>](../api/profile-list-educationalactivities.md) | <span data-ttu-id="13d8e-129">coleção [educationalActivity](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-129">[educationalActivity](educationalactivity.md) collection</span></span>       | <span data-ttu-id="13d8e-130">Obtenha uma coleção de objetos **educationalActivity** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-130">Get an **educationalActivity** object collection.</span></span>                                         |
| [<span data-ttu-id="13d8e-131">Criar email</span><span class="sxs-lookup"><span data-stu-id="13d8e-131">Create itemEmail</span></span>](../api/profile-post-emails.md)                          | [<span data-ttu-id="13d8e-132">Email</span><span class="sxs-lookup"><span data-stu-id="13d8e-132">itemEmail</span></span>](itememail.md)                                      | <span data-ttu-id="13d8e-133">Crie um novo **email** postando na coleção emails.</span><span class="sxs-lookup"><span data-stu-id="13d8e-133">Create a new **itemEmail** by posting to the emails collection.</span></span>                          |
| [<span data-ttu-id="13d8e-134">Listar emails</span><span class="sxs-lookup"><span data-stu-id="13d8e-134">List emails</span></span>](../api/profile-list-emails.md)                               | <span data-ttu-id="13d8e-135">coleção [email](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-135">[itemEmail](itememail.md) collection</span></span>                           | <span data-ttu-id="13d8e-136">Obter uma coleção de objetos de **email** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-136">Get an **itemEmail** object collection.</span></span>                                                   |
| [<span data-ttu-id="13d8e-137">Criar personInterest</span><span class="sxs-lookup"><span data-stu-id="13d8e-137">Create personInterest</span></span>](../api/profile-post-interests.md)                  | [<span data-ttu-id="13d8e-138">personInterest</span><span class="sxs-lookup"><span data-stu-id="13d8e-138">personInterest</span></span>](personinterest.md)                            | <span data-ttu-id="13d8e-139">Crie um novo **personInterest** postando na coleção interesses.</span><span class="sxs-lookup"><span data-stu-id="13d8e-139">Create a new **personInterest** by posting to the interests collection.</span></span>                  |
| [<span data-ttu-id="13d8e-140">Listar interesses</span><span class="sxs-lookup"><span data-stu-id="13d8e-140">List interests</span></span>](../api/profile-list-interests.md)                         | <span data-ttu-id="13d8e-141">coleção [personInterest](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-141">[personInterest](personinterest.md) collection</span></span>                 | <span data-ttu-id="13d8e-142">Obtenha uma coleção de objetos **personInterest** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-142">Get a **personInterest** object collection.</span></span>                                              |
| [<span data-ttu-id="13d8e-143">Criar languageProficiency</span><span class="sxs-lookup"><span data-stu-id="13d8e-143">Create languageProficiency</span></span>](../api/profile-post-languages.md)             | [<span data-ttu-id="13d8e-144">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="13d8e-144">languageProficiency</span></span>](languageproficiency.md)                  | <span data-ttu-id="13d8e-145">Crie um novo **languageProficiency** postando na coleção de idiomas.</span><span class="sxs-lookup"><span data-stu-id="13d8e-145">Create a new **languageProficiency** by posting to the languages collection.</span></span>             |
| [<span data-ttu-id="13d8e-146">Idiomas de lista</span><span class="sxs-lookup"><span data-stu-id="13d8e-146">List languages</span></span>](../api/profile-list-languages.md)                         | <span data-ttu-id="13d8e-147">coleção [languageProficiency](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-147">[languageProficiency](languageproficiency.md) collection</span></span>       | <span data-ttu-id="13d8e-148">Obtenha uma coleção de objetos **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-148">Get a **languageProficiency** object collection.</span></span>                                         |
| [<span data-ttu-id="13d8e-149">Nomes da lista</span><span class="sxs-lookup"><span data-stu-id="13d8e-149">List names</span></span>](../api/profile-list-names.md)                                 | <span data-ttu-id="13d8e-150">coleção [PersonName](personname.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-150">[personName](personname.md) collection</span></span>                         | <span data-ttu-id="13d8e-151">Obtenha uma coleção de objetos **PersonName** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-151">Get a **personName** object collection.</span></span>                                                  |
| [<span data-ttu-id="13d8e-152">Criar PersonName</span><span class="sxs-lookup"><span data-stu-id="13d8e-152">Create personName</span></span>](../api/profile-post-names.md)                          | [<span data-ttu-id="13d8e-153">personName</span><span class="sxs-lookup"><span data-stu-id="13d8e-153">personName</span></span>](personName.md)                                    | <span data-ttu-id="13d8e-154">Crie um novo objeto **PersonName** postando na coleção names.</span><span class="sxs-lookup"><span data-stu-id="13d8e-154">Create a new **personName** object by posting to the names collection.</span></span>                   |
| [<span data-ttu-id="13d8e-155">Listar sites</span><span class="sxs-lookup"><span data-stu-id="13d8e-155">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="13d8e-156">coleção [personWebsite](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-156">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="13d8e-157">Obtenha uma coleção de objetos **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-157">Get a **personWebsite** object collection.</span></span>                                               |
| [<span data-ttu-id="13d8e-158">Criar um número de telefone</span><span class="sxs-lookup"><span data-stu-id="13d8e-158">Create itemPhone</span></span>](../api/profile-post-phones.md)                          | [<span data-ttu-id="13d8e-159">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="13d8e-159">itemPhone</span></span>](itemphone.md)                                      | <span data-ttu-id="13d8e-160">Criar um novo meu telefone postando na coleção phones.</span><span class="sxs-lookup"><span data-stu-id="13d8e-160">Create a new itemPhone by posting to the phones collection.</span></span>                          |
| [<span data-ttu-id="13d8e-161">Listar telefones</span><span class="sxs-lookup"><span data-stu-id="13d8e-161">List phones</span></span>](../api/profile-list-phones.md)                               | <span data-ttu-id="13d8e-162">coleção [Multiphone](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-162">[itemPhone](itemphone.md) collection</span></span>                           | <span data-ttu-id="13d8e-163">Obter uma coleção de objetos de **Multiphone** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-163">Get a **itemPhone** object collection.</span></span>                                                   |
| [<span data-ttu-id="13d8e-164">Criar workPosition</span><span class="sxs-lookup"><span data-stu-id="13d8e-164">Create workPosition</span></span>](../api/profile-post-positions.md)                    | [<span data-ttu-id="13d8e-165">workPosition</span><span class="sxs-lookup"><span data-stu-id="13d8e-165">workPosition</span></span>](workposition.md)                                | <span data-ttu-id="13d8e-166">Crie um novo workPosition postando na coleção Positions.</span><span class="sxs-lookup"><span data-stu-id="13d8e-166">Create a new workPosition by posting to the positions collection.</span></span>                    |
| [<span data-ttu-id="13d8e-167">Listar posições</span><span class="sxs-lookup"><span data-stu-id="13d8e-167">List positions</span></span>](../api/profile-list-positions.md)                         | <span data-ttu-id="13d8e-168">coleção [workPosition](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-168">[workPosition](workposition.md) collection</span></span>                     | <span data-ttu-id="13d8e-169">Obtenha uma coleção de objetos **workPosition** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-169">Get a **workPosition** object collection.</span></span>                                                |
| [<span data-ttu-id="13d8e-170">Criar projectParticipation</span><span class="sxs-lookup"><span data-stu-id="13d8e-170">Create projectParticipation</span></span>](../api/profile-post-projects.md)             | [<span data-ttu-id="13d8e-171">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="13d8e-171">projectParticipation</span></span>](projectparticipation.md)                | <span data-ttu-id="13d8e-172">Criar um novo **projectParticipation** postando na coleção Projects.</span><span class="sxs-lookup"><span data-stu-id="13d8e-172">Create a new **projectParticipation** by posting to the projects collection.</span></span>             |
| [<span data-ttu-id="13d8e-173">Listar projetos</span><span class="sxs-lookup"><span data-stu-id="13d8e-173">List projects</span></span>](../api/profile-list-projects.md)                           | <span data-ttu-id="13d8e-174">coleção [projectParticipation](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-174">[projectParticipation](projectparticipation.md) collection</span></span>     | <span data-ttu-id="13d8e-175">Obtenha uma coleção de objetos **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-175">Get a **projectParticipation** object collection.</span></span>                                        |
| [<span data-ttu-id="13d8e-176">Criar skillProficiency</span><span class="sxs-lookup"><span data-stu-id="13d8e-176">Create skillProficiency</span></span>](../api/profile-post-skills.md)                   | [<span data-ttu-id="13d8e-177">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="13d8e-177">skillProficiency</span></span>](skillproficiency.md)                        | <span data-ttu-id="13d8e-178">Crie um novo **skillProficiency** postando na coleção de habilidades.</span><span class="sxs-lookup"><span data-stu-id="13d8e-178">Create a new **skillProficiency** by posting to the skills collection.</span></span>                   |
| [<span data-ttu-id="13d8e-179">Listar qualificações</span><span class="sxs-lookup"><span data-stu-id="13d8e-179">List skills</span></span>](../api/profile-list-skills.md)                               | <span data-ttu-id="13d8e-180">coleção [skillProficiency](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-180">[skillProficiency](skillproficiency.md) collection</span></span>             | <span data-ttu-id="13d8e-181">Obtenha uma coleção de objetos **skillProficiency** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-181">Get a **skillProficiency** object collection.</span></span>                                            |
| [<span data-ttu-id="13d8e-182">Criar conta da</span><span class="sxs-lookup"><span data-stu-id="13d8e-182">Create webAccount</span></span>](../api/profile-post-webaccounts.md)                    | [<span data-ttu-id="13d8e-183">conta da</span><span class="sxs-lookup"><span data-stu-id="13d8e-183">webAccount</span></span>](webaccount.md)                                    | <span data-ttu-id="13d8e-184">Crie uma nova **conta da webaccount** postando na coleção webaccounts.</span><span class="sxs-lookup"><span data-stu-id="13d8e-184">Create a new **webAccount** by posting to the webAccounts collection.</span></span>                    |
| [<span data-ttu-id="13d8e-185">Listar contas da webaccount</span><span class="sxs-lookup"><span data-stu-id="13d8e-185">List webAccounts</span></span>](../api/profile-list-webaccounts.md)                     | <span data-ttu-id="13d8e-186">coleção [Webaccount](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-186">[webAccount](webaccount.md) collection</span></span>                         | <span data-ttu-id="13d8e-187">Obtenha uma coleção de objetos **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-187">Get a **webAccount** object collection.</span></span>                                                  |
| [<span data-ttu-id="13d8e-188">Criar personWebsite</span><span class="sxs-lookup"><span data-stu-id="13d8e-188">Create personWebsite</span></span>](../api/profile-post-websites.md)                    | [<span data-ttu-id="13d8e-189">personWebsite</span><span class="sxs-lookup"><span data-stu-id="13d8e-189">personWebsite</span></span>](personwebsite.md)                              | <span data-ttu-id="13d8e-190">Crie um novo **personWebsite** postando na coleção sites.</span><span class="sxs-lookup"><span data-stu-id="13d8e-190">Create a new **personWebsite** by posting to the websites collection.</span></span>                    |
| [<span data-ttu-id="13d8e-191">Listar sites</span><span class="sxs-lookup"><span data-stu-id="13d8e-191">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="13d8e-192">coleção [personWebsite](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-192">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="13d8e-193">Obtenha uma coleção de objetos **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="13d8e-193">Get a **personWebsite** object collection.</span></span>                                               |

## <a name="properties"></a><span data-ttu-id="13d8e-194">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13d8e-194">Properties</span></span>

| <span data-ttu-id="13d8e-195">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13d8e-195">Property</span></span>     | <span data-ttu-id="13d8e-196">Tipo</span><span class="sxs-lookup"><span data-stu-id="13d8e-196">Type</span></span>        | <span data-ttu-id="13d8e-197">Descrição</span><span class="sxs-lookup"><span data-stu-id="13d8e-197">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13d8e-198">id</span><span class="sxs-lookup"><span data-stu-id="13d8e-198">id</span></span>            |<span data-ttu-id="13d8e-199">String</span><span class="sxs-lookup"><span data-stu-id="13d8e-199">String</span></span>       | <span data-ttu-id="13d8e-200">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-200">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="13d8e-201">Relações</span><span class="sxs-lookup"><span data-stu-id="13d8e-201">Relationships</span></span>

| <span data-ttu-id="13d8e-202">Relação</span><span class="sxs-lookup"><span data-stu-id="13d8e-202">Relationship</span></span>          | <span data-ttu-id="13d8e-203">Tipo</span><span class="sxs-lookup"><span data-stu-id="13d8e-203">Type</span></span>                                                         | <span data-ttu-id="13d8e-204">Descrição</span><span class="sxs-lookup"><span data-stu-id="13d8e-204">Description</span></span>         |
|:----------------------|:-------------------------------------------------------------|:--------------------|
|<span data-ttu-id="13d8e-205">Count</span><span class="sxs-lookup"><span data-stu-id="13d8e-205">account</span></span>                |<span data-ttu-id="13d8e-206">coleção [userAccountInformation](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-206">[userAccountInformation](useraccountinformation.md) collection</span></span>| <span data-ttu-id="13d8e-207">Representa informações especificamente associadas à conta de um usuário.</span><span class="sxs-lookup"><span data-stu-id="13d8e-207">Represents information specifically tied to a user's account.</span></span> <span data-ttu-id="13d8e-208">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-208">Read-only.</span></span> <span data-ttu-id="13d8e-209">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-209">Nullable.</span></span>|
|<span data-ttu-id="13d8e-210">datas especiais</span><span class="sxs-lookup"><span data-stu-id="13d8e-210">anniversaries</span></span>          |<span data-ttu-id="13d8e-211">coleção [personAnniversary](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-211">[personAnniversary](personanniversary.md) collection</span></span>          | <span data-ttu-id="13d8e-212">Representa os detalhes de datas significativas associadas a uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="13d8e-212">Represents the details of meaningful dates associated with a person.</span></span> <span data-ttu-id="13d8e-213">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-213">Read-only.</span></span> <span data-ttu-id="13d8e-214">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-214">Nullable.</span></span>|
|<span data-ttu-id="13d8e-215">educationalActivities</span><span class="sxs-lookup"><span data-stu-id="13d8e-215">educationalActivities</span></span>  |<span data-ttu-id="13d8e-216">coleção [educationalActivity](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-216">[educationalActivity](educationalactivity.md) collection</span></span>      | <span data-ttu-id="13d8e-217">Representa os dados que um usuário forneceu relacionados ao Undergraduate, graduado, dograduação ou outras atividades educacionais.</span><span class="sxs-lookup"><span data-stu-id="13d8e-217">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span> <span data-ttu-id="13d8e-218">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-218">Read-only.</span></span> <span data-ttu-id="13d8e-219">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-219">Nullable.</span></span>|
|<span data-ttu-id="13d8e-220">email</span><span class="sxs-lookup"><span data-stu-id="13d8e-220">emails</span></span>                 |<span data-ttu-id="13d8e-221">coleção [email](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-221">[itemEmail](itememail.md) collection</span></span>                          | <span data-ttu-id="13d8e-222">Representa informações detalhadas sobre endereços de email associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="13d8e-222">Represents detailed information about email addresses associated with the user.</span></span> <span data-ttu-id="13d8e-223">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-223">Read-only.</span></span> <span data-ttu-id="13d8e-224">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-224">Nullable.</span></span>|
|<span data-ttu-id="13d8e-225">interests</span><span class="sxs-lookup"><span data-stu-id="13d8e-225">interests</span></span>              |<span data-ttu-id="13d8e-226">coleção [personInterest](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-226">[personInterest](personinterest.md) collection</span></span>                | <span data-ttu-id="13d8e-227">Fornece informações detalhadas sobre os interesses que o usuário tenha associado a si mesmos em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="13d8e-227">Provides detailed information about interests the user has associated with themselves in various services.</span></span> <span data-ttu-id="13d8e-228">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-228">Read-only.</span></span> <span data-ttu-id="13d8e-229">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-229">Nullable.</span></span>|
|<span data-ttu-id="13d8e-230">Idiomas</span><span class="sxs-lookup"><span data-stu-id="13d8e-230">languages</span></span>              |<span data-ttu-id="13d8e-231">coleção [languageProficiency](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-231">[languageProficiency](languageproficiency.md) collection</span></span>      | <span data-ttu-id="13d8e-232">Representa informações detalhadas sobre os idiomas que um usuário adicionou ao perfil.</span><span class="sxs-lookup"><span data-stu-id="13d8e-232">Represents detailed information about languages that a user has added to their profile.</span></span> <span data-ttu-id="13d8e-233">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-233">Read-only.</span></span> <span data-ttu-id="13d8e-234">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-234">Nullable.</span></span>|
|<span data-ttu-id="13d8e-235">telefones</span><span class="sxs-lookup"><span data-stu-id="13d8e-235">phones</span></span>                 |<span data-ttu-id="13d8e-236">coleção [Multiphone](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-236">[itemPhone](itemphone.md) collection</span></span>                          | <span data-ttu-id="13d8e-237">Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="13d8e-237">Represents detailed information about phone numbers associated with a user in various services.</span></span> <span data-ttu-id="13d8e-238">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-238">Read-only.</span></span> <span data-ttu-id="13d8e-239">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-239">Nullable.</span></span>|
|<span data-ttu-id="13d8e-240">as</span><span class="sxs-lookup"><span data-stu-id="13d8e-240">positions</span></span>              |<span data-ttu-id="13d8e-241">coleção [workPosition](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-241">[workPosition](workposition.md) collection</span></span>                    | <span data-ttu-id="13d8e-242">Representa informações detalhadas sobre posições de trabalho associadas ao perfil de um usuário.</span><span class="sxs-lookup"><span data-stu-id="13d8e-242">Represents detailed information about work positions associated with a user's profile.</span></span> <span data-ttu-id="13d8e-243">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-243">Read-only.</span></span> <span data-ttu-id="13d8e-244">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-244">Nullable.</span></span>|
|<span data-ttu-id="13d8e-245">Projetos</span><span class="sxs-lookup"><span data-stu-id="13d8e-245">projects</span></span>               |<span data-ttu-id="13d8e-246">coleção [projectParticipation](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-246">[projectParticipation](projectparticipation.md) collection</span></span>    | <span data-ttu-id="13d8e-247">Representa informações detalhadas sobre os projetos associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="13d8e-247">Represents detailed information about projects associated with a user.</span></span> <span data-ttu-id="13d8e-248">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-248">Read-only.</span></span> <span data-ttu-id="13d8e-249">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-249">Nullable.</span></span>|
|<span data-ttu-id="13d8e-250">skills</span><span class="sxs-lookup"><span data-stu-id="13d8e-250">skills</span></span>                 |<span data-ttu-id="13d8e-251">coleção [skillProficiency](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-251">[skillProficiency](skillproficiency.md) collection</span></span>            | <span data-ttu-id="13d8e-252">Representa informações detalhadas sobre as habilidades associadas a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="13d8e-252">Represents detailed information about skills associated with a user in various services.</span></span> <span data-ttu-id="13d8e-253">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-253">Read-only.</span></span> <span data-ttu-id="13d8e-254">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-254">Nullable.</span></span>|
|<span data-ttu-id="13d8e-255">contas da</span><span class="sxs-lookup"><span data-stu-id="13d8e-255">webAccounts</span></span>            |<span data-ttu-id="13d8e-256">coleção [Webaccount](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-256">[webAccount](webaccount.md) collection</span></span>                        | <span data-ttu-id="13d8e-257">Representa contas da Web que o usuário indicou que usa ou adicionou ao perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="13d8e-257">Represents web accounts the user has indicated they use or has added to their user profile.</span></span> <span data-ttu-id="13d8e-258">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-258">Read-only.</span></span> <span data-ttu-id="13d8e-259">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-259">Nullable.</span></span>|
|<span data-ttu-id="13d8e-260">websites</span><span class="sxs-lookup"><span data-stu-id="13d8e-260">websites</span></span>               |<span data-ttu-id="13d8e-261">coleção [personWebsite](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="13d8e-261">[personWebsite](personwebsite.md) collection</span></span>                  | <span data-ttu-id="13d8e-262">Representa informações detalhadas sobre sites associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="13d8e-262">Represents detailed information about websites associated with a user in various services.</span></span> <span data-ttu-id="13d8e-263">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13d8e-263">Read-only.</span></span> <span data-ttu-id="13d8e-264">Anulável.</span><span class="sxs-lookup"><span data-stu-id="13d8e-264">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13d8e-265">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13d8e-265">JSON representation</span></span>

<span data-ttu-id="13d8e-266">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13d8e-266">The following is a JSON representation of the resource.</span></span>

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
