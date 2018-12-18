---
title: Atualizar contato
description: Atualize as propriedades de um objeto contact.
author: angelgolfer-ms
ms.openlocfilehash: 386f0d3f7673733de805893e16ab049d85d120a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351230"
---
# <a name="update-contact"></a><span data-ttu-id="60c89-103">Atualizar contato</span><span class="sxs-lookup"><span data-stu-id="60c89-103">Update contact</span></span>

<span data-ttu-id="60c89-104">Atualize as propriedades de um objeto contact.</span><span class="sxs-lookup"><span data-stu-id="60c89-104">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="60c89-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="60c89-105">Permissions</span></span>
<span data-ttu-id="60c89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60c89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60c89-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60c89-108">Permission type</span></span>      | <span data-ttu-id="60c89-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60c89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60c89-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60c89-110">Delegated (work or school account)</span></span> | <span data-ttu-id="60c89-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60c89-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="60c89-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60c89-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60c89-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60c89-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="60c89-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60c89-114">Application</span></span> | <span data-ttu-id="60c89-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60c89-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="60c89-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60c89-116">HTTP request</span></span>
<span data-ttu-id="60c89-117"><!-- { "blockType": "ignored" } -->Um [contato](../resources/contact.md) do padrão de um usuário [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="60c89-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="60c89-118">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="60c89-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="60c89-p102">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="60c89-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="60c89-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60c89-121">Request headers</span></span>
| <span data-ttu-id="60c89-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60c89-122">Header</span></span>       | <span data-ttu-id="60c89-123">Valor</span><span class="sxs-lookup"><span data-stu-id="60c89-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="60c89-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="60c89-124">Authorization</span></span>  | <span data-ttu-id="60c89-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60c89-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="60c89-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60c89-127">Content-Type</span></span>  | <span data-ttu-id="60c89-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60c89-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="60c89-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60c89-130">Request body</span></span>
<span data-ttu-id="60c89-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="60c89-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="60c89-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60c89-134">Property</span></span>     | <span data-ttu-id="60c89-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="60c89-135">Type</span></span>   |<span data-ttu-id="60c89-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="60c89-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60c89-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="60c89-137">assistantName</span></span>|<span data-ttu-id="60c89-138">String</span><span class="sxs-lookup"><span data-stu-id="60c89-138">String</span></span>|<span data-ttu-id="60c89-139">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="60c89-140">birthday</span><span class="sxs-lookup"><span data-stu-id="60c89-140">birthday</span></span>|<span data-ttu-id="60c89-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60c89-141">DateTimeOffset</span></span>|<span data-ttu-id="60c89-142">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-142">The contact's birthday.</span></span>|
|<span data-ttu-id="60c89-143">businessAddress</span><span class="sxs-lookup"><span data-stu-id="60c89-143">businessAddress</span></span>|[<span data-ttu-id="60c89-144">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="60c89-144">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="60c89-145">O endereço comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-145">The contact's business address.</span></span>|
|<span data-ttu-id="60c89-146">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="60c89-146">businessHomePage</span></span>|<span data-ttu-id="60c89-147">String</span><span class="sxs-lookup"><span data-stu-id="60c89-147">String</span></span>|<span data-ttu-id="60c89-148">A home page comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-148">The business home page of the contact.</span></span>|
|<span data-ttu-id="60c89-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="60c89-149">businessPhones</span></span>|<span data-ttu-id="60c89-150">String</span><span class="sxs-lookup"><span data-stu-id="60c89-150">String</span></span>|<span data-ttu-id="60c89-151">Os números de telefone comerciais do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-151">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="60c89-152">categories</span><span class="sxs-lookup"><span data-stu-id="60c89-152">categories</span></span>|<span data-ttu-id="60c89-153">String</span><span class="sxs-lookup"><span data-stu-id="60c89-153">String</span></span>|<span data-ttu-id="60c89-154">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-154">The categories associated with the contact.</span></span>|
|<span data-ttu-id="60c89-155">children</span><span class="sxs-lookup"><span data-stu-id="60c89-155">children</span></span>|<span data-ttu-id="60c89-156">String</span><span class="sxs-lookup"><span data-stu-id="60c89-156">String</span></span>|<span data-ttu-id="60c89-157">Os nomes dos filhos do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-157">The names of the contact's children.</span></span>|
|<span data-ttu-id="60c89-158">nomeDaEmpresa</span><span class="sxs-lookup"><span data-stu-id="60c89-158">companyName</span></span>|<span data-ttu-id="60c89-159">String</span><span class="sxs-lookup"><span data-stu-id="60c89-159">String</span></span>|<span data-ttu-id="60c89-160">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-160">The name of the contact's company.</span></span>|
|<span data-ttu-id="60c89-161">departamento</span><span class="sxs-lookup"><span data-stu-id="60c89-161">department</span></span>|<span data-ttu-id="60c89-162">String</span><span class="sxs-lookup"><span data-stu-id="60c89-162">String</span></span>|<span data-ttu-id="60c89-163">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-163">The contact's department.</span></span>|
|<span data-ttu-id="60c89-164">displayName</span><span class="sxs-lookup"><span data-stu-id="60c89-164">displayName</span></span>|<span data-ttu-id="60c89-165">String</span><span class="sxs-lookup"><span data-stu-id="60c89-165">String</span></span>|<span data-ttu-id="60c89-166">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-166">The contact's display name.</span></span> <span data-ttu-id="60c89-167">Observe que as atualizações posteriores a outras propriedades podem causar um valor gerado automaticamente substituir o valor displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="60c89-167">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="60c89-168">Para preservar a um valor pré-existente, sempre incluí-lo como displayName em uma operação de atualização.</span><span class="sxs-lookup"><span data-stu-id="60c89-168">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="60c89-169">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="60c89-169">emailAddresses</span></span>|<span data-ttu-id="60c89-170">Coleção [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="60c89-170">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="60c89-171">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-171">The contact's email addresses.</span></span>|
|<span data-ttu-id="60c89-172">fileAs</span><span class="sxs-lookup"><span data-stu-id="60c89-172">fileAs</span></span>|<span data-ttu-id="60c89-173">String</span><span class="sxs-lookup"><span data-stu-id="60c89-173">String</span></span>|<span data-ttu-id="60c89-174">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="60c89-174">The name the contact is filed under.</span></span>|
|<span data-ttu-id="60c89-175">generation</span><span class="sxs-lookup"><span data-stu-id="60c89-175">generation</span></span>|<span data-ttu-id="60c89-176">String</span><span class="sxs-lookup"><span data-stu-id="60c89-176">String</span></span>|<span data-ttu-id="60c89-177">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-177">The contact's generation.</span></span>|
|<span data-ttu-id="60c89-178">givenName</span><span class="sxs-lookup"><span data-stu-id="60c89-178">givenName</span></span>|<span data-ttu-id="60c89-179">String</span><span class="sxs-lookup"><span data-stu-id="60c89-179">String</span></span>|<span data-ttu-id="60c89-180">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-180">The contact's given name.</span></span>|
|<span data-ttu-id="60c89-181">homeAddress</span><span class="sxs-lookup"><span data-stu-id="60c89-181">homeAddress</span></span>|[<span data-ttu-id="60c89-182">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="60c89-182">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="60c89-183">O endereço residencial do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-183">The contact's home address.</span></span>|
|<span data-ttu-id="60c89-184">homePhones</span><span class="sxs-lookup"><span data-stu-id="60c89-184">homePhones</span></span>|<span data-ttu-id="60c89-185">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="60c89-185">String collection</span></span>|<span data-ttu-id="60c89-186">Os números de telefone residenciais do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-186">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="60c89-187">imAddresses</span><span class="sxs-lookup"><span data-stu-id="60c89-187">imAddresses</span></span>|<span data-ttu-id="60c89-188">String</span><span class="sxs-lookup"><span data-stu-id="60c89-188">String</span></span>|<span data-ttu-id="60c89-189">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-189">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="60c89-190">initials</span><span class="sxs-lookup"><span data-stu-id="60c89-190">initials</span></span>|<span data-ttu-id="60c89-191">String</span><span class="sxs-lookup"><span data-stu-id="60c89-191">String</span></span>|<span data-ttu-id="60c89-192">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-192">The contact's initials.</span></span>|
|<span data-ttu-id="60c89-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="60c89-193">jobTitle</span></span>|<span data-ttu-id="60c89-194">String</span><span class="sxs-lookup"><span data-stu-id="60c89-194">String</span></span>|<span data-ttu-id="60c89-195">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-195">The contact’s job title.</span></span>|
|<span data-ttu-id="60c89-196">manager</span><span class="sxs-lookup"><span data-stu-id="60c89-196">manager</span></span>|<span data-ttu-id="60c89-197">String</span><span class="sxs-lookup"><span data-stu-id="60c89-197">String</span></span>|<span data-ttu-id="60c89-198">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-198">The name of the contact's manager.</span></span>
|<span data-ttu-id="60c89-199">middleName</span><span class="sxs-lookup"><span data-stu-id="60c89-199">middleName</span></span>|<span data-ttu-id="60c89-200">String</span><span class="sxs-lookup"><span data-stu-id="60c89-200">String</span></span>|<span data-ttu-id="60c89-201">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-201">The contact's middle name.</span></span>|
|<span data-ttu-id="60c89-202">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="60c89-202">mobilePhone</span></span>|<span data-ttu-id="60c89-203">String</span><span class="sxs-lookup"><span data-stu-id="60c89-203">String</span></span>|<span data-ttu-id="60c89-204">O número de celular do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-204">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="60c89-205">nickName</span><span class="sxs-lookup"><span data-stu-id="60c89-205">nickName</span></span>|<span data-ttu-id="60c89-206">String</span><span class="sxs-lookup"><span data-stu-id="60c89-206">String</span></span>|<span data-ttu-id="60c89-207">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-207">The contact's nickname.</span></span>|
|<span data-ttu-id="60c89-208">officeLocation</span><span class="sxs-lookup"><span data-stu-id="60c89-208">officeLocation</span></span>|<span data-ttu-id="60c89-209">String</span><span class="sxs-lookup"><span data-stu-id="60c89-209">String</span></span>|<span data-ttu-id="60c89-210">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-210">The location of the contact's office.</span></span>|
|<span data-ttu-id="60c89-211">otherAddress</span><span class="sxs-lookup"><span data-stu-id="60c89-211">otherAddress</span></span>|[<span data-ttu-id="60c89-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="60c89-212">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="60c89-213">Outros endereços do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-213">Other addresses for the contact.</span></span>|
|<span data-ttu-id="60c89-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="60c89-214">parentFolderId</span></span>|<span data-ttu-id="60c89-215">String</span><span class="sxs-lookup"><span data-stu-id="60c89-215">String</span></span>|<span data-ttu-id="60c89-216">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-216">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="60c89-217">personalNotes</span><span class="sxs-lookup"><span data-stu-id="60c89-217">personalNotes</span></span>|<span data-ttu-id="60c89-218">String</span><span class="sxs-lookup"><span data-stu-id="60c89-218">String</span></span>|<span data-ttu-id="60c89-219">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-219">The user's notes about the contact.</span></span>|
|<span data-ttu-id="60c89-220">profession</span><span class="sxs-lookup"><span data-stu-id="60c89-220">profession</span></span>|<span data-ttu-id="60c89-221">String</span><span class="sxs-lookup"><span data-stu-id="60c89-221">String</span></span>|<span data-ttu-id="60c89-222">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-222">The contact's profession.</span></span>|
|<span data-ttu-id="60c89-223">spouseName</span><span class="sxs-lookup"><span data-stu-id="60c89-223">spouseName</span></span>|<span data-ttu-id="60c89-224">String</span><span class="sxs-lookup"><span data-stu-id="60c89-224">String</span></span>|<span data-ttu-id="60c89-225">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-225">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="60c89-226">surname</span><span class="sxs-lookup"><span data-stu-id="60c89-226">surname</span></span>|<span data-ttu-id="60c89-227">String</span><span class="sxs-lookup"><span data-stu-id="60c89-227">String</span></span>|<span data-ttu-id="60c89-228">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-228">The contact's surname.</span></span>|
|<span data-ttu-id="60c89-229">title</span><span class="sxs-lookup"><span data-stu-id="60c89-229">title</span></span>|<span data-ttu-id="60c89-230">String</span><span class="sxs-lookup"><span data-stu-id="60c89-230">String</span></span>|<span data-ttu-id="60c89-231">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="60c89-231">The contact's title.</span></span>|
|<span data-ttu-id="60c89-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="60c89-232">yomiCompanyName</span></span>|<span data-ttu-id="60c89-233">String</span><span class="sxs-lookup"><span data-stu-id="60c89-233">String</span></span>|<span data-ttu-id="60c89-p107">O nome de empresa japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="60c89-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="60c89-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="60c89-236">yomiGivenName</span></span>|<span data-ttu-id="60c89-237">String</span><span class="sxs-lookup"><span data-stu-id="60c89-237">String</span></span>|<span data-ttu-id="60c89-p108">O nome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="60c89-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="60c89-240">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="60c89-240">yomiSurname</span></span>|<span data-ttu-id="60c89-241">String</span><span class="sxs-lookup"><span data-stu-id="60c89-241">String</span></span>|<span data-ttu-id="60c89-p109">O sobrenome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="60c89-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="60c89-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="60c89-244">Response</span></span>

<span data-ttu-id="60c89-245">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60c89-245">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60c89-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60c89-246">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60c89-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60c89-247">Request</span></span>
<span data-ttu-id="60c89-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60c89-248">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contacts/{id}
Content-type: application/json
Content-length: 1977

{
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "birthday": "1974-07-22"
}
```
##### <a name="response"></a><span data-ttu-id="60c89-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="60c89-249">Response</span></span>
<span data-ttu-id="60c89-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60c89-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "https://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98121"
  },
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
