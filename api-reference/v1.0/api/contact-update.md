---
title: Atualizar contato
description: Atualize as propriedades de um objeto contact.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6b7643f411533dd554934d522e988d6dfcb49eb4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472766"
---
# <a name="update-contact"></a><span data-ttu-id="33b0a-103">Atualizar contato</span><span class="sxs-lookup"><span data-stu-id="33b0a-103">Update contact</span></span>

<span data-ttu-id="33b0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33b0a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33b0a-105">Atualize as propriedades de um objeto contact.</span><span class="sxs-lookup"><span data-stu-id="33b0a-105">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="33b0a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="33b0a-106">Permissions</span></span>
<span data-ttu-id="33b0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33b0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33b0a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33b0a-109">Permission type</span></span>      | <span data-ttu-id="33b0a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33b0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33b0a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33b0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33b0a-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33b0a-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="33b0a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33b0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33b0a-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33b0a-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="33b0a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33b0a-115">Application</span></span> | <span data-ttu-id="33b0a-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33b0a-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="33b0a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33b0a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="33b0a-118">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="33b0a-118">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="33b0a-119">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="33b0a-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="33b0a-p102">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="33b0a-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="33b0a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33b0a-122">Request headers</span></span>
| <span data-ttu-id="33b0a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33b0a-123">Header</span></span>       | <span data-ttu-id="33b0a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="33b0a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="33b0a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="33b0a-125">Authorization</span></span>  | <span data-ttu-id="33b0a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33b0a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="33b0a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33b0a-128">Content-Type</span></span>  | <span data-ttu-id="33b0a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33b0a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="33b0a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33b0a-131">Request body</span></span>
<span data-ttu-id="33b0a-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="33b0a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="33b0a-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33b0a-135">Property</span></span>     | <span data-ttu-id="33b0a-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="33b0a-136">Type</span></span>   |<span data-ttu-id="33b0a-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="33b0a-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33b0a-138">assistantName</span><span class="sxs-lookup"><span data-stu-id="33b0a-138">assistantName</span></span>|<span data-ttu-id="33b0a-139">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-139">String</span></span>|<span data-ttu-id="33b0a-140">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-140">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="33b0a-141">birthday</span><span class="sxs-lookup"><span data-stu-id="33b0a-141">birthday</span></span>|<span data-ttu-id="33b0a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33b0a-142">DateTimeOffset</span></span>|<span data-ttu-id="33b0a-143">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-143">The contact's birthday.</span></span>|
|<span data-ttu-id="33b0a-144">businessAddress</span><span class="sxs-lookup"><span data-stu-id="33b0a-144">businessAddress</span></span>|[<span data-ttu-id="33b0a-145">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="33b0a-145">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="33b0a-146">O endereço comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-146">The contact's business address.</span></span>|
|<span data-ttu-id="33b0a-147">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="33b0a-147">businessHomePage</span></span>|<span data-ttu-id="33b0a-148">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-148">String</span></span>|<span data-ttu-id="33b0a-149">A home page comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-149">The business home page of the contact.</span></span>|
|<span data-ttu-id="33b0a-150">businessPhones</span><span class="sxs-lookup"><span data-stu-id="33b0a-150">businessPhones</span></span>|<span data-ttu-id="33b0a-151">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-151">String</span></span>|<span data-ttu-id="33b0a-152">Os números de telefone comerciais do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-152">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="33b0a-153">categories</span><span class="sxs-lookup"><span data-stu-id="33b0a-153">categories</span></span>|<span data-ttu-id="33b0a-154">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-154">String</span></span>|<span data-ttu-id="33b0a-155">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-155">The categories associated with the contact.</span></span>|
|<span data-ttu-id="33b0a-156">children</span><span class="sxs-lookup"><span data-stu-id="33b0a-156">children</span></span>|<span data-ttu-id="33b0a-157">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-157">String</span></span>|<span data-ttu-id="33b0a-158">Os nomes dos filhos do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-158">The names of the contact's children.</span></span>|
|<span data-ttu-id="33b0a-159">nomeDaEmpresa</span><span class="sxs-lookup"><span data-stu-id="33b0a-159">companyName</span></span>|<span data-ttu-id="33b0a-160">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-160">String</span></span>|<span data-ttu-id="33b0a-161">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-161">The name of the contact's company.</span></span>|
|<span data-ttu-id="33b0a-162">department</span><span class="sxs-lookup"><span data-stu-id="33b0a-162">department</span></span>|<span data-ttu-id="33b0a-163">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-163">String</span></span>|<span data-ttu-id="33b0a-164">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-164">The contact's department.</span></span>|
|<span data-ttu-id="33b0a-165">displayName</span><span class="sxs-lookup"><span data-stu-id="33b0a-165">displayName</span></span>|<span data-ttu-id="33b0a-166">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-166">String</span></span>|<span data-ttu-id="33b0a-167">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-167">The contact's display name.</span></span> <span data-ttu-id="33b0a-168">Observe que atualizações posteriores em outras propriedades podem fazer com que um valor gerado automaticamente sobrescreva o valor de displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="33b0a-168">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="33b0a-169">Para preservar a um valor preexistente, inclua-o como o displayName na operação atualizar.</span><span class="sxs-lookup"><span data-stu-id="33b0a-169">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="33b0a-170">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="33b0a-170">emailAddresses</span></span>|<span data-ttu-id="33b0a-171">Coleção [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="33b0a-171">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="33b0a-172">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-172">The contact's email addresses.</span></span>|
|<span data-ttu-id="33b0a-173">fileAs</span><span class="sxs-lookup"><span data-stu-id="33b0a-173">fileAs</span></span>|<span data-ttu-id="33b0a-174">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-174">String</span></span>|<span data-ttu-id="33b0a-175">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="33b0a-175">The name the contact is filed under.</span></span>|
|<span data-ttu-id="33b0a-176">generation</span><span class="sxs-lookup"><span data-stu-id="33b0a-176">generation</span></span>|<span data-ttu-id="33b0a-177">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-177">String</span></span>|<span data-ttu-id="33b0a-178">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-178">The contact's generation.</span></span>|
|<span data-ttu-id="33b0a-179">givenName</span><span class="sxs-lookup"><span data-stu-id="33b0a-179">givenName</span></span>|<span data-ttu-id="33b0a-180">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-180">String</span></span>|<span data-ttu-id="33b0a-181">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-181">The contact's given name.</span></span>|
|<span data-ttu-id="33b0a-182">homeAddress</span><span class="sxs-lookup"><span data-stu-id="33b0a-182">homeAddress</span></span>|[<span data-ttu-id="33b0a-183">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="33b0a-183">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="33b0a-184">O endereço residencial do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-184">The contact's home address.</span></span>|
|<span data-ttu-id="33b0a-185">homePhones</span><span class="sxs-lookup"><span data-stu-id="33b0a-185">homePhones</span></span>|<span data-ttu-id="33b0a-186">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="33b0a-186">String collection</span></span>|<span data-ttu-id="33b0a-187">Os números de telefone residenciais do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-187">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="33b0a-188">imAddresses</span><span class="sxs-lookup"><span data-stu-id="33b0a-188">imAddresses</span></span>|<span data-ttu-id="33b0a-189">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-189">String</span></span>|<span data-ttu-id="33b0a-190">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-190">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="33b0a-191">initials</span><span class="sxs-lookup"><span data-stu-id="33b0a-191">initials</span></span>|<span data-ttu-id="33b0a-192">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-192">String</span></span>|<span data-ttu-id="33b0a-193">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-193">The contact's initials.</span></span>|
|<span data-ttu-id="33b0a-194">jobTitle</span><span class="sxs-lookup"><span data-stu-id="33b0a-194">jobTitle</span></span>|<span data-ttu-id="33b0a-195">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-195">String</span></span>|<span data-ttu-id="33b0a-196">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-196">The contact’s job title.</span></span>|
|<span data-ttu-id="33b0a-197">manager</span><span class="sxs-lookup"><span data-stu-id="33b0a-197">manager</span></span>|<span data-ttu-id="33b0a-198">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-198">String</span></span>|<span data-ttu-id="33b0a-199">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-199">The name of the contact's manager.</span></span>
|<span data-ttu-id="33b0a-200">middleName</span><span class="sxs-lookup"><span data-stu-id="33b0a-200">middleName</span></span>|<span data-ttu-id="33b0a-201">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-201">String</span></span>|<span data-ttu-id="33b0a-202">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-202">The contact's middle name.</span></span>|
|<span data-ttu-id="33b0a-203">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="33b0a-203">mobilePhone</span></span>|<span data-ttu-id="33b0a-204">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-204">String</span></span>|<span data-ttu-id="33b0a-205">O número de celular do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-205">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="33b0a-206">nickName</span><span class="sxs-lookup"><span data-stu-id="33b0a-206">nickName</span></span>|<span data-ttu-id="33b0a-207">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-207">String</span></span>|<span data-ttu-id="33b0a-208">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-208">The contact's nickname.</span></span>|
|<span data-ttu-id="33b0a-209">officeLocation</span><span class="sxs-lookup"><span data-stu-id="33b0a-209">officeLocation</span></span>|<span data-ttu-id="33b0a-210">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-210">String</span></span>|<span data-ttu-id="33b0a-211">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-211">The location of the contact's office.</span></span>|
|<span data-ttu-id="33b0a-212">otherAddress</span><span class="sxs-lookup"><span data-stu-id="33b0a-212">otherAddress</span></span>|[<span data-ttu-id="33b0a-213">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="33b0a-213">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="33b0a-214">Outros endereços do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-214">Other addresses for the contact.</span></span>|
|<span data-ttu-id="33b0a-215">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="33b0a-215">parentFolderId</span></span>|<span data-ttu-id="33b0a-216">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-216">String</span></span>|<span data-ttu-id="33b0a-217">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-217">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="33b0a-218">personalNotes</span><span class="sxs-lookup"><span data-stu-id="33b0a-218">personalNotes</span></span>|<span data-ttu-id="33b0a-219">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-219">String</span></span>|<span data-ttu-id="33b0a-220">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-220">The user's notes about the contact.</span></span>|
|<span data-ttu-id="33b0a-221">profession</span><span class="sxs-lookup"><span data-stu-id="33b0a-221">profession</span></span>|<span data-ttu-id="33b0a-222">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-222">String</span></span>|<span data-ttu-id="33b0a-223">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-223">The contact's profession.</span></span>|
|<span data-ttu-id="33b0a-224">spouseName</span><span class="sxs-lookup"><span data-stu-id="33b0a-224">spouseName</span></span>|<span data-ttu-id="33b0a-225">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-225">String</span></span>|<span data-ttu-id="33b0a-226">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-226">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="33b0a-227">surname</span><span class="sxs-lookup"><span data-stu-id="33b0a-227">surname</span></span>|<span data-ttu-id="33b0a-228">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-228">String</span></span>|<span data-ttu-id="33b0a-229">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-229">The contact's surname.</span></span>|
|<span data-ttu-id="33b0a-230">title</span><span class="sxs-lookup"><span data-stu-id="33b0a-230">title</span></span>|<span data-ttu-id="33b0a-231">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-231">String</span></span>|<span data-ttu-id="33b0a-232">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="33b0a-232">The contact's title.</span></span>|
|<span data-ttu-id="33b0a-233">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="33b0a-233">yomiCompanyName</span></span>|<span data-ttu-id="33b0a-234">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-234">String</span></span>|<span data-ttu-id="33b0a-p107">O nome de empresa japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="33b0a-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="33b0a-237">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="33b0a-237">yomiGivenName</span></span>|<span data-ttu-id="33b0a-238">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-238">String</span></span>|<span data-ttu-id="33b0a-p108">O nome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="33b0a-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="33b0a-241">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="33b0a-241">yomiSurname</span></span>|<span data-ttu-id="33b0a-242">String</span><span class="sxs-lookup"><span data-stu-id="33b0a-242">String</span></span>|<span data-ttu-id="33b0a-p109">O sobrenome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="33b0a-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="33b0a-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b0a-245">Response</span></span>

<span data-ttu-id="33b0a-246">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33b0a-246">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33b0a-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33b0a-247">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33b0a-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33b0a-248">Request</span></span>
<span data-ttu-id="33b0a-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33b0a-249">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33b0a-250">HTTP</span><span class="sxs-lookup"><span data-stu-id="33b0a-250">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="33b0a-251">C#</span><span class="sxs-lookup"><span data-stu-id="33b0a-251">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33b0a-252">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33b0a-252">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33b0a-253">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33b0a-253">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33b0a-254">Java</span><span class="sxs-lookup"><span data-stu-id="33b0a-254">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="33b0a-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b0a-255">Response</span></span>
<span data-ttu-id="33b0a-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33b0a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

