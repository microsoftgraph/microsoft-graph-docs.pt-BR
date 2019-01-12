---
title: Atualizar contato
description: Atualize as propriedades de um objeto contact.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 381aa191639e32677d4fccbf9e9f48c99f3d988f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927902"
---
# <a name="update-contact"></a><span data-ttu-id="3e80f-103">Atualizar contato</span><span class="sxs-lookup"><span data-stu-id="3e80f-103">Update contact</span></span>

<span data-ttu-id="3e80f-104">Atualize as propriedades de um objeto contact.</span><span class="sxs-lookup"><span data-stu-id="3e80f-104">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e80f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e80f-105">Permissions</span></span>
<span data-ttu-id="3e80f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e80f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e80f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e80f-108">Permission type</span></span>      | <span data-ttu-id="3e80f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e80f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e80f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e80f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e80f-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e80f-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3e80f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e80f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e80f-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e80f-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3e80f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e80f-114">Application</span></span> | <span data-ttu-id="3e80f-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e80f-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e80f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e80f-116">HTTP request</span></span>
<span data-ttu-id="3e80f-117"><!-- { "blockType": "ignored" } -->Um [contato](../resources/contact.md) do padrão de um usuário [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="3e80f-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="3e80f-118">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="3e80f-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="3e80f-p102">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="3e80f-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3e80f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e80f-121">Request headers</span></span>
| <span data-ttu-id="3e80f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e80f-122">Header</span></span>       | <span data-ttu-id="3e80f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3e80f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e80f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e80f-124">Authorization</span></span>  | <span data-ttu-id="3e80f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e80f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3e80f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e80f-127">Content-Type</span></span>  | <span data-ttu-id="3e80f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e80f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e80f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e80f-130">Request body</span></span>
<span data-ttu-id="3e80f-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3e80f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e80f-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e80f-134">Property</span></span>     | <span data-ttu-id="3e80f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e80f-135">Type</span></span>   |<span data-ttu-id="3e80f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e80f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e80f-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="3e80f-137">assistantName</span></span>|<span data-ttu-id="3e80f-138">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-138">String</span></span>|<span data-ttu-id="3e80f-139">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="3e80f-140">birthday</span><span class="sxs-lookup"><span data-stu-id="3e80f-140">birthday</span></span>|<span data-ttu-id="3e80f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e80f-141">DateTimeOffset</span></span>|<span data-ttu-id="3e80f-142">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-142">The contact's birthday.</span></span>|
|<span data-ttu-id="3e80f-143">businessAddress</span><span class="sxs-lookup"><span data-stu-id="3e80f-143">businessAddress</span></span>|[<span data-ttu-id="3e80f-144">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="3e80f-144">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="3e80f-145">O endereço comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-145">The contact's business address.</span></span>|
|<span data-ttu-id="3e80f-146">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="3e80f-146">businessHomePage</span></span>|<span data-ttu-id="3e80f-147">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-147">String</span></span>|<span data-ttu-id="3e80f-148">A home page comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-148">The business home page of the contact.</span></span>|
|<span data-ttu-id="3e80f-149">businessPhones</span><span class="sxs-lookup"><span data-stu-id="3e80f-149">businessPhones</span></span>|<span data-ttu-id="3e80f-150">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-150">String</span></span>|<span data-ttu-id="3e80f-151">Os números de telefone comerciais do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-151">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="3e80f-152">categories</span><span class="sxs-lookup"><span data-stu-id="3e80f-152">categories</span></span>|<span data-ttu-id="3e80f-153">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-153">String</span></span>|<span data-ttu-id="3e80f-154">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-154">The categories associated with the contact.</span></span>|
|<span data-ttu-id="3e80f-155">children</span><span class="sxs-lookup"><span data-stu-id="3e80f-155">children</span></span>|<span data-ttu-id="3e80f-156">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-156">String</span></span>|<span data-ttu-id="3e80f-157">Os nomes dos filhos do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-157">The names of the contact's children.</span></span>|
|<span data-ttu-id="3e80f-158">nomeDaEmpresa</span><span class="sxs-lookup"><span data-stu-id="3e80f-158">companyName</span></span>|<span data-ttu-id="3e80f-159">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-159">String</span></span>|<span data-ttu-id="3e80f-160">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-160">The name of the contact's company.</span></span>|
|<span data-ttu-id="3e80f-161">departamento</span><span class="sxs-lookup"><span data-stu-id="3e80f-161">department</span></span>|<span data-ttu-id="3e80f-162">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-162">String</span></span>|<span data-ttu-id="3e80f-163">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-163">The contact's department.</span></span>|
|<span data-ttu-id="3e80f-164">displayName</span><span class="sxs-lookup"><span data-stu-id="3e80f-164">displayName</span></span>|<span data-ttu-id="3e80f-165">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-165">String</span></span>|<span data-ttu-id="3e80f-166">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-166">The contact's display name.</span></span> <span data-ttu-id="3e80f-167">Observe que as atualizações posteriores a outras propriedades podem causar um valor gerado automaticamente substituir o valor displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="3e80f-167">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="3e80f-168">Para preservar a um valor pré-existente, sempre incluí-lo como displayName em uma operação de atualização.</span><span class="sxs-lookup"><span data-stu-id="3e80f-168">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="3e80f-169">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="3e80f-169">emailAddresses</span></span>|<span data-ttu-id="3e80f-170">Coleção [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="3e80f-170">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="3e80f-171">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-171">The contact's email addresses.</span></span>|
|<span data-ttu-id="3e80f-172">fileAs</span><span class="sxs-lookup"><span data-stu-id="3e80f-172">fileAs</span></span>|<span data-ttu-id="3e80f-173">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-173">String</span></span>|<span data-ttu-id="3e80f-174">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="3e80f-174">The name the contact is filed under.</span></span>|
|<span data-ttu-id="3e80f-175">generation</span><span class="sxs-lookup"><span data-stu-id="3e80f-175">generation</span></span>|<span data-ttu-id="3e80f-176">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-176">String</span></span>|<span data-ttu-id="3e80f-177">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-177">The contact's generation.</span></span>|
|<span data-ttu-id="3e80f-178">givenName</span><span class="sxs-lookup"><span data-stu-id="3e80f-178">givenName</span></span>|<span data-ttu-id="3e80f-179">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-179">String</span></span>|<span data-ttu-id="3e80f-180">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-180">The contact's given name.</span></span>|
|<span data-ttu-id="3e80f-181">homeAddress</span><span class="sxs-lookup"><span data-stu-id="3e80f-181">homeAddress</span></span>|[<span data-ttu-id="3e80f-182">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="3e80f-182">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="3e80f-183">O endereço residencial do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-183">The contact's home address.</span></span>|
|<span data-ttu-id="3e80f-184">homePhones</span><span class="sxs-lookup"><span data-stu-id="3e80f-184">homePhones</span></span>|<span data-ttu-id="3e80f-185">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e80f-185">String collection</span></span>|<span data-ttu-id="3e80f-186">Os números de telefone residenciais do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-186">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="3e80f-187">imAddresses</span><span class="sxs-lookup"><span data-stu-id="3e80f-187">imAddresses</span></span>|<span data-ttu-id="3e80f-188">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-188">String</span></span>|<span data-ttu-id="3e80f-189">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-189">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="3e80f-190">initials</span><span class="sxs-lookup"><span data-stu-id="3e80f-190">initials</span></span>|<span data-ttu-id="3e80f-191">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-191">String</span></span>|<span data-ttu-id="3e80f-192">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-192">The contact's initials.</span></span>|
|<span data-ttu-id="3e80f-193">jobTitle</span><span class="sxs-lookup"><span data-stu-id="3e80f-193">jobTitle</span></span>|<span data-ttu-id="3e80f-194">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-194">String</span></span>|<span data-ttu-id="3e80f-195">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-195">The contact’s job title.</span></span>|
|<span data-ttu-id="3e80f-196">manager</span><span class="sxs-lookup"><span data-stu-id="3e80f-196">manager</span></span>|<span data-ttu-id="3e80f-197">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-197">String</span></span>|<span data-ttu-id="3e80f-198">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-198">The name of the contact's manager.</span></span>
|<span data-ttu-id="3e80f-199">middleName</span><span class="sxs-lookup"><span data-stu-id="3e80f-199">middleName</span></span>|<span data-ttu-id="3e80f-200">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-200">String</span></span>|<span data-ttu-id="3e80f-201">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-201">The contact's middle name.</span></span>|
|<span data-ttu-id="3e80f-202">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="3e80f-202">mobilePhone</span></span>|<span data-ttu-id="3e80f-203">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-203">String</span></span>|<span data-ttu-id="3e80f-204">O número de celular do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-204">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="3e80f-205">nickName</span><span class="sxs-lookup"><span data-stu-id="3e80f-205">nickName</span></span>|<span data-ttu-id="3e80f-206">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-206">String</span></span>|<span data-ttu-id="3e80f-207">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-207">The contact's nickname.</span></span>|
|<span data-ttu-id="3e80f-208">officeLocation</span><span class="sxs-lookup"><span data-stu-id="3e80f-208">officeLocation</span></span>|<span data-ttu-id="3e80f-209">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-209">String</span></span>|<span data-ttu-id="3e80f-210">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-210">The location of the contact's office.</span></span>|
|<span data-ttu-id="3e80f-211">otherAddress</span><span class="sxs-lookup"><span data-stu-id="3e80f-211">otherAddress</span></span>|[<span data-ttu-id="3e80f-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="3e80f-212">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="3e80f-213">Outros endereços do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-213">Other addresses for the contact.</span></span>|
|<span data-ttu-id="3e80f-214">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="3e80f-214">parentFolderId</span></span>|<span data-ttu-id="3e80f-215">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-215">String</span></span>|<span data-ttu-id="3e80f-216">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-216">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="3e80f-217">personalNotes</span><span class="sxs-lookup"><span data-stu-id="3e80f-217">personalNotes</span></span>|<span data-ttu-id="3e80f-218">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-218">String</span></span>|<span data-ttu-id="3e80f-219">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-219">The user's notes about the contact.</span></span>|
|<span data-ttu-id="3e80f-220">profession</span><span class="sxs-lookup"><span data-stu-id="3e80f-220">profession</span></span>|<span data-ttu-id="3e80f-221">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-221">String</span></span>|<span data-ttu-id="3e80f-222">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-222">The contact's profession.</span></span>|
|<span data-ttu-id="3e80f-223">spouseName</span><span class="sxs-lookup"><span data-stu-id="3e80f-223">spouseName</span></span>|<span data-ttu-id="3e80f-224">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-224">String</span></span>|<span data-ttu-id="3e80f-225">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-225">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="3e80f-226">surname</span><span class="sxs-lookup"><span data-stu-id="3e80f-226">surname</span></span>|<span data-ttu-id="3e80f-227">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-227">String</span></span>|<span data-ttu-id="3e80f-228">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-228">The contact's surname.</span></span>|
|<span data-ttu-id="3e80f-229">title</span><span class="sxs-lookup"><span data-stu-id="3e80f-229">title</span></span>|<span data-ttu-id="3e80f-230">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-230">String</span></span>|<span data-ttu-id="3e80f-231">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="3e80f-231">The contact's title.</span></span>|
|<span data-ttu-id="3e80f-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="3e80f-232">yomiCompanyName</span></span>|<span data-ttu-id="3e80f-233">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-233">String</span></span>|<span data-ttu-id="3e80f-p107">O nome de empresa japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="3e80f-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="3e80f-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="3e80f-236">yomiGivenName</span></span>|<span data-ttu-id="3e80f-237">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-237">String</span></span>|<span data-ttu-id="3e80f-p108">O nome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="3e80f-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="3e80f-240">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="3e80f-240">yomiSurname</span></span>|<span data-ttu-id="3e80f-241">String</span><span class="sxs-lookup"><span data-stu-id="3e80f-241">String</span></span>|<span data-ttu-id="3e80f-p109">O sobrenome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="3e80f-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="3e80f-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e80f-244">Response</span></span>

<span data-ttu-id="3e80f-245">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e80f-245">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e80f-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e80f-246">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e80f-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e80f-247">Request</span></span>
<span data-ttu-id="3e80f-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e80f-248">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3e80f-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e80f-249">Response</span></span>
<span data-ttu-id="3e80f-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e80f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
