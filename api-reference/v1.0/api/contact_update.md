# <a name="update-contact"></a><span data-ttu-id="c9ea8-101">Atualizar contato</span><span class="sxs-lookup"><span data-stu-id="c9ea8-101">Update contact</span></span>

<span data-ttu-id="c9ea8-102">Atualize as propriedades de um objeto contact.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-102">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9ea8-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9ea8-103">Permissions</span></span>
<span data-ttu-id="c9ea8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c9ea8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c9ea8-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9ea8-106">Permission type</span></span>      | <span data-ttu-id="c9ea8-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9ea8-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c9ea8-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9ea8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c9ea8-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9ea8-109">Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="c9ea8-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9ea8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9ea8-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9ea8-111">Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="c9ea8-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9ea8-112">Application</span></span> | <span data-ttu-id="c9ea8-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9ea8-113">Contacts.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c9ea8-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9ea8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c9ea8-115">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="c9ea8-116">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="c9ea8-p102">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c9ea8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9ea8-119">Request headers</span></span>
| <span data-ttu-id="c9ea8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9ea8-120">Header</span></span>       | <span data-ttu-id="c9ea8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c9ea8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9ea8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9ea8-122">Authorization</span></span>  | <span data-ttu-id="c9ea8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c9ea8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9ea8-125">Content-Type</span></span>  | <span data-ttu-id="c9ea8-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c9ea8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9ea8-128">Request body</span></span>
<span data-ttu-id="c9ea8-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c9ea8-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9ea8-132">Property</span></span>     | <span data-ttu-id="c9ea8-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9ea8-133">Type</span></span>   |<span data-ttu-id="c9ea8-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9ea8-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9ea8-135">assistantName</span><span class="sxs-lookup"><span data-stu-id="c9ea8-135">assistantName</span></span>|<span data-ttu-id="c9ea8-136">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-136">String</span></span>|<span data-ttu-id="c9ea8-137">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-137">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="c9ea8-138">birthday</span><span class="sxs-lookup"><span data-stu-id="c9ea8-138">birthday</span></span>|<span data-ttu-id="c9ea8-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9ea8-139">DateTimeOffset</span></span>|<span data-ttu-id="c9ea8-140">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-140">The contact's birthday.</span></span>|
|<span data-ttu-id="c9ea8-141">businessAddress</span><span class="sxs-lookup"><span data-stu-id="c9ea8-141">businessAddress</span></span>|[<span data-ttu-id="c9ea8-142">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="c9ea8-142">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="c9ea8-143">O endereço comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-143">The contact's business address.</span></span>|
|<span data-ttu-id="c9ea8-144">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="c9ea8-144">businessHomePage</span></span>|<span data-ttu-id="c9ea8-145">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-145">String</span></span>|<span data-ttu-id="c9ea8-146">A home page comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-146">The business home page of the contact.</span></span>|
|<span data-ttu-id="c9ea8-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="c9ea8-147">businessPhones</span></span>|<span data-ttu-id="c9ea8-148">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-148">String</span></span>|<span data-ttu-id="c9ea8-149">Os números de telefone comerciais do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-149">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="c9ea8-150">categories</span><span class="sxs-lookup"><span data-stu-id="c9ea8-150">categories</span></span>|<span data-ttu-id="c9ea8-151">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-151">String</span></span>|<span data-ttu-id="c9ea8-152">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-152">The categories associated with the contact.</span></span>|
|<span data-ttu-id="c9ea8-153">children</span><span class="sxs-lookup"><span data-stu-id="c9ea8-153">children</span></span>|<span data-ttu-id="c9ea8-154">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-154">String</span></span>|<span data-ttu-id="c9ea8-155">Os nomes dos filhos do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-155">The names of the contact's children.</span></span>|
|<span data-ttu-id="c9ea8-156">nomeDaEmpresa</span><span class="sxs-lookup"><span data-stu-id="c9ea8-156">companyName</span></span>|<span data-ttu-id="c9ea8-157">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-157">String</span></span>|<span data-ttu-id="c9ea8-158">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-158">The name of the contact's company.</span></span>|
|<span data-ttu-id="c9ea8-159">departamento</span><span class="sxs-lookup"><span data-stu-id="c9ea8-159">department</span></span>|<span data-ttu-id="c9ea8-160">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-160">String</span></span>|<span data-ttu-id="c9ea8-161">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-161">The contact's department.</span></span>|
|<span data-ttu-id="c9ea8-162">displayName</span><span class="sxs-lookup"><span data-stu-id="c9ea8-162">displayName</span></span>|<span data-ttu-id="c9ea8-163">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-163">String</span></span>|<span data-ttu-id="c9ea8-164">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-164">The contact's display name.</span></span>|
|<span data-ttu-id="c9ea8-165">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="c9ea8-165">emailAddresses</span></span>|<span data-ttu-id="c9ea8-166">Coleção [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="c9ea8-166">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="c9ea8-167">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-167">The contact's email addresses.</span></span>|
|<span data-ttu-id="c9ea8-168">fileAs</span><span class="sxs-lookup"><span data-stu-id="c9ea8-168">fileAs</span></span>|<span data-ttu-id="c9ea8-169">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-169">String</span></span>|<span data-ttu-id="c9ea8-170">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-170">The name the contact is filed under.</span></span>|
|<span data-ttu-id="c9ea8-171">generation</span><span class="sxs-lookup"><span data-stu-id="c9ea8-171">generation</span></span>|<span data-ttu-id="c9ea8-172">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-172">String</span></span>|<span data-ttu-id="c9ea8-173">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-173">The contact's generation.</span></span>|
|<span data-ttu-id="c9ea8-174">givenName</span><span class="sxs-lookup"><span data-stu-id="c9ea8-174">givenName</span></span>|<span data-ttu-id="c9ea8-175">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-175">String</span></span>|<span data-ttu-id="c9ea8-176">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-176">The contact's given name.</span></span>|
|<span data-ttu-id="c9ea8-177">homeAddress</span><span class="sxs-lookup"><span data-stu-id="c9ea8-177">homeAddress</span></span>|[<span data-ttu-id="c9ea8-178">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="c9ea8-178">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="c9ea8-179">O endereço residencial do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-179">The contact's home address.</span></span>|
|<span data-ttu-id="c9ea8-180">homePhones</span><span class="sxs-lookup"><span data-stu-id="c9ea8-180">homePhones</span></span>|<span data-ttu-id="c9ea8-181">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9ea8-181">String collection</span></span>|<span data-ttu-id="c9ea8-182">Os números de telefone residenciais do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-182">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="c9ea8-183">imAddresses</span><span class="sxs-lookup"><span data-stu-id="c9ea8-183">imAddresses</span></span>|<span data-ttu-id="c9ea8-184">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-184">String</span></span>|<span data-ttu-id="c9ea8-185">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-185">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="c9ea8-186">initials</span><span class="sxs-lookup"><span data-stu-id="c9ea8-186">initials</span></span>|<span data-ttu-id="c9ea8-187">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-187">String</span></span>|<span data-ttu-id="c9ea8-188">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-188">The contact's initials.</span></span>|
|<span data-ttu-id="c9ea8-189">jobTitle</span><span class="sxs-lookup"><span data-stu-id="c9ea8-189">jobTitle</span></span>|<span data-ttu-id="c9ea8-190">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-190">String</span></span>|<span data-ttu-id="c9ea8-191">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-191">The contact’s job title.</span></span>|
|<span data-ttu-id="c9ea8-192">manager</span><span class="sxs-lookup"><span data-stu-id="c9ea8-192">manager</span></span>|<span data-ttu-id="c9ea8-193">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-193">String</span></span>|<span data-ttu-id="c9ea8-194">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-194">The name of the contact's manager.</span></span>
|<span data-ttu-id="c9ea8-195">middleName</span><span class="sxs-lookup"><span data-stu-id="c9ea8-195">middleName</span></span>|<span data-ttu-id="c9ea8-196">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-196">String</span></span>|<span data-ttu-id="c9ea8-197">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-197">The contact's middle name.</span></span>|
|<span data-ttu-id="c9ea8-198">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="c9ea8-198">mobilePhone</span></span>|<span data-ttu-id="c9ea8-199">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-199">String</span></span>|<span data-ttu-id="c9ea8-200">O número de celular do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-200">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="c9ea8-201">nickName</span><span class="sxs-lookup"><span data-stu-id="c9ea8-201">nickName</span></span>|<span data-ttu-id="c9ea8-202">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-202">String</span></span>|<span data-ttu-id="c9ea8-203">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-203">The contact's nickname.</span></span>|
|<span data-ttu-id="c9ea8-204">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c9ea8-204">officeLocation</span></span>|<span data-ttu-id="c9ea8-205">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-205">String</span></span>|<span data-ttu-id="c9ea8-206">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-206">The location of the contact's office.</span></span>|
|<span data-ttu-id="c9ea8-207">otherAddress</span><span class="sxs-lookup"><span data-stu-id="c9ea8-207">otherAddress</span></span>|[<span data-ttu-id="c9ea8-208">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="c9ea8-208">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="c9ea8-209">Outros endereços do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-209">Other addresses for the contact.</span></span>|
|<span data-ttu-id="c9ea8-210">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="c9ea8-210">parentFolderId</span></span>|<span data-ttu-id="c9ea8-211">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-211">String</span></span>|<span data-ttu-id="c9ea8-212">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-212">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="c9ea8-213">personalNotes</span><span class="sxs-lookup"><span data-stu-id="c9ea8-213">personalNotes</span></span>|<span data-ttu-id="c9ea8-214">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-214">String</span></span>|<span data-ttu-id="c9ea8-215">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-215">The user's notes about the contact.</span></span>|
|<span data-ttu-id="c9ea8-216">profession</span><span class="sxs-lookup"><span data-stu-id="c9ea8-216">profession</span></span>|<span data-ttu-id="c9ea8-217">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-217">String</span></span>|<span data-ttu-id="c9ea8-218">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-218">The contact's profession.</span></span>|
|<span data-ttu-id="c9ea8-219">spouseName</span><span class="sxs-lookup"><span data-stu-id="c9ea8-219">spouseName</span></span>|<span data-ttu-id="c9ea8-220">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-220">String</span></span>|<span data-ttu-id="c9ea8-221">O nome do cônjuge do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-221">The name of the contact's spouse.</span></span>|
|<span data-ttu-id="c9ea8-222">surname</span><span class="sxs-lookup"><span data-stu-id="c9ea8-222">surname</span></span>|<span data-ttu-id="c9ea8-223">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-223">String</span></span>|<span data-ttu-id="c9ea8-224">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-224">The contact's surname.</span></span>|
|<span data-ttu-id="c9ea8-225">title</span><span class="sxs-lookup"><span data-stu-id="c9ea8-225">title</span></span>|<span data-ttu-id="c9ea8-226">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-226">String</span></span>|<span data-ttu-id="c9ea8-227">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-227">The contact's title.</span></span>|
|<span data-ttu-id="c9ea8-228">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="c9ea8-228">yomiCompanyName</span></span>|<span data-ttu-id="c9ea8-229">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-229">String</span></span>|<span data-ttu-id="c9ea8-p106">O nome de empresa japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-p106">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="c9ea8-232">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="c9ea8-232">yomiGivenName</span></span>|<span data-ttu-id="c9ea8-233">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-233">String</span></span>|<span data-ttu-id="c9ea8-p107">O nome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-p107">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="c9ea8-236">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="c9ea8-236">yomiSurname</span></span>|<span data-ttu-id="c9ea8-237">String</span><span class="sxs-lookup"><span data-stu-id="c9ea8-237">String</span></span>|<span data-ttu-id="c9ea8-p108">O sobrenome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-p108">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="c9ea8-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9ea8-240">Response</span></span>

<span data-ttu-id="c9ea8-241">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-241">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9ea8-242">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9ea8-242">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9ea8-243">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9ea8-243">Request</span></span>
<span data-ttu-id="c9ea8-244">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-244">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c9ea8-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9ea8-245">Response</span></span>
<span data-ttu-id="c9ea8-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9ea8-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "businessHomePage": "http://www.contoso.com",
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
