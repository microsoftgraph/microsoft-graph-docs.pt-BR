---
title: Atualizar contato
description: Atualize as propriedades de um objeto contact.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4e26fb6521c3f9bcd6672da4241a727b3680aab1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518291"
---
# <a name="update-contact"></a><span data-ttu-id="0c33b-103">Atualizar contato</span><span class="sxs-lookup"><span data-stu-id="0c33b-103">Update contact</span></span>

<span data-ttu-id="0c33b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c33b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0c33b-105">Atualize as propriedades de um objeto contact.</span><span class="sxs-lookup"><span data-stu-id="0c33b-105">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0c33b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c33b-106">Permissions</span></span>
<span data-ttu-id="0c33b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c33b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c33b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c33b-109">Permission type</span></span>      | <span data-ttu-id="0c33b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c33b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c33b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c33b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0c33b-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c33b-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0c33b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c33b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c33b-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c33b-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0c33b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c33b-115">Application</span></span> | <span data-ttu-id="0c33b-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c33b-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c33b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c33b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0c33b-118">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="0c33b-118">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="0c33b-119">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="0c33b-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="0c33b-p102">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="0c33b-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0c33b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c33b-122">Request headers</span></span>
| <span data-ttu-id="0c33b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c33b-123">Header</span></span>       | <span data-ttu-id="0c33b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0c33b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c33b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c33b-125">Authorization</span></span>  | <span data-ttu-id="0c33b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c33b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0c33b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c33b-128">Content-Type</span></span>  | <span data-ttu-id="0c33b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c33b-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c33b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c33b-131">Request body</span></span>
<span data-ttu-id="0c33b-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0c33b-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0c33b-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c33b-135">Property</span></span>     | <span data-ttu-id="0c33b-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c33b-136">Type</span></span>   |<span data-ttu-id="0c33b-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c33b-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c33b-138">assistantName</span><span class="sxs-lookup"><span data-stu-id="0c33b-138">assistantName</span></span>|<span data-ttu-id="0c33b-139">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-139">String</span></span>|<span data-ttu-id="0c33b-140">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-140">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="0c33b-141">birthday</span><span class="sxs-lookup"><span data-stu-id="0c33b-141">birthday</span></span>|<span data-ttu-id="0c33b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c33b-142">DateTimeOffset</span></span>|<span data-ttu-id="0c33b-143">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-143">The contact's birthday.</span></span>|
|<span data-ttu-id="0c33b-144">businessAddress</span><span class="sxs-lookup"><span data-stu-id="0c33b-144">businessAddress</span></span>|[<span data-ttu-id="0c33b-145">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="0c33b-145">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="0c33b-146">O endereço comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-146">The contact's business address.</span></span>|
|<span data-ttu-id="0c33b-147">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="0c33b-147">businessHomePage</span></span>|<span data-ttu-id="0c33b-148">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-148">String</span></span>|<span data-ttu-id="0c33b-149">A home page comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-149">The business home page of the contact.</span></span>|
|<span data-ttu-id="0c33b-150">businessPhones</span><span class="sxs-lookup"><span data-stu-id="0c33b-150">businessPhones</span></span>|<span data-ttu-id="0c33b-151">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-151">String</span></span>|<span data-ttu-id="0c33b-152">Os números de telefone comerciais do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-152">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="0c33b-153">categories</span><span class="sxs-lookup"><span data-stu-id="0c33b-153">categories</span></span>|<span data-ttu-id="0c33b-154">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-154">String</span></span>|<span data-ttu-id="0c33b-155">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-155">The categories associated with the contact.</span></span>|
|<span data-ttu-id="0c33b-156">children</span><span class="sxs-lookup"><span data-stu-id="0c33b-156">children</span></span>|<span data-ttu-id="0c33b-157">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-157">String</span></span>|<span data-ttu-id="0c33b-158">Os nomes dos filhos do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-158">The names of the contact's children.</span></span>|
|<span data-ttu-id="0c33b-159">nomeDaEmpresa</span><span class="sxs-lookup"><span data-stu-id="0c33b-159">companyName</span></span>|<span data-ttu-id="0c33b-160">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-160">String</span></span>|<span data-ttu-id="0c33b-161">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-161">The name of the contact's company.</span></span>|
|<span data-ttu-id="0c33b-162">department</span><span class="sxs-lookup"><span data-stu-id="0c33b-162">department</span></span>|<span data-ttu-id="0c33b-163">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-163">String</span></span>|<span data-ttu-id="0c33b-164">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-164">The contact's department.</span></span>|
|<span data-ttu-id="0c33b-165">displayName</span><span class="sxs-lookup"><span data-stu-id="0c33b-165">displayName</span></span>|<span data-ttu-id="0c33b-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c33b-166">String</span></span>|<span data-ttu-id="0c33b-167">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-167">The contact's display name.</span></span> <span data-ttu-id="0c33b-168">Observe que atualizações posteriores em outras propriedades podem fazer com que um valor gerado automaticamente sobrescreva o valor de displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="0c33b-168">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="0c33b-169">Para preservar a um valor preexistente, inclua-o como o displayName na operação atualizar.</span><span class="sxs-lookup"><span data-stu-id="0c33b-169">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="0c33b-170">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="0c33b-170">emailAddresses</span></span>|<span data-ttu-id="0c33b-171">Coleção [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="0c33b-171">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="0c33b-172">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-172">The contact's email addresses.</span></span>|
|<span data-ttu-id="0c33b-173">fileAs</span><span class="sxs-lookup"><span data-stu-id="0c33b-173">fileAs</span></span>|<span data-ttu-id="0c33b-174">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-174">String</span></span>|<span data-ttu-id="0c33b-175">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="0c33b-175">The name the contact is filed under.</span></span>|
|<span data-ttu-id="0c33b-176">generation</span><span class="sxs-lookup"><span data-stu-id="0c33b-176">generation</span></span>|<span data-ttu-id="0c33b-177">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-177">String</span></span>|<span data-ttu-id="0c33b-178">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-178">The contact's generation.</span></span>|
|<span data-ttu-id="0c33b-179">givenName</span><span class="sxs-lookup"><span data-stu-id="0c33b-179">givenName</span></span>|<span data-ttu-id="0c33b-180">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-180">String</span></span>|<span data-ttu-id="0c33b-181">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-181">The contact's given name.</span></span>|
|<span data-ttu-id="0c33b-182">homeAddress</span><span class="sxs-lookup"><span data-stu-id="0c33b-182">homeAddress</span></span>|[<span data-ttu-id="0c33b-183">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="0c33b-183">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="0c33b-184">O endereço residencial do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-184">The contact's home address.</span></span>|
|<span data-ttu-id="0c33b-185">homePhones</span><span class="sxs-lookup"><span data-stu-id="0c33b-185">homePhones</span></span>|<span data-ttu-id="0c33b-186">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c33b-186">String collection</span></span>|<span data-ttu-id="0c33b-187">Os números de telefone residenciais do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-187">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="0c33b-188">imAddresses</span><span class="sxs-lookup"><span data-stu-id="0c33b-188">imAddresses</span></span>|<span data-ttu-id="0c33b-189">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-189">String</span></span>|<span data-ttu-id="0c33b-190">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-190">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="0c33b-191">initials</span><span class="sxs-lookup"><span data-stu-id="0c33b-191">initials</span></span>|<span data-ttu-id="0c33b-192">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-192">String</span></span>|<span data-ttu-id="0c33b-193">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-193">The contact's initials.</span></span>|
|<span data-ttu-id="0c33b-194">jobTitle</span><span class="sxs-lookup"><span data-stu-id="0c33b-194">jobTitle</span></span>|<span data-ttu-id="0c33b-195">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-195">String</span></span>|<span data-ttu-id="0c33b-196">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-196">The contact’s job title.</span></span>|
|<span data-ttu-id="0c33b-197">manager</span><span class="sxs-lookup"><span data-stu-id="0c33b-197">manager</span></span>|<span data-ttu-id="0c33b-198">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-198">String</span></span>|<span data-ttu-id="0c33b-199">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-199">The name of the contact's manager.</span></span>
|<span data-ttu-id="0c33b-200">middleName</span><span class="sxs-lookup"><span data-stu-id="0c33b-200">middleName</span></span>|<span data-ttu-id="0c33b-201">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-201">String</span></span>|<span data-ttu-id="0c33b-202">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-202">The contact's middle name.</span></span>|
|<span data-ttu-id="0c33b-203">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="0c33b-203">mobilePhone</span></span>|<span data-ttu-id="0c33b-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c33b-204">String</span></span>|<span data-ttu-id="0c33b-205">O número de celular do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-205">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="0c33b-206">nickName</span><span class="sxs-lookup"><span data-stu-id="0c33b-206">nickName</span></span>|<span data-ttu-id="0c33b-207">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-207">String</span></span>|<span data-ttu-id="0c33b-208">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-208">The contact's nickname.</span></span>|
|<span data-ttu-id="0c33b-209">officeLocation</span><span class="sxs-lookup"><span data-stu-id="0c33b-209">officeLocation</span></span>|<span data-ttu-id="0c33b-210">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-210">String</span></span>|<span data-ttu-id="0c33b-211">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-211">The location of the contact's office.</span></span>|
|<span data-ttu-id="0c33b-212">otherAddress</span><span class="sxs-lookup"><span data-stu-id="0c33b-212">otherAddress</span></span>|[<span data-ttu-id="0c33b-213">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="0c33b-213">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="0c33b-214">Outros endereços do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-214">Other addresses for the contact.</span></span>|
|<span data-ttu-id="0c33b-215">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="0c33b-215">parentFolderId</span></span>|<span data-ttu-id="0c33b-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c33b-216">String</span></span>|<span data-ttu-id="0c33b-217">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-217">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="0c33b-218">personalNotes</span><span class="sxs-lookup"><span data-stu-id="0c33b-218">personalNotes</span></span>|<span data-ttu-id="0c33b-219">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-219">String</span></span>|<span data-ttu-id="0c33b-220">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-220">The user's notes about the contact.</span></span>|
|<span data-ttu-id="0c33b-221">profession</span><span class="sxs-lookup"><span data-stu-id="0c33b-221">profession</span></span>|<span data-ttu-id="0c33b-222">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-222">String</span></span>|<span data-ttu-id="0c33b-223">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-223">The contact's profession.</span></span>|
|<span data-ttu-id="0c33b-224">spouseName</span><span class="sxs-lookup"><span data-stu-id="0c33b-224">spouseName</span></span>|<span data-ttu-id="0c33b-225">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-225">String</span></span>|<span data-ttu-id="0c33b-226">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-226">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="0c33b-227">surname</span><span class="sxs-lookup"><span data-stu-id="0c33b-227">surname</span></span>|<span data-ttu-id="0c33b-228">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-228">String</span></span>|<span data-ttu-id="0c33b-229">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-229">The contact's surname.</span></span>|
|<span data-ttu-id="0c33b-230">title</span><span class="sxs-lookup"><span data-stu-id="0c33b-230">title</span></span>|<span data-ttu-id="0c33b-231">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-231">String</span></span>|<span data-ttu-id="0c33b-232">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="0c33b-232">The contact's title.</span></span>|
|<span data-ttu-id="0c33b-233">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="0c33b-233">yomiCompanyName</span></span>|<span data-ttu-id="0c33b-234">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-234">String</span></span>|<span data-ttu-id="0c33b-p107">O nome de empresa japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="0c33b-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="0c33b-237">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="0c33b-237">yomiGivenName</span></span>|<span data-ttu-id="0c33b-238">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-238">String</span></span>|<span data-ttu-id="0c33b-p108">O nome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="0c33b-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="0c33b-241">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="0c33b-241">yomiSurname</span></span>|<span data-ttu-id="0c33b-242">String</span><span class="sxs-lookup"><span data-stu-id="0c33b-242">String</span></span>|<span data-ttu-id="0c33b-p109">O sobrenome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="0c33b-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="0c33b-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c33b-245">Response</span></span>

<span data-ttu-id="0c33b-246">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c33b-246">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0c33b-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c33b-247">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c33b-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c33b-248">Request</span></span>
<span data-ttu-id="0c33b-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c33b-249">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0c33b-250">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c33b-250">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0c33b-251">C#</span><span class="sxs-lookup"><span data-stu-id="0c33b-251">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c33b-252">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c33b-252">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c33b-253">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c33b-253">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c33b-254">Java</span><span class="sxs-lookup"><span data-stu-id="0c33b-254">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0c33b-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c33b-255">Response</span></span>
<span data-ttu-id="0c33b-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c33b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
