---
title: Atualizar contato
description: Atualize as propriedades do objeto de contato.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7022203e1e3ca4867ba1c1b026f450d21d94b591
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472521"
---
# <a name="update-contact"></a><span data-ttu-id="97c9f-103">Atualizar contato</span><span class="sxs-lookup"><span data-stu-id="97c9f-103">Update contact</span></span>

<span data-ttu-id="97c9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97c9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97c9f-105">Atualize as propriedades do objeto de contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-105">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="97c9f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="97c9f-106">Permissions</span></span>
<span data-ttu-id="97c9f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97c9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97c9f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97c9f-109">Permission type</span></span>      | <span data-ttu-id="97c9f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97c9f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97c9f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97c9f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97c9f-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97c9f-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="97c9f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97c9f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97c9f-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97c9f-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="97c9f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97c9f-115">Application</span></span> | <span data-ttu-id="97c9f-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97c9f-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="97c9f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97c9f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="97c9f-118">Um [contato](../resources/contact.md) do [contactFolder](../resources/contactfolder.md)padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="97c9f-118">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="97c9f-119">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="97c9f-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="97c9f-120">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="97c9f-120">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="97c9f-121">O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="97c9f-121">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="97c9f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97c9f-122">Request headers</span></span>
| <span data-ttu-id="97c9f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97c9f-123">Header</span></span>       | <span data-ttu-id="97c9f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="97c9f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97c9f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="97c9f-125">Authorization</span></span>  | <span data-ttu-id="97c9f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97c9f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97c9f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97c9f-128">Content-Type</span></span>  | <span data-ttu-id="97c9f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97c9f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97c9f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97c9f-131">Request body</span></span>
<span data-ttu-id="97c9f-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="97c9f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97c9f-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97c9f-135">Property</span></span>     | <span data-ttu-id="97c9f-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="97c9f-136">Type</span></span>   |<span data-ttu-id="97c9f-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="97c9f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97c9f-138">assistantName</span><span class="sxs-lookup"><span data-stu-id="97c9f-138">assistantName</span></span>|<span data-ttu-id="97c9f-139">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-139">String</span></span>|<span data-ttu-id="97c9f-140">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-140">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="97c9f-141">birthday</span><span class="sxs-lookup"><span data-stu-id="97c9f-141">birthday</span></span>|<span data-ttu-id="97c9f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97c9f-142">DateTimeOffset</span></span>|<span data-ttu-id="97c9f-143">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-143">The contact's birthday.</span></span>|
|<span data-ttu-id="97c9f-144">categories</span><span class="sxs-lookup"><span data-stu-id="97c9f-144">categories</span></span>|<span data-ttu-id="97c9f-145">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-145">String</span></span>|<span data-ttu-id="97c9f-146">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-146">The categories associated with the contact.</span></span>|
|<span data-ttu-id="97c9f-147">children</span><span class="sxs-lookup"><span data-stu-id="97c9f-147">children</span></span>|<span data-ttu-id="97c9f-148">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-148">String</span></span>||
|<span data-ttu-id="97c9f-149">companyName</span><span class="sxs-lookup"><span data-stu-id="97c9f-149">companyName</span></span>|<span data-ttu-id="97c9f-150">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-150">String</span></span>|<span data-ttu-id="97c9f-151">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-151">The name of the contact's company.</span></span>|
|<span data-ttu-id="97c9f-152">department</span><span class="sxs-lookup"><span data-stu-id="97c9f-152">department</span></span>|<span data-ttu-id="97c9f-153">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-153">String</span></span>|<span data-ttu-id="97c9f-154">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-154">The contact's department.</span></span>|
|<span data-ttu-id="97c9f-155">displayName</span><span class="sxs-lookup"><span data-stu-id="97c9f-155">displayName</span></span>|<span data-ttu-id="97c9f-156">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-156">String</span></span>|<span data-ttu-id="97c9f-157">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-157">The contact's display name.</span></span> <span data-ttu-id="97c9f-158">Observe que atualizações posteriores em outras propriedades podem fazer com que um valor gerado automaticamente sobrescreva o valor de displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="97c9f-158">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="97c9f-159">Para preservar a um valor preexistente, inclua-o como o displayName na operação atualizar.</span><span class="sxs-lookup"><span data-stu-id="97c9f-159">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="97c9f-160">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="97c9f-160">emailAddresses</span></span>|<span data-ttu-id="97c9f-161">[Coleção typedEmailAddress](../resources/typedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="97c9f-161">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="97c9f-162">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-162">The contact's email addresses.</span></span>|
|<span data-ttu-id="97c9f-163">fileAs</span><span class="sxs-lookup"><span data-stu-id="97c9f-163">fileAs</span></span>|<span data-ttu-id="97c9f-164">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-164">String</span></span>|<span data-ttu-id="97c9f-165">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="97c9f-165">The name the contact is filed under.</span></span>|
|<span data-ttu-id="97c9f-166">gender</span><span class="sxs-lookup"><span data-stu-id="97c9f-166">gender</span></span> |<span data-ttu-id="97c9f-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97c9f-167">String</span></span> |<span data-ttu-id="97c9f-168">O sexo do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-168">The contact's gender.</span></span> |
|<span data-ttu-id="97c9f-169">generation</span><span class="sxs-lookup"><span data-stu-id="97c9f-169">generation</span></span>|<span data-ttu-id="97c9f-170">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-170">String</span></span>|<span data-ttu-id="97c9f-171">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-171">The contact's generation.</span></span>|
|<span data-ttu-id="97c9f-172">givenName</span><span class="sxs-lookup"><span data-stu-id="97c9f-172">givenName</span></span>|<span data-ttu-id="97c9f-173">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-173">String</span></span>|<span data-ttu-id="97c9f-174">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-174">The contact's given name.</span></span>|
|<span data-ttu-id="97c9f-175">imAddresses</span><span class="sxs-lookup"><span data-stu-id="97c9f-175">imAddresses</span></span>|<span data-ttu-id="97c9f-176">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-176">String</span></span>|<span data-ttu-id="97c9f-177">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-177">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="97c9f-178">initials</span><span class="sxs-lookup"><span data-stu-id="97c9f-178">initials</span></span>|<span data-ttu-id="97c9f-179">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-179">String</span></span>|<span data-ttu-id="97c9f-180">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-180">The contact's initials.</span></span>|
|<span data-ttu-id="97c9f-181">jobTitle</span><span class="sxs-lookup"><span data-stu-id="97c9f-181">jobTitle</span></span>|<span data-ttu-id="97c9f-182">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-182">String</span></span>|<span data-ttu-id="97c9f-183">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-183">The contact’s job title.</span></span>|
|<span data-ttu-id="97c9f-184">manager</span><span class="sxs-lookup"><span data-stu-id="97c9f-184">manager</span></span>|<span data-ttu-id="97c9f-185">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-185">String</span></span>|<span data-ttu-id="97c9f-186">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-186">The name of the contact's manager.</span></span>
|<span data-ttu-id="97c9f-187">middleName</span><span class="sxs-lookup"><span data-stu-id="97c9f-187">middleName</span></span>|<span data-ttu-id="97c9f-188">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-188">String</span></span>|<span data-ttu-id="97c9f-189">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-189">The contact's middle name.</span></span>|
|<span data-ttu-id="97c9f-190">nickName</span><span class="sxs-lookup"><span data-stu-id="97c9f-190">nickName</span></span>|<span data-ttu-id="97c9f-191">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-191">String</span></span>|<span data-ttu-id="97c9f-192">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-192">The contact's nickname.</span></span>|
|<span data-ttu-id="97c9f-193">officeLocation</span><span class="sxs-lookup"><span data-stu-id="97c9f-193">officeLocation</span></span>|<span data-ttu-id="97c9f-194">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-194">String</span></span>|<span data-ttu-id="97c9f-195">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-195">The location of the contact's office.</span></span>|
|<span data-ttu-id="97c9f-196">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="97c9f-196">parentFolderId</span></span>|<span data-ttu-id="97c9f-197">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-197">String</span></span>|<span data-ttu-id="97c9f-198">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-198">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="97c9f-199">personalNotes</span><span class="sxs-lookup"><span data-stu-id="97c9f-199">personalNotes</span></span>|<span data-ttu-id="97c9f-200">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-200">String</span></span>|<span data-ttu-id="97c9f-201">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-201">The user's notes about the contact.</span></span>|
|<span data-ttu-id="97c9f-202">telefones</span><span class="sxs-lookup"><span data-stu-id="97c9f-202">phones</span></span> |<span data-ttu-id="97c9f-203">Coleção [phone](../resources/phone.md)</span><span class="sxs-lookup"><span data-stu-id="97c9f-203">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="97c9f-204">Números de telefone associados ao contato, por exemplo, telefone 1, celular e telefone comercial.</span><span class="sxs-lookup"><span data-stu-id="97c9f-204">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="97c9f-205">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="97c9f-205">postalAddresses</span></span> |<span data-ttu-id="97c9f-206">[Coleção physicalAddress](../resources/physicaladdress.md)</span><span class="sxs-lookup"><span data-stu-id="97c9f-206">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="97c9f-207">Endereços associados ao contato, por exemplo, endereço residencial e endereço comercial.</span><span class="sxs-lookup"><span data-stu-id="97c9f-207">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="97c9f-208">profession</span><span class="sxs-lookup"><span data-stu-id="97c9f-208">profession</span></span>|<span data-ttu-id="97c9f-209">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-209">String</span></span>|<span data-ttu-id="97c9f-210">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-210">The contact's profession.</span></span>|
|<span data-ttu-id="97c9f-211">spouseName</span><span class="sxs-lookup"><span data-stu-id="97c9f-211">spouseName</span></span>|<span data-ttu-id="97c9f-212">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-212">String</span></span>|<span data-ttu-id="97c9f-213">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-213">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="97c9f-214">surname</span><span class="sxs-lookup"><span data-stu-id="97c9f-214">surname</span></span>|<span data-ttu-id="97c9f-215">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-215">String</span></span>|<span data-ttu-id="97c9f-216">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-216">The contact's surname.</span></span>|
|<span data-ttu-id="97c9f-217">title</span><span class="sxs-lookup"><span data-stu-id="97c9f-217">title</span></span>|<span data-ttu-id="97c9f-218">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-218">String</span></span>|<span data-ttu-id="97c9f-219">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-219">The contact's title.</span></span>|
|<span data-ttu-id="97c9f-220">websites</span><span class="sxs-lookup"><span data-stu-id="97c9f-220">websites</span></span> |<span data-ttu-id="97c9f-221">Coleção [website](../resources/website.md)</span><span class="sxs-lookup"><span data-stu-id="97c9f-221">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="97c9f-222">Sites associados ao contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-222">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="97c9f-223">weddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="97c9f-223">weddingAnniversary</span></span> |<span data-ttu-id="97c9f-224">Data</span><span class="sxs-lookup"><span data-stu-id="97c9f-224">Date</span></span> |<span data-ttu-id="97c9f-225">O aniversário de casamento do contato.</span><span class="sxs-lookup"><span data-stu-id="97c9f-225">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="97c9f-226">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="97c9f-226">yomiCompanyName</span></span>|<span data-ttu-id="97c9f-227">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-227">String</span></span>|<span data-ttu-id="97c9f-p107">O nome de empresa japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="97c9f-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="97c9f-230">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="97c9f-230">yomiGivenName</span></span>|<span data-ttu-id="97c9f-231">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-231">String</span></span>|<span data-ttu-id="97c9f-p108">O nome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="97c9f-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="97c9f-234">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="97c9f-234">yomiSurname</span></span>|<span data-ttu-id="97c9f-235">String</span><span class="sxs-lookup"><span data-stu-id="97c9f-235">String</span></span>|<span data-ttu-id="97c9f-p109">O sobrenome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="97c9f-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="97c9f-238">Como o **recurso de** contato dá suporte a extensões, você pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo em propriedades [personalizadas](/graph/extensibility-overview)de uma extensão em uma instância de `PATCH` contato existente. </span><span class="sxs-lookup"><span data-stu-id="97c9f-238">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="97c9f-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="97c9f-239">Response</span></span>

<span data-ttu-id="97c9f-240">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [de](../resources/contact.md) contato atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97c9f-240">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97c9f-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97c9f-241">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97c9f-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97c9f-242">Request</span></span>
<span data-ttu-id="97c9f-243">O exemplo a seguir atualiza o endereço de email pessoal do contato especificado.</span><span class="sxs-lookup"><span data-stu-id="97c9f-243">The following example updates the personal email address of the specified contact.</span></span>

# <a name="http"></a>[<span data-ttu-id="97c9f-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="97c9f-244">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="97c9f-245">C#</span><span class="sxs-lookup"><span data-stu-id="97c9f-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97c9f-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97c9f-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97c9f-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97c9f-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97c9f-248">Java</span><span class="sxs-lookup"><span data-stu-id="97c9f-248">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="97c9f-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="97c9f-249">Response</span></span>
<span data-ttu-id="97c9f-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97c9f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="97c9f-253">Confira também</span><span class="sxs-lookup"><span data-stu-id="97c9f-253">See also</span></span>

- [<span data-ttu-id="97c9f-254">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="97c9f-254">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="97c9f-255">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="97c9f-255">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


