---
title: Atualizar contato
description: Atualize as propriedades do objeto de contato.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: e205421413dabeec7667252a05fc8398bdd48e36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809321"
---
# <a name="update-contact"></a><span data-ttu-id="e171a-103">Atualizar contato</span><span class="sxs-lookup"><span data-stu-id="e171a-103">Update contact</span></span>

> <span data-ttu-id="e171a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e171a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e171a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e171a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e171a-106">Atualize as propriedades do objeto de contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-106">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e171a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e171a-107">Permissions</span></span>
<span data-ttu-id="e171a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e171a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e171a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e171a-110">Permission type</span></span>      | <span data-ttu-id="e171a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e171a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e171a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e171a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e171a-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e171a-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e171a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e171a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e171a-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e171a-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e171a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e171a-116">Application</span></span> | <span data-ttu-id="e171a-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e171a-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e171a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e171a-118">HTTP request</span></span>
<span data-ttu-id="e171a-119"><!-- { "blockType": "ignored" } -->Um [contato](../resources/contact.md) de de padrão do usuário [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e171a-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="e171a-120">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="e171a-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="e171a-121">Um [contato](../resources/contact.md) contidos em uma pasta filho de um [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e171a-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="e171a-122">O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado no filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="e171a-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e171a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e171a-123">Request headers</span></span>
| <span data-ttu-id="e171a-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e171a-124">Header</span></span>       | <span data-ttu-id="e171a-125">Valor</span><span class="sxs-lookup"><span data-stu-id="e171a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e171a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e171a-126">Authorization</span></span>  | <span data-ttu-id="e171a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e171a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e171a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e171a-129">Content-Type</span></span>  | <span data-ttu-id="e171a-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e171a-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e171a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e171a-132">Request body</span></span>
<span data-ttu-id="e171a-p106">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e171a-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e171a-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e171a-136">Property</span></span>     | <span data-ttu-id="e171a-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="e171a-137">Type</span></span>   |<span data-ttu-id="e171a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="e171a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e171a-139">assistantName</span><span class="sxs-lookup"><span data-stu-id="e171a-139">assistantName</span></span>|<span data-ttu-id="e171a-140">String</span><span class="sxs-lookup"><span data-stu-id="e171a-140">String</span></span>|<span data-ttu-id="e171a-141">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-141">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="e171a-142">birthday</span><span class="sxs-lookup"><span data-stu-id="e171a-142">birthday</span></span>|<span data-ttu-id="e171a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e171a-143">DateTimeOffset</span></span>|<span data-ttu-id="e171a-144">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-144">The contact's birthday.</span></span>|
|<span data-ttu-id="e171a-145">categories</span><span class="sxs-lookup"><span data-stu-id="e171a-145">categories</span></span>|<span data-ttu-id="e171a-146">String</span><span class="sxs-lookup"><span data-stu-id="e171a-146">String</span></span>|<span data-ttu-id="e171a-147">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-147">The categories associated with the contact.</span></span>|
|<span data-ttu-id="e171a-148">children</span><span class="sxs-lookup"><span data-stu-id="e171a-148">children</span></span>|<span data-ttu-id="e171a-149">String</span><span class="sxs-lookup"><span data-stu-id="e171a-149">String</span></span>||
|<span data-ttu-id="e171a-150">companyName</span><span class="sxs-lookup"><span data-stu-id="e171a-150">companyName</span></span>|<span data-ttu-id="e171a-151">String</span><span class="sxs-lookup"><span data-stu-id="e171a-151">String</span></span>|<span data-ttu-id="e171a-152">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-152">The name of the contact's company.</span></span>|
|<span data-ttu-id="e171a-153">departamento</span><span class="sxs-lookup"><span data-stu-id="e171a-153">department</span></span>|<span data-ttu-id="e171a-154">String</span><span class="sxs-lookup"><span data-stu-id="e171a-154">String</span></span>|<span data-ttu-id="e171a-155">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-155">The contact's department.</span></span>|
|<span data-ttu-id="e171a-156">displayName</span><span class="sxs-lookup"><span data-stu-id="e171a-156">displayName</span></span>|<span data-ttu-id="e171a-157">String</span><span class="sxs-lookup"><span data-stu-id="e171a-157">String</span></span>|<span data-ttu-id="e171a-158">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-158">The contact's display name.</span></span> <span data-ttu-id="e171a-159">Observe que as atualizações posteriores a outras propriedades podem causar um valor gerado automaticamente substituir o valor displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="e171a-159">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="e171a-160">Para preservar a um valor pré-existente, sempre incluí-lo como displayName em uma operação de atualização.</span><span class="sxs-lookup"><span data-stu-id="e171a-160">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="e171a-161">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="e171a-161">emailAddresses</span></span>|<span data-ttu-id="e171a-162">coleção [typedEmailAddress](../resources/typedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="e171a-162">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="e171a-163">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-163">The contact's email addresses.</span></span>|
|<span data-ttu-id="e171a-164">fileAs</span><span class="sxs-lookup"><span data-stu-id="e171a-164">fileAs</span></span>|<span data-ttu-id="e171a-165">String</span><span class="sxs-lookup"><span data-stu-id="e171a-165">String</span></span>|<span data-ttu-id="e171a-166">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="e171a-166">The name the contact is filed under.</span></span>|
|<span data-ttu-id="e171a-167">gender</span><span class="sxs-lookup"><span data-stu-id="e171a-167">gender</span></span> |<span data-ttu-id="e171a-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e171a-168">String</span></span> |<span data-ttu-id="e171a-169">Gênero do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-169">The contact's gender.</span></span> |
|<span data-ttu-id="e171a-170">generation</span><span class="sxs-lookup"><span data-stu-id="e171a-170">generation</span></span>|<span data-ttu-id="e171a-171">String</span><span class="sxs-lookup"><span data-stu-id="e171a-171">String</span></span>|<span data-ttu-id="e171a-172">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-172">The contact's generation.</span></span>|
|<span data-ttu-id="e171a-173">givenName</span><span class="sxs-lookup"><span data-stu-id="e171a-173">givenName</span></span>|<span data-ttu-id="e171a-174">String</span><span class="sxs-lookup"><span data-stu-id="e171a-174">String</span></span>|<span data-ttu-id="e171a-175">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-175">The contact's given name.</span></span>|
|<span data-ttu-id="e171a-176">imAddresses</span><span class="sxs-lookup"><span data-stu-id="e171a-176">imAddresses</span></span>|<span data-ttu-id="e171a-177">String</span><span class="sxs-lookup"><span data-stu-id="e171a-177">String</span></span>|<span data-ttu-id="e171a-178">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-178">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="e171a-179">initials</span><span class="sxs-lookup"><span data-stu-id="e171a-179">initials</span></span>|<span data-ttu-id="e171a-180">String</span><span class="sxs-lookup"><span data-stu-id="e171a-180">String</span></span>|<span data-ttu-id="e171a-181">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-181">The contact's initials.</span></span>|
|<span data-ttu-id="e171a-182">jobTitle</span><span class="sxs-lookup"><span data-stu-id="e171a-182">jobTitle</span></span>|<span data-ttu-id="e171a-183">String</span><span class="sxs-lookup"><span data-stu-id="e171a-183">String</span></span>|<span data-ttu-id="e171a-184">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-184">The contact’s job title.</span></span>|
|<span data-ttu-id="e171a-185">manager</span><span class="sxs-lookup"><span data-stu-id="e171a-185">manager</span></span>|<span data-ttu-id="e171a-186">String</span><span class="sxs-lookup"><span data-stu-id="e171a-186">String</span></span>|<span data-ttu-id="e171a-187">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-187">The name of the contact's manager.</span></span>
|<span data-ttu-id="e171a-188">middleName</span><span class="sxs-lookup"><span data-stu-id="e171a-188">middleName</span></span>|<span data-ttu-id="e171a-189">String</span><span class="sxs-lookup"><span data-stu-id="e171a-189">String</span></span>|<span data-ttu-id="e171a-190">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-190">The contact's middle name.</span></span>|
|<span data-ttu-id="e171a-191">nickName</span><span class="sxs-lookup"><span data-stu-id="e171a-191">nickName</span></span>|<span data-ttu-id="e171a-192">String</span><span class="sxs-lookup"><span data-stu-id="e171a-192">String</span></span>|<span data-ttu-id="e171a-193">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-193">The contact's nickname.</span></span>|
|<span data-ttu-id="e171a-194">officeLocation</span><span class="sxs-lookup"><span data-stu-id="e171a-194">officeLocation</span></span>|<span data-ttu-id="e171a-195">String</span><span class="sxs-lookup"><span data-stu-id="e171a-195">String</span></span>|<span data-ttu-id="e171a-196">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-196">The location of the contact's office.</span></span>|
|<span data-ttu-id="e171a-197">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="e171a-197">parentFolderId</span></span>|<span data-ttu-id="e171a-198">String</span><span class="sxs-lookup"><span data-stu-id="e171a-198">String</span></span>|<span data-ttu-id="e171a-199">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-199">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="e171a-200">personalNotes</span><span class="sxs-lookup"><span data-stu-id="e171a-200">personalNotes</span></span>|<span data-ttu-id="e171a-201">String</span><span class="sxs-lookup"><span data-stu-id="e171a-201">String</span></span>|<span data-ttu-id="e171a-202">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-202">The user's notes about the contact.</span></span>|
|<span data-ttu-id="e171a-203">telefones</span><span class="sxs-lookup"><span data-stu-id="e171a-203">phones</span></span> |<span data-ttu-id="e171a-204">Coleção [phone](../resources/phone.md)</span><span class="sxs-lookup"><span data-stu-id="e171a-204">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="e171a-205">Números de telefone associados com o contato, por exemplo, telefone residencial, celular e telefone comercial.</span><span class="sxs-lookup"><span data-stu-id="e171a-205">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="e171a-206">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="e171a-206">postalAddresses</span></span> |<span data-ttu-id="e171a-207">coleção [physicalAddress](../resources/physicaladdress.md)</span><span class="sxs-lookup"><span data-stu-id="e171a-207">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="e171a-208">Endereços associados ao contato, por exemplo, início endereço e o endereço comercial.</span><span class="sxs-lookup"><span data-stu-id="e171a-208">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="e171a-209">profession</span><span class="sxs-lookup"><span data-stu-id="e171a-209">profession</span></span>|<span data-ttu-id="e171a-210">String</span><span class="sxs-lookup"><span data-stu-id="e171a-210">String</span></span>|<span data-ttu-id="e171a-211">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-211">The contact's profession.</span></span>|
|<span data-ttu-id="e171a-212">spouseName</span><span class="sxs-lookup"><span data-stu-id="e171a-212">spouseName</span></span>|<span data-ttu-id="e171a-213">String</span><span class="sxs-lookup"><span data-stu-id="e171a-213">String</span></span>|<span data-ttu-id="e171a-214">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-214">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="e171a-215">surname</span><span class="sxs-lookup"><span data-stu-id="e171a-215">surname</span></span>|<span data-ttu-id="e171a-216">String</span><span class="sxs-lookup"><span data-stu-id="e171a-216">String</span></span>|<span data-ttu-id="e171a-217">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-217">The contact's surname.</span></span>|
|<span data-ttu-id="e171a-218">title</span><span class="sxs-lookup"><span data-stu-id="e171a-218">title</span></span>|<span data-ttu-id="e171a-219">String</span><span class="sxs-lookup"><span data-stu-id="e171a-219">String</span></span>|<span data-ttu-id="e171a-220">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-220">The contact's title.</span></span>|
|<span data-ttu-id="e171a-221">websites</span><span class="sxs-lookup"><span data-stu-id="e171a-221">websites</span></span> |<span data-ttu-id="e171a-222">Coleção [website](../resources/website.md)</span><span class="sxs-lookup"><span data-stu-id="e171a-222">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="e171a-223">Sites da Web associados ao contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-223">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="e171a-224">weddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="e171a-224">weddingAnniversary</span></span> |<span data-ttu-id="e171a-225">Data</span><span class="sxs-lookup"><span data-stu-id="e171a-225">Date</span></span> |<span data-ttu-id="e171a-226">Aniversário de chá do contato.</span><span class="sxs-lookup"><span data-stu-id="e171a-226">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="e171a-227">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="e171a-227">yomiCompanyName</span></span>|<span data-ttu-id="e171a-228">String</span><span class="sxs-lookup"><span data-stu-id="e171a-228">String</span></span>|<span data-ttu-id="e171a-p108">O nome de empresa japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="e171a-p108">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="e171a-231">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="e171a-231">yomiGivenName</span></span>|<span data-ttu-id="e171a-232">String</span><span class="sxs-lookup"><span data-stu-id="e171a-232">String</span></span>|<span data-ttu-id="e171a-p109">O nome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="e171a-p109">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="e171a-235">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="e171a-235">yomiSurname</span></span>|<span data-ttu-id="e171a-236">String</span><span class="sxs-lookup"><span data-stu-id="e171a-236">String</span></span>|<span data-ttu-id="e171a-p110">O sobrenome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="e171a-p110">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="e171a-239">Desde que o recurso **Contatos** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância existente do **contato** .</span><span class="sxs-lookup"><span data-stu-id="e171a-239">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="e171a-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="e171a-240">Response</span></span>

<span data-ttu-id="e171a-241">Se tiver êxito, este método retornará um `200 OK` código de resposta e atualizadas, [entre em contato com](../resources/contact.md) o objeto no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e171a-241">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e171a-242">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e171a-242">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e171a-243">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e171a-243">Request</span></span>
<span data-ttu-id="e171a-244">O exemplo a seguir atualiza o endereço de email pessoal do contato especificado.</span><span class="sxs-lookup"><span data-stu-id="e171a-244">The following example updates the personal email address of the specified contact.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contacts/AAMkADh6v5AAAvgTCEAAA=
Content-type: application/json

{
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
          "address": "pavelb@fabrikam.onmicrosoft.com",
          "name": "Pavel Bansky",
          "type": "other",
          "otherLabel": "Volunteer work"
        }
    ]
}
```
##### <a name="response"></a><span data-ttu-id="e171a-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="e171a-245">Response</span></span>
<span data-ttu-id="e171a-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e171a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T20:26:23Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
            "type":"other",
            "otherLabel":"Volunteer work",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="e171a-249">Confira também</span><span class="sxs-lookup"><span data-stu-id="e171a-249">See also</span></span>

- [<span data-ttu-id="e171a-250">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="e171a-250">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e171a-251">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="e171a-251">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
