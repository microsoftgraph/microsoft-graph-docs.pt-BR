---
title: Atualizar contato
description: Atualiza as propriedades do objeto de contato.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c6ed3304b5f44a8bb1d35c1db491e8eaf7ae47b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455696"
---
# <a name="update-contact"></a><span data-ttu-id="27a3f-103">Atualizar contato</span><span class="sxs-lookup"><span data-stu-id="27a3f-103">Update contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27a3f-104">Atualiza as propriedades do objeto de contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-104">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="27a3f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="27a3f-105">Permissions</span></span>
<span data-ttu-id="27a3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27a3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27a3f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27a3f-108">Permission type</span></span>      | <span data-ttu-id="27a3f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27a3f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27a3f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27a3f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27a3f-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27a3f-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="27a3f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27a3f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27a3f-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27a3f-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="27a3f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27a3f-114">Application</span></span> | <span data-ttu-id="27a3f-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27a3f-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="27a3f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27a3f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="27a3f-117">Um [contato](../resources/contact.md) do [contactFolder](../resources/contactfolder.md)padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="27a3f-117">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="27a3f-118">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="27a3f-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="27a3f-119">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="27a3f-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="27a3f-120">O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="27a3f-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="27a3f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27a3f-121">Request headers</span></span>
| <span data-ttu-id="27a3f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27a3f-122">Header</span></span>       | <span data-ttu-id="27a3f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="27a3f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27a3f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="27a3f-124">Authorization</span></span>  | <span data-ttu-id="27a3f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27a3f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27a3f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27a3f-127">Content-Type</span></span>  | <span data-ttu-id="27a3f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27a3f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27a3f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27a3f-130">Request body</span></span>
<span data-ttu-id="27a3f-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="27a3f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="27a3f-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27a3f-134">Property</span></span>     | <span data-ttu-id="27a3f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="27a3f-135">Type</span></span>   |<span data-ttu-id="27a3f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="27a3f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27a3f-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="27a3f-137">assistantName</span></span>|<span data-ttu-id="27a3f-138">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-138">String</span></span>|<span data-ttu-id="27a3f-139">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="27a3f-140">birthday</span><span class="sxs-lookup"><span data-stu-id="27a3f-140">birthday</span></span>|<span data-ttu-id="27a3f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27a3f-141">DateTimeOffset</span></span>|<span data-ttu-id="27a3f-142">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-142">The contact's birthday.</span></span>|
|<span data-ttu-id="27a3f-143">categories</span><span class="sxs-lookup"><span data-stu-id="27a3f-143">categories</span></span>|<span data-ttu-id="27a3f-144">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-144">String</span></span>|<span data-ttu-id="27a3f-145">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-145">The categories associated with the contact.</span></span>|
|<span data-ttu-id="27a3f-146">children</span><span class="sxs-lookup"><span data-stu-id="27a3f-146">children</span></span>|<span data-ttu-id="27a3f-147">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-147">String</span></span>||
|<span data-ttu-id="27a3f-148">companyName</span><span class="sxs-lookup"><span data-stu-id="27a3f-148">companyName</span></span>|<span data-ttu-id="27a3f-149">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-149">String</span></span>|<span data-ttu-id="27a3f-150">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-150">The name of the contact's company.</span></span>|
|<span data-ttu-id="27a3f-151">department</span><span class="sxs-lookup"><span data-stu-id="27a3f-151">department</span></span>|<span data-ttu-id="27a3f-152">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-152">String</span></span>|<span data-ttu-id="27a3f-153">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-153">The contact's department.</span></span>|
|<span data-ttu-id="27a3f-154">displayName</span><span class="sxs-lookup"><span data-stu-id="27a3f-154">displayName</span></span>|<span data-ttu-id="27a3f-155">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-155">String</span></span>|<span data-ttu-id="27a3f-156">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-156">The contact's display name.</span></span> <span data-ttu-id="27a3f-157">Observe que atualizações posteriores a outras propriedades podem fazer com que um valor gerado automaticamente substitua o valor displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="27a3f-157">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="27a3f-158">Para preservar um valor preexistente, sempre inclua-o como displayName em uma operação Update.</span><span class="sxs-lookup"><span data-stu-id="27a3f-158">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="27a3f-159">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="27a3f-159">emailAddresses</span></span>|<span data-ttu-id="27a3f-160">coleção [typedEmailAddress](../resources/typedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="27a3f-160">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="27a3f-161">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-161">The contact's email addresses.</span></span>|
|<span data-ttu-id="27a3f-162">fileAs</span><span class="sxs-lookup"><span data-stu-id="27a3f-162">fileAs</span></span>|<span data-ttu-id="27a3f-163">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-163">String</span></span>|<span data-ttu-id="27a3f-164">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="27a3f-164">The name the contact is filed under.</span></span>|
|<span data-ttu-id="27a3f-165">gender</span><span class="sxs-lookup"><span data-stu-id="27a3f-165">gender</span></span> |<span data-ttu-id="27a3f-166">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-166">String</span></span> |<span data-ttu-id="27a3f-167">O sexo do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-167">The contact's gender.</span></span> |
|<span data-ttu-id="27a3f-168">generation</span><span class="sxs-lookup"><span data-stu-id="27a3f-168">generation</span></span>|<span data-ttu-id="27a3f-169">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-169">String</span></span>|<span data-ttu-id="27a3f-170">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-170">The contact's generation.</span></span>|
|<span data-ttu-id="27a3f-171">givenName</span><span class="sxs-lookup"><span data-stu-id="27a3f-171">givenName</span></span>|<span data-ttu-id="27a3f-172">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-172">String</span></span>|<span data-ttu-id="27a3f-173">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-173">The contact's given name.</span></span>|
|<span data-ttu-id="27a3f-174">imAddresses</span><span class="sxs-lookup"><span data-stu-id="27a3f-174">imAddresses</span></span>|<span data-ttu-id="27a3f-175">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-175">String</span></span>|<span data-ttu-id="27a3f-176">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-176">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="27a3f-177">initials</span><span class="sxs-lookup"><span data-stu-id="27a3f-177">initials</span></span>|<span data-ttu-id="27a3f-178">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-178">String</span></span>|<span data-ttu-id="27a3f-179">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-179">The contact's initials.</span></span>|
|<span data-ttu-id="27a3f-180">jobTitle</span><span class="sxs-lookup"><span data-stu-id="27a3f-180">jobTitle</span></span>|<span data-ttu-id="27a3f-181">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-181">String</span></span>|<span data-ttu-id="27a3f-182">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-182">The contact’s job title.</span></span>|
|<span data-ttu-id="27a3f-183">manager</span><span class="sxs-lookup"><span data-stu-id="27a3f-183">manager</span></span>|<span data-ttu-id="27a3f-184">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-184">String</span></span>|<span data-ttu-id="27a3f-185">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-185">The name of the contact's manager.</span></span>
|<span data-ttu-id="27a3f-186">middleName</span><span class="sxs-lookup"><span data-stu-id="27a3f-186">middleName</span></span>|<span data-ttu-id="27a3f-187">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-187">String</span></span>|<span data-ttu-id="27a3f-188">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-188">The contact's middle name.</span></span>|
|<span data-ttu-id="27a3f-189">nickName</span><span class="sxs-lookup"><span data-stu-id="27a3f-189">nickName</span></span>|<span data-ttu-id="27a3f-190">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-190">String</span></span>|<span data-ttu-id="27a3f-191">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-191">The contact's nickname.</span></span>|
|<span data-ttu-id="27a3f-192">officeLocation</span><span class="sxs-lookup"><span data-stu-id="27a3f-192">officeLocation</span></span>|<span data-ttu-id="27a3f-193">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-193">String</span></span>|<span data-ttu-id="27a3f-194">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-194">The location of the contact's office.</span></span>|
|<span data-ttu-id="27a3f-195">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="27a3f-195">parentFolderId</span></span>|<span data-ttu-id="27a3f-196">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-196">String</span></span>|<span data-ttu-id="27a3f-197">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-197">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="27a3f-198">personalNotes</span><span class="sxs-lookup"><span data-stu-id="27a3f-198">personalNotes</span></span>|<span data-ttu-id="27a3f-199">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-199">String</span></span>|<span data-ttu-id="27a3f-200">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-200">The user's notes about the contact.</span></span>|
|<span data-ttu-id="27a3f-201">telefones</span><span class="sxs-lookup"><span data-stu-id="27a3f-201">phones</span></span> |<span data-ttu-id="27a3f-202">Coleção [phone](../resources/phone.md)</span><span class="sxs-lookup"><span data-stu-id="27a3f-202">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="27a3f-203">Números de telefone associados ao contato, por exemplo, telefone residencial, telefone celular e telefone comercial.</span><span class="sxs-lookup"><span data-stu-id="27a3f-203">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="27a3f-204">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="27a3f-204">postalAddresses</span></span> |<span data-ttu-id="27a3f-205">coleção [physicalAddress](../resources/physicaladdress.md)</span><span class="sxs-lookup"><span data-stu-id="27a3f-205">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="27a3f-206">Endereços associados ao contato, por exemplo, endereço residencial e endereço comercial.</span><span class="sxs-lookup"><span data-stu-id="27a3f-206">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="27a3f-207">profession</span><span class="sxs-lookup"><span data-stu-id="27a3f-207">profession</span></span>|<span data-ttu-id="27a3f-208">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-208">String</span></span>|<span data-ttu-id="27a3f-209">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-209">The contact's profession.</span></span>|
|<span data-ttu-id="27a3f-210">spouseName</span><span class="sxs-lookup"><span data-stu-id="27a3f-210">spouseName</span></span>|<span data-ttu-id="27a3f-211">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-211">String</span></span>|<span data-ttu-id="27a3f-212">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-212">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="27a3f-213">surname</span><span class="sxs-lookup"><span data-stu-id="27a3f-213">surname</span></span>|<span data-ttu-id="27a3f-214">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-214">String</span></span>|<span data-ttu-id="27a3f-215">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-215">The contact's surname.</span></span>|
|<span data-ttu-id="27a3f-216">title</span><span class="sxs-lookup"><span data-stu-id="27a3f-216">title</span></span>|<span data-ttu-id="27a3f-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27a3f-217">String</span></span>|<span data-ttu-id="27a3f-218">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-218">The contact's title.</span></span>|
|<span data-ttu-id="27a3f-219">websites</span><span class="sxs-lookup"><span data-stu-id="27a3f-219">websites</span></span> |<span data-ttu-id="27a3f-220">Coleção [website](../resources/website.md)</span><span class="sxs-lookup"><span data-stu-id="27a3f-220">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="27a3f-221">Sites da Web associados ao contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-221">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="27a3f-222">weddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="27a3f-222">weddingAnniversary</span></span> |<span data-ttu-id="27a3f-223">Data</span><span class="sxs-lookup"><span data-stu-id="27a3f-223">Date</span></span> |<span data-ttu-id="27a3f-224">Aniversário de casamento do contato.</span><span class="sxs-lookup"><span data-stu-id="27a3f-224">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="27a3f-225">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="27a3f-225">yomiCompanyName</span></span>|<span data-ttu-id="27a3f-226">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-226">String</span></span>|<span data-ttu-id="27a3f-p107">O nome de empresa japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="27a3f-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="27a3f-229">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="27a3f-229">yomiGivenName</span></span>|<span data-ttu-id="27a3f-230">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-230">String</span></span>|<span data-ttu-id="27a3f-p108">O nome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="27a3f-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="27a3f-233">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="27a3f-233">yomiSurname</span></span>|<span data-ttu-id="27a3f-234">String</span><span class="sxs-lookup"><span data-stu-id="27a3f-234">String</span></span>|<span data-ttu-id="27a3f-p109">O sobrenome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="27a3f-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="27a3f-237">Como o recurso de **contato** oferece suporte a [extensões](/graph/extensibility-overview), você `PATCH` pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **contato** existente.</span><span class="sxs-lookup"><span data-stu-id="27a3f-237">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="27a3f-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="27a3f-238">Response</span></span>

<span data-ttu-id="27a3f-239">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Contact](../resources/contact.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27a3f-239">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27a3f-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27a3f-240">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27a3f-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27a3f-241">Request</span></span>
<span data-ttu-id="27a3f-242">O exemplo a seguir atualiza o endereço de email pessoal do contato especificado.</span><span class="sxs-lookup"><span data-stu-id="27a3f-242">The following example updates the personal email address of the specified contact.</span></span>
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
##### <a name="response"></a><span data-ttu-id="27a3f-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="27a3f-243">Response</span></span>
<span data-ttu-id="27a3f-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27a3f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="27a3f-247">Confira também</span><span class="sxs-lookup"><span data-stu-id="27a3f-247">See also</span></span>

- [<span data-ttu-id="27a3f-248">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="27a3f-248">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="27a3f-249">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="27a3f-249">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/contact-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
