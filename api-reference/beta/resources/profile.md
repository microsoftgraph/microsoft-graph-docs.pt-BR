---
title: tipo de recurso Profile
description: Representa propriedades que são descritivas de um usuário e que são exibidas em experiências de pessoas compartilhadas entre o Microsoft 365 e serviços e experiências de terceiros por meio do Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c5c7d7765d546dad5f6de39f72f092b3bf9daee6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521464"
---
# <a name="profile-resource-type"></a><span data-ttu-id="f4a4b-103">tipo de recurso Profile</span><span class="sxs-lookup"><span data-stu-id="f4a4b-103">profile resource type</span></span>

<span data-ttu-id="f4a4b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f4a4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4a4b-105">Representa propriedades descritivas de uma pessoa em um locatário.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-105">Represents descriptive properties of a person in a tenant.</span></span> <span data-ttu-id="f4a4b-106">Essas propriedades são mostradas em experiências de pessoas compartilhadas entre o Microsoft 365 e serviços e experiências de terceiros por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-106">These properties are surfaced in shared people experiences across Microsoft 365 and third-party services and experiences via Microsoft Graph.</span></span> 

## <a name="methods"></a><span data-ttu-id="f4a4b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f4a4b-107">Methods</span></span>

| <span data-ttu-id="f4a4b-108">Método</span><span class="sxs-lookup"><span data-stu-id="f4a4b-108">Method</span></span>                                                                     | <span data-ttu-id="f4a4b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4a4b-109">Return Type</span></span>                                                    | <span data-ttu-id="f4a4b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4a4b-110">Description</span></span>                                                                          |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:-------------------------------------------------------------------------------------|
| [<span data-ttu-id="f4a4b-111">Obter perfil</span><span class="sxs-lookup"><span data-stu-id="f4a4b-111">Get profile</span></span>](../api/profile-get.md)                                       | [<span data-ttu-id="f4a4b-112">perfil</span><span class="sxs-lookup"><span data-stu-id="f4a4b-112">profile</span></span>](profile.md)                                          | <span data-ttu-id="f4a4b-113">Leia as propriedades e as relações do objeto de perfil.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-113">Read properties and relationships of profile object.</span></span>                                 |
| [<span data-ttu-id="f4a4b-114">Excluir perfil</span><span class="sxs-lookup"><span data-stu-id="f4a4b-114">Delete profile</span></span>](../api/profile-delete.md)                                         | <span data-ttu-id="f4a4b-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4a4b-115">None</span></span>                                                           | <span data-ttu-id="f4a4b-116">Excluir um objeto de **perfil** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-116">Delete a **profile** object.</span></span>                                                               |
| [<span data-ttu-id="f4a4b-117">Listar conta</span><span class="sxs-lookup"><span data-stu-id="f4a4b-117">List account</span></span>](../api/profile-list-account.md)                             | <span data-ttu-id="f4a4b-118">coleção [userAccountInformation](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-118">[userAccountInformation](useraccountinformation.md) collection</span></span> | <span data-ttu-id="f4a4b-119">Obtenha uma coleção de objetos **userAccountInformation** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-119">Get a **userAccountInformation** object collection.</span></span>                                      |
| [<span data-ttu-id="f4a4b-120">Criar personAnniversary</span><span class="sxs-lookup"><span data-stu-id="f4a4b-120">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)           | [<span data-ttu-id="f4a4b-121">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="f4a4b-121">personAnniversary</span></span>](personanniversary.md)                      | <span data-ttu-id="f4a4b-122">Crie um novo **personAnniversary** postando na coleção de datas comemorativas.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-122">Create a new **personAnniversary** by posting to the anniversaries collection.</span></span>           |
| [<span data-ttu-id="f4a4b-123">Listar aniversários</span><span class="sxs-lookup"><span data-stu-id="f4a4b-123">List anniversaries</span></span>](../api/profile-list-anniversaries.md)                 | <span data-ttu-id="f4a4b-124">coleção [personAnniversary](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-124">[personAnniversary](personanniversary.md) collection</span></span>           | <span data-ttu-id="f4a4b-125">Obtenha uma coleção de objetos **personAnniversary** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-125">Get a **personAnniversary** object collection.</span></span>                                           |
| [<span data-ttu-id="f4a4b-126">Criar educationalActivity</span><span class="sxs-lookup"><span data-stu-id="f4a4b-126">Create educationalActivity</span></span>](../api/profile-post-educationalactivities.md) | [<span data-ttu-id="f4a4b-127">educationalActivity</span><span class="sxs-lookup"><span data-stu-id="f4a4b-127">educationalActivity</span></span>](educationalactivity.md)                  | <span data-ttu-id="f4a4b-128">Crie um novo **educationalActivity** postando na coleção **educationalActivities** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-128">Create a new **educationalActivity** by posting to the **educationalActivities** collection.</span></span> |
| [<span data-ttu-id="f4a4b-129">Listar educationalActivities</span><span class="sxs-lookup"><span data-stu-id="f4a4b-129">List educationalActivities</span></span>](../api/profile-list-educationalactivities.md) | <span data-ttu-id="f4a4b-130">coleção [educationalActivity](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-130">[educationalActivity](educationalactivity.md) collection</span></span>       | <span data-ttu-id="f4a4b-131">Obtenha uma coleção de objetos **educationalActivity** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-131">Get an **educationalActivity** object collection.</span></span>                                         |
| [<span data-ttu-id="f4a4b-132">Criar email</span><span class="sxs-lookup"><span data-stu-id="f4a4b-132">Create itemEmail</span></span>](../api/profile-post-emails.md)                          | [<span data-ttu-id="f4a4b-133">Email</span><span class="sxs-lookup"><span data-stu-id="f4a4b-133">itemEmail</span></span>](itememail.md)                                      | <span data-ttu-id="f4a4b-134">Crie um novo **email** postando na coleção emails.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-134">Create a new **itemEmail** by posting to the emails collection.</span></span>                          |
| [<span data-ttu-id="f4a4b-135">Listar emails</span><span class="sxs-lookup"><span data-stu-id="f4a4b-135">List emails</span></span>](../api/profile-list-emails.md)                               | <span data-ttu-id="f4a4b-136">coleção [email](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-136">[itemEmail](itememail.md) collection</span></span>                           | <span data-ttu-id="f4a4b-137">Obter uma coleção de objetos de **email** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-137">Get an **itemEmail** object collection.</span></span>                                                   |
| [<span data-ttu-id="f4a4b-138">Criar personInterest</span><span class="sxs-lookup"><span data-stu-id="f4a4b-138">Create personInterest</span></span>](../api/profile-post-interests.md)                  | [<span data-ttu-id="f4a4b-139">personInterest</span><span class="sxs-lookup"><span data-stu-id="f4a4b-139">personInterest</span></span>](personinterest.md)                            | <span data-ttu-id="f4a4b-140">Crie um novo **personInterest** postando na coleção interesses.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-140">Create a new **personInterest** by posting to the interests collection.</span></span>                  |
| [<span data-ttu-id="f4a4b-141">Listar interesses</span><span class="sxs-lookup"><span data-stu-id="f4a4b-141">List interests</span></span>](../api/profile-list-interests.md)                         | <span data-ttu-id="f4a4b-142">coleção [personInterest](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-142">[personInterest](personinterest.md) collection</span></span>                 | <span data-ttu-id="f4a4b-143">Obtenha uma coleção de objetos **personInterest** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-143">Get a **personInterest** object collection.</span></span>                                              |
| [<span data-ttu-id="f4a4b-144">Criar languageProficiency</span><span class="sxs-lookup"><span data-stu-id="f4a4b-144">Create languageProficiency</span></span>](../api/profile-post-languages.md)             | [<span data-ttu-id="f4a4b-145">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="f4a4b-145">languageProficiency</span></span>](languageproficiency.md)                  | <span data-ttu-id="f4a4b-146">Crie um novo **languageProficiency** postando na coleção de idiomas.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-146">Create a new **languageProficiency** by posting to the languages collection.</span></span>             |
| [<span data-ttu-id="f4a4b-147">Idiomas de lista</span><span class="sxs-lookup"><span data-stu-id="f4a4b-147">List languages</span></span>](../api/profile-list-languages.md)                         | <span data-ttu-id="f4a4b-148">coleção [languageProficiency](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-148">[languageProficiency](languageproficiency.md) collection</span></span>       | <span data-ttu-id="f4a4b-149">Obtenha uma coleção de objetos **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-149">Get a **languageProficiency** object collection.</span></span>                                         |
| [<span data-ttu-id="f4a4b-150">Nomes da lista</span><span class="sxs-lookup"><span data-stu-id="f4a4b-150">List names</span></span>](../api/profile-list-names.md)                                 | <span data-ttu-id="f4a4b-151">coleção [PersonName](personname.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-151">[personName](personname.md) collection</span></span>                         | <span data-ttu-id="f4a4b-152">Obtenha uma coleção de objetos **PersonName** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-152">Get a **personName** object collection.</span></span>                                                  |
| [<span data-ttu-id="f4a4b-153">Criar PersonName</span><span class="sxs-lookup"><span data-stu-id="f4a4b-153">Create personName</span></span>](../api/profile-post-names.md)                          | [<span data-ttu-id="f4a4b-154">personName</span><span class="sxs-lookup"><span data-stu-id="f4a4b-154">personName</span></span>](personName.md)                                    | <span data-ttu-id="f4a4b-155">Crie um novo objeto **PersonName** postando na coleção names.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-155">Create a new **personName** object by posting to the names collection.</span></span>                   |
| [<span data-ttu-id="f4a4b-156">Listar sites</span><span class="sxs-lookup"><span data-stu-id="f4a4b-156">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="f4a4b-157">coleção [personWebsite](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-157">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="f4a4b-158">Obtenha uma coleção de objetos **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-158">Get a **personWebsite** object collection.</span></span>                                               |
| [<span data-ttu-id="f4a4b-159">Criar um número de telefone</span><span class="sxs-lookup"><span data-stu-id="f4a4b-159">Create itemPhone</span></span>](../api/profile-post-phones.md)                          | [<span data-ttu-id="f4a4b-160">Número de telefone</span><span class="sxs-lookup"><span data-stu-id="f4a4b-160">itemPhone</span></span>](itemphone.md)                                      | <span data-ttu-id="f4a4b-161">Criar um novo meu telefone postando na coleção phones.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-161">Create a new itemPhone by posting to the phones collection.</span></span>                          |
| [<span data-ttu-id="f4a4b-162">Listar telefones</span><span class="sxs-lookup"><span data-stu-id="f4a4b-162">List phones</span></span>](../api/profile-list-phones.md)                               | <span data-ttu-id="f4a4b-163">coleção [Multiphone](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-163">[itemPhone](itemphone.md) collection</span></span>                           | <span data-ttu-id="f4a4b-164">Obter uma coleção de objetos de **Multiphone** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-164">Get a **itemPhone** object collection.</span></span>                                                   |
| [<span data-ttu-id="f4a4b-165">Criar workPosition</span><span class="sxs-lookup"><span data-stu-id="f4a4b-165">Create workPosition</span></span>](../api/profile-post-positions.md)                    | [<span data-ttu-id="f4a4b-166">workPosition</span><span class="sxs-lookup"><span data-stu-id="f4a4b-166">workPosition</span></span>](workposition.md)                                | <span data-ttu-id="f4a4b-167">Crie um novo workPosition postando na coleção Positions.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-167">Create a new workPosition by posting to the positions collection.</span></span>                    |
| [<span data-ttu-id="f4a4b-168">Listar posições</span><span class="sxs-lookup"><span data-stu-id="f4a4b-168">List positions</span></span>](../api/profile-list-positions.md)                         | <span data-ttu-id="f4a4b-169">coleção [workPosition](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-169">[workPosition](workposition.md) collection</span></span>                     | <span data-ttu-id="f4a4b-170">Obtenha uma coleção de objetos **workPosition** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-170">Get a **workPosition** object collection.</span></span>                                                |
| [<span data-ttu-id="f4a4b-171">Criar projectParticipation</span><span class="sxs-lookup"><span data-stu-id="f4a4b-171">Create projectParticipation</span></span>](../api/profile-post-projects.md)             | [<span data-ttu-id="f4a4b-172">projectParticipation</span><span class="sxs-lookup"><span data-stu-id="f4a4b-172">projectParticipation</span></span>](projectparticipation.md)                | <span data-ttu-id="f4a4b-173">Criar um novo **projectParticipation** postando na coleção Projects.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-173">Create a new **projectParticipation** by posting to the projects collection.</span></span>             |
| [<span data-ttu-id="f4a4b-174">Listar projetos</span><span class="sxs-lookup"><span data-stu-id="f4a4b-174">List projects</span></span>](../api/profile-list-projects.md)                           | <span data-ttu-id="f4a4b-175">coleção [projectParticipation](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-175">[projectParticipation](projectparticipation.md) collection</span></span>     | <span data-ttu-id="f4a4b-176">Obtenha uma coleção de objetos **projectParticipation** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-176">Get a **projectParticipation** object collection.</span></span>                                        |
| [<span data-ttu-id="f4a4b-177">Criar skillProficiency</span><span class="sxs-lookup"><span data-stu-id="f4a4b-177">Create skillProficiency</span></span>](../api/profile-post-skills.md)                   | [<span data-ttu-id="f4a4b-178">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="f4a4b-178">skillProficiency</span></span>](skillproficiency.md)                        | <span data-ttu-id="f4a4b-179">Crie um novo **skillProficiency** postando na coleção de habilidades.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-179">Create a new **skillProficiency** by posting to the skills collection.</span></span>                   |
| [<span data-ttu-id="f4a4b-180">Listar qualificações</span><span class="sxs-lookup"><span data-stu-id="f4a4b-180">List skills</span></span>](../api/profile-list-skills.md)                               | <span data-ttu-id="f4a4b-181">coleção [skillProficiency](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-181">[skillProficiency](skillproficiency.md) collection</span></span>             | <span data-ttu-id="f4a4b-182">Obtenha uma coleção de objetos **skillProficiency** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-182">Get a **skillProficiency** object collection.</span></span>                                            |
| [<span data-ttu-id="f4a4b-183">Criar conta da</span><span class="sxs-lookup"><span data-stu-id="f4a4b-183">Create webAccount</span></span>](../api/profile-post-webaccounts.md)                    | [<span data-ttu-id="f4a4b-184">conta da</span><span class="sxs-lookup"><span data-stu-id="f4a4b-184">webAccount</span></span>](webaccount.md)                                    | <span data-ttu-id="f4a4b-185">Crie uma nova **conta da webaccount** postando na coleção webaccounts.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-185">Create a new **webAccount** by posting to the webAccounts collection.</span></span>                    |
| [<span data-ttu-id="f4a4b-186">Listar contas da webaccount</span><span class="sxs-lookup"><span data-stu-id="f4a4b-186">List webAccounts</span></span>](../api/profile-list-webaccounts.md)                     | <span data-ttu-id="f4a4b-187">coleção [Webaccount](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-187">[webAccount](webaccount.md) collection</span></span>                         | <span data-ttu-id="f4a4b-188">Obtenha uma coleção de objetos **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-188">Get a **webAccount** object collection.</span></span>                                                  |
| [<span data-ttu-id="f4a4b-189">Criar personWebsite</span><span class="sxs-lookup"><span data-stu-id="f4a4b-189">Create personWebsite</span></span>](../api/profile-post-websites.md)                    | [<span data-ttu-id="f4a4b-190">personWebsite</span><span class="sxs-lookup"><span data-stu-id="f4a4b-190">personWebsite</span></span>](personwebsite.md)                              | <span data-ttu-id="f4a4b-191">Crie um novo **personWebsite** postando na coleção sites.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-191">Create a new **personWebsite** by posting to the websites collection.</span></span>                    |
| [<span data-ttu-id="f4a4b-192">Listar sites</span><span class="sxs-lookup"><span data-stu-id="f4a4b-192">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="f4a4b-193">coleção [personWebsite](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-193">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="f4a4b-194">Obtenha uma coleção de objetos **personWebsite** .</span><span class="sxs-lookup"><span data-stu-id="f4a4b-194">Get a **personWebsite** object collection.</span></span>                                               |

## <a name="properties"></a><span data-ttu-id="f4a4b-195">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4a4b-195">Properties</span></span>

| <span data-ttu-id="f4a4b-196">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4a4b-196">Property</span></span>     | <span data-ttu-id="f4a4b-197">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4a4b-197">Type</span></span>        | <span data-ttu-id="f4a4b-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4a4b-198">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4a4b-199">id</span><span class="sxs-lookup"><span data-stu-id="f4a4b-199">id</span></span>            |<span data-ttu-id="f4a4b-200">String</span><span class="sxs-lookup"><span data-stu-id="f4a4b-200">String</span></span>       | <span data-ttu-id="f4a4b-201">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-201">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="f4a4b-202">Relações</span><span class="sxs-lookup"><span data-stu-id="f4a4b-202">Relationships</span></span>

| <span data-ttu-id="f4a4b-203">Relação</span><span class="sxs-lookup"><span data-stu-id="f4a4b-203">Relationship</span></span>          | <span data-ttu-id="f4a4b-204">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4a4b-204">Type</span></span>                                                         | <span data-ttu-id="f4a4b-205">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4a4b-205">Description</span></span>         |
|:----------------------|:-------------------------------------------------------------|:--------------------|
|<span data-ttu-id="f4a4b-206">Count</span><span class="sxs-lookup"><span data-stu-id="f4a4b-206">account</span></span>                |<span data-ttu-id="f4a4b-207">coleção [userAccountInformation](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-207">[userAccountInformation](useraccountinformation.md) collection</span></span>| <span data-ttu-id="f4a4b-208">Representa informações especificamente associadas à conta de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-208">Represents information specifically tied to a user's account.</span></span> <span data-ttu-id="f4a4b-209">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-209">Read-only.</span></span> <span data-ttu-id="f4a4b-210">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-210">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-211">datas especiais</span><span class="sxs-lookup"><span data-stu-id="f4a4b-211">anniversaries</span></span>          |<span data-ttu-id="f4a4b-212">coleção [personAnniversary](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-212">[personAnniversary](personanniversary.md) collection</span></span>          | <span data-ttu-id="f4a4b-213">Representa os detalhes de datas significativas associadas a uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-213">Represents the details of meaningful dates associated with a person.</span></span> <span data-ttu-id="f4a4b-214">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-214">Read-only.</span></span> <span data-ttu-id="f4a4b-215">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-215">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-216">educationalActivities</span><span class="sxs-lookup"><span data-stu-id="f4a4b-216">educationalActivities</span></span>  |<span data-ttu-id="f4a4b-217">coleção [educationalActivity](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-217">[educationalActivity](educationalactivity.md) collection</span></span>      | <span data-ttu-id="f4a4b-218">Representa os dados que um usuário forneceu relacionados ao Undergraduate, graduado, dograduação ou outras atividades educacionais.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-218">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span> <span data-ttu-id="f4a4b-219">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-219">Read-only.</span></span> <span data-ttu-id="f4a4b-220">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-220">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-221">email</span><span class="sxs-lookup"><span data-stu-id="f4a4b-221">emails</span></span>                 |<span data-ttu-id="f4a4b-222">coleção [email](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-222">[itemEmail](itememail.md) collection</span></span>                          | <span data-ttu-id="f4a4b-223">Representa informações detalhadas sobre endereços de email associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-223">Represents detailed information about email addresses associated with the user.</span></span> <span data-ttu-id="f4a4b-224">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-224">Read-only.</span></span> <span data-ttu-id="f4a4b-225">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-225">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-226">interests</span><span class="sxs-lookup"><span data-stu-id="f4a4b-226">interests</span></span>              |<span data-ttu-id="f4a4b-227">coleção [personInterest](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-227">[personInterest](personinterest.md) collection</span></span>                | <span data-ttu-id="f4a4b-228">Fornece informações detalhadas sobre os interesses que o usuário tenha associado a si mesmos em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-228">Provides detailed information about interests the user has associated with themselves in various services.</span></span> <span data-ttu-id="f4a4b-229">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-229">Read-only.</span></span> <span data-ttu-id="f4a4b-230">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-230">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-231">Idiomas</span><span class="sxs-lookup"><span data-stu-id="f4a4b-231">languages</span></span>              |<span data-ttu-id="f4a4b-232">coleção [languageProficiency](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-232">[languageProficiency](languageproficiency.md) collection</span></span>      | <span data-ttu-id="f4a4b-233">Representa informações detalhadas sobre os idiomas que um usuário adicionou ao perfil.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-233">Represents detailed information about languages that a user has added to their profile.</span></span> <span data-ttu-id="f4a4b-234">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-234">Read-only.</span></span> <span data-ttu-id="f4a4b-235">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-235">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-236">telefones</span><span class="sxs-lookup"><span data-stu-id="f4a4b-236">phones</span></span>                 |<span data-ttu-id="f4a4b-237">coleção [Multiphone](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-237">[itemPhone](itemphone.md) collection</span></span>                          | <span data-ttu-id="f4a4b-238">Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-238">Represents detailed information about phone numbers associated with a user in various services.</span></span> <span data-ttu-id="f4a4b-239">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-239">Read-only.</span></span> <span data-ttu-id="f4a4b-240">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-240">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-241">as</span><span class="sxs-lookup"><span data-stu-id="f4a4b-241">positions</span></span>              |<span data-ttu-id="f4a4b-242">coleção [workPosition](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-242">[workPosition](workposition.md) collection</span></span>                    | <span data-ttu-id="f4a4b-243">Representa informações detalhadas sobre posições de trabalho associadas ao perfil de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-243">Represents detailed information about work positions associated with a user's profile.</span></span> <span data-ttu-id="f4a4b-244">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-244">Read-only.</span></span> <span data-ttu-id="f4a4b-245">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-245">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-246">Projetos</span><span class="sxs-lookup"><span data-stu-id="f4a4b-246">projects</span></span>               |<span data-ttu-id="f4a4b-247">coleção [projectParticipation](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-247">[projectParticipation](projectparticipation.md) collection</span></span>    | <span data-ttu-id="f4a4b-248">Representa informações detalhadas sobre os projetos associados a um usuário.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-248">Represents detailed information about projects associated with a user.</span></span> <span data-ttu-id="f4a4b-249">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-249">Read-only.</span></span> <span data-ttu-id="f4a4b-250">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-250">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-251">skills</span><span class="sxs-lookup"><span data-stu-id="f4a4b-251">skills</span></span>                 |<span data-ttu-id="f4a4b-252">coleção [skillProficiency](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-252">[skillProficiency](skillproficiency.md) collection</span></span>            | <span data-ttu-id="f4a4b-253">Representa informações detalhadas sobre as habilidades associadas a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-253">Represents detailed information about skills associated with a user in various services.</span></span> <span data-ttu-id="f4a4b-254">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-254">Read-only.</span></span> <span data-ttu-id="f4a4b-255">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-255">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-256">contas da</span><span class="sxs-lookup"><span data-stu-id="f4a4b-256">webAccounts</span></span>            |<span data-ttu-id="f4a4b-257">coleção [Webaccount](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-257">[webAccount](webaccount.md) collection</span></span>                        | <span data-ttu-id="f4a4b-258">Representa contas da Web que o usuário indicou que usa ou adicionou ao perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-258">Represents web accounts the user has indicated they use or has added to their user profile.</span></span> <span data-ttu-id="f4a4b-259">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-259">Read-only.</span></span> <span data-ttu-id="f4a4b-260">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-260">Nullable.</span></span>|
|<span data-ttu-id="f4a4b-261">websites</span><span class="sxs-lookup"><span data-stu-id="f4a4b-261">websites</span></span>               |<span data-ttu-id="f4a4b-262">coleção [personWebsite](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="f4a4b-262">[personWebsite](personwebsite.md) collection</span></span>                  | <span data-ttu-id="f4a4b-263">Representa informações detalhadas sobre sites associados a um usuário em vários serviços.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-263">Represents detailed information about websites associated with a user in various services.</span></span> <span data-ttu-id="f4a4b-264">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-264">Read-only.</span></span> <span data-ttu-id="f4a4b-265">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-265">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4a4b-266">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4a4b-266">JSON representation</span></span>

<span data-ttu-id="f4a4b-267">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4a4b-267">The following is a JSON representation of the resource.</span></span>

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
