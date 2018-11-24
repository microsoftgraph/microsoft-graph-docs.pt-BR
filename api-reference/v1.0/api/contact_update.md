# <a name="update-contact"></a><span data-ttu-id="91f4b-101">Atualizar contato</span><span class="sxs-lookup"><span data-stu-id="91f4b-101">Update contact</span></span>

<span data-ttu-id="91f4b-102">Atualize as propriedades de um objeto contact.</span><span class="sxs-lookup"><span data-stu-id="91f4b-102">Update the properties of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="91f4b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="91f4b-103">Permissions</span></span>
<span data-ttu-id="91f4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="91f4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="91f4b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91f4b-106">Permission type</span></span>      | <span data-ttu-id="91f4b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91f4b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91f4b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91f4b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="91f4b-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91f4b-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="91f4b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91f4b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91f4b-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91f4b-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="91f4b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91f4b-112">Application</span></span> | <span data-ttu-id="91f4b-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91f4b-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="91f4b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91f4b-114">HTTP request</span></span>
<span data-ttu-id="91f4b-115"><!-- { "blockType": "ignored" } -->Um [contato](../resources/contact.md) do padrão de um usuário [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="91f4b-115"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="91f4b-116">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="91f4b-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="91f4b-p102">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="91f4b-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="91f4b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91f4b-119">Request headers</span></span>
| <span data-ttu-id="91f4b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91f4b-120">Header</span></span>       | <span data-ttu-id="91f4b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="91f4b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91f4b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="91f4b-122">Authorization</span></span>  | <span data-ttu-id="91f4b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91f4b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="91f4b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91f4b-125">Content-Type</span></span>  | <span data-ttu-id="91f4b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91f4b-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91f4b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91f4b-128">Request body</span></span>
<span data-ttu-id="91f4b-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="91f4b-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="91f4b-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91f4b-132">Property</span></span>     | <span data-ttu-id="91f4b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="91f4b-133">Type</span></span>   |<span data-ttu-id="91f4b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="91f4b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91f4b-135">assistantName</span><span class="sxs-lookup"><span data-stu-id="91f4b-135">assistantName</span></span>|<span data-ttu-id="91f4b-136">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-136">String</span></span>|<span data-ttu-id="91f4b-137">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-137">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="91f4b-138">birthday</span><span class="sxs-lookup"><span data-stu-id="91f4b-138">birthday</span></span>|<span data-ttu-id="91f4b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f4b-139">DateTimeOffset</span></span>|<span data-ttu-id="91f4b-140">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-140">The contact's birthday.</span></span>|
|<span data-ttu-id="91f4b-141">businessAddress</span><span class="sxs-lookup"><span data-stu-id="91f4b-141">businessAddress</span></span>|[<span data-ttu-id="91f4b-142">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="91f4b-142">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="91f4b-143">O endereço comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-143">The contact's business address.</span></span>|
|<span data-ttu-id="91f4b-144">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="91f4b-144">businessHomePage</span></span>|<span data-ttu-id="91f4b-145">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-145">String</span></span>|<span data-ttu-id="91f4b-146">A home page comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-146">The business home page of the contact.</span></span>|
|<span data-ttu-id="91f4b-147">businessPhones</span><span class="sxs-lookup"><span data-stu-id="91f4b-147">businessPhones</span></span>|<span data-ttu-id="91f4b-148">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-148">String</span></span>|<span data-ttu-id="91f4b-149">Os números de telefone comerciais do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-149">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="91f4b-150">categories</span><span class="sxs-lookup"><span data-stu-id="91f4b-150">categories</span></span>|<span data-ttu-id="91f4b-151">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-151">String</span></span>|<span data-ttu-id="91f4b-152">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-152">The categories associated with the contact.</span></span>|
|<span data-ttu-id="91f4b-153">children</span><span class="sxs-lookup"><span data-stu-id="91f4b-153">children</span></span>|<span data-ttu-id="91f4b-154">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-154">String</span></span>|<span data-ttu-id="91f4b-155">Os nomes dos filhos do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-155">The names of the contact's children.</span></span>|
|<span data-ttu-id="91f4b-156">nomeDaEmpresa</span><span class="sxs-lookup"><span data-stu-id="91f4b-156">companyName</span></span>|<span data-ttu-id="91f4b-157">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-157">String</span></span>|<span data-ttu-id="91f4b-158">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-158">The name of the contact's company.</span></span>|
|<span data-ttu-id="91f4b-159">departamento</span><span class="sxs-lookup"><span data-stu-id="91f4b-159">department</span></span>|<span data-ttu-id="91f4b-160">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-160">String</span></span>|<span data-ttu-id="91f4b-161">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-161">The contact's department.</span></span>|
|<span data-ttu-id="91f4b-162">displayName</span><span class="sxs-lookup"><span data-stu-id="91f4b-162">displayName</span></span>|<span data-ttu-id="91f4b-163">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-163">String</span></span>|<span data-ttu-id="91f4b-164">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-164">The contact's display name.</span></span> <span data-ttu-id="91f4b-165">Observe que as atualizações posteriores a outras propriedades podem causar um valor gerado automaticamente substituir o valor displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="91f4b-165">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="91f4b-166">Para preservar a um valor pré-existente, sempre incluí-lo como displayName em uma operação de atualização.</span><span class="sxs-lookup"><span data-stu-id="91f4b-166">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="91f4b-167">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="91f4b-167">emailAddresses</span></span>|<span data-ttu-id="91f4b-168">Coleção [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="91f4b-168">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="91f4b-169">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-169">The contact's email addresses.</span></span>|
|<span data-ttu-id="91f4b-170">fileAs</span><span class="sxs-lookup"><span data-stu-id="91f4b-170">fileAs</span></span>|<span data-ttu-id="91f4b-171">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-171">String</span></span>|<span data-ttu-id="91f4b-172">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="91f4b-172">The name the contact is filed under.</span></span>|
|<span data-ttu-id="91f4b-173">generation</span><span class="sxs-lookup"><span data-stu-id="91f4b-173">generation</span></span>|<span data-ttu-id="91f4b-174">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-174">String</span></span>|<span data-ttu-id="91f4b-175">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-175">The contact's generation.</span></span>|
|<span data-ttu-id="91f4b-176">givenName</span><span class="sxs-lookup"><span data-stu-id="91f4b-176">givenName</span></span>|<span data-ttu-id="91f4b-177">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-177">String</span></span>|<span data-ttu-id="91f4b-178">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-178">The contact's given name.</span></span>|
|<span data-ttu-id="91f4b-179">homeAddress</span><span class="sxs-lookup"><span data-stu-id="91f4b-179">homeAddress</span></span>|[<span data-ttu-id="91f4b-180">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="91f4b-180">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="91f4b-181">O endereço residencial do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-181">The contact's home address.</span></span>|
|<span data-ttu-id="91f4b-182">homePhones</span><span class="sxs-lookup"><span data-stu-id="91f4b-182">homePhones</span></span>|<span data-ttu-id="91f4b-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f4b-183">String collection</span></span>|<span data-ttu-id="91f4b-184">Os números de telefone residenciais do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-184">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="91f4b-185">imAddresses</span><span class="sxs-lookup"><span data-stu-id="91f4b-185">imAddresses</span></span>|<span data-ttu-id="91f4b-186">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-186">String</span></span>|<span data-ttu-id="91f4b-187">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-187">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="91f4b-188">initials</span><span class="sxs-lookup"><span data-stu-id="91f4b-188">initials</span></span>|<span data-ttu-id="91f4b-189">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-189">String</span></span>|<span data-ttu-id="91f4b-190">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-190">The contact's initials.</span></span>|
|<span data-ttu-id="91f4b-191">jobTitle</span><span class="sxs-lookup"><span data-stu-id="91f4b-191">jobTitle</span></span>|<span data-ttu-id="91f4b-192">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-192">String</span></span>|<span data-ttu-id="91f4b-193">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-193">The contact’s job title.</span></span>|
|<span data-ttu-id="91f4b-194">manager</span><span class="sxs-lookup"><span data-stu-id="91f4b-194">manager</span></span>|<span data-ttu-id="91f4b-195">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-195">String</span></span>|<span data-ttu-id="91f4b-196">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-196">The name of the contact's manager.</span></span>
|<span data-ttu-id="91f4b-197">middleName</span><span class="sxs-lookup"><span data-stu-id="91f4b-197">middleName</span></span>|<span data-ttu-id="91f4b-198">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-198">String</span></span>|<span data-ttu-id="91f4b-199">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-199">The contact's middle name.</span></span>|
|<span data-ttu-id="91f4b-200">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="91f4b-200">mobilePhone</span></span>|<span data-ttu-id="91f4b-201">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-201">String</span></span>|<span data-ttu-id="91f4b-202">O número de celular do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-202">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="91f4b-203">nickName</span><span class="sxs-lookup"><span data-stu-id="91f4b-203">nickName</span></span>|<span data-ttu-id="91f4b-204">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-204">String</span></span>|<span data-ttu-id="91f4b-205">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-205">The contact's nickname.</span></span>|
|<span data-ttu-id="91f4b-206">officeLocation</span><span class="sxs-lookup"><span data-stu-id="91f4b-206">officeLocation</span></span>|<span data-ttu-id="91f4b-207">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-207">String</span></span>|<span data-ttu-id="91f4b-208">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-208">The location of the contact's office.</span></span>|
|<span data-ttu-id="91f4b-209">otherAddress</span><span class="sxs-lookup"><span data-stu-id="91f4b-209">otherAddress</span></span>|[<span data-ttu-id="91f4b-210">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="91f4b-210">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="91f4b-211">Outros endereços do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-211">Other addresses for the contact.</span></span>|
|<span data-ttu-id="91f4b-212">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="91f4b-212">parentFolderId</span></span>|<span data-ttu-id="91f4b-213">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-213">String</span></span>|<span data-ttu-id="91f4b-214">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-214">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="91f4b-215">personalNotes</span><span class="sxs-lookup"><span data-stu-id="91f4b-215">personalNotes</span></span>|<span data-ttu-id="91f4b-216">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-216">String</span></span>|<span data-ttu-id="91f4b-217">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-217">The user's notes about the contact.</span></span>|
|<span data-ttu-id="91f4b-218">profession</span><span class="sxs-lookup"><span data-stu-id="91f4b-218">profession</span></span>|<span data-ttu-id="91f4b-219">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-219">String</span></span>|<span data-ttu-id="91f4b-220">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-220">The contact's profession.</span></span>|
|<span data-ttu-id="91f4b-221">spouseName</span><span class="sxs-lookup"><span data-stu-id="91f4b-221">spouseName</span></span>|<span data-ttu-id="91f4b-222">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-222">String</span></span>|<span data-ttu-id="91f4b-223">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-223">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="91f4b-224">surname</span><span class="sxs-lookup"><span data-stu-id="91f4b-224">surname</span></span>|<span data-ttu-id="91f4b-225">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-225">String</span></span>|<span data-ttu-id="91f4b-226">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-226">The contact's surname.</span></span>|
|<span data-ttu-id="91f4b-227">title</span><span class="sxs-lookup"><span data-stu-id="91f4b-227">title</span></span>|<span data-ttu-id="91f4b-228">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-228">String</span></span>|<span data-ttu-id="91f4b-229">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="91f4b-229">The contact's title.</span></span>|
|<span data-ttu-id="91f4b-230">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="91f4b-230">yomiCompanyName</span></span>|<span data-ttu-id="91f4b-231">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-231">String</span></span>|<span data-ttu-id="91f4b-p107">O nome de empresa japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="91f4b-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="91f4b-234">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="91f4b-234">yomiGivenName</span></span>|<span data-ttu-id="91f4b-235">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-235">String</span></span>|<span data-ttu-id="91f4b-p108">O nome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="91f4b-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="91f4b-238">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="91f4b-238">yomiSurname</span></span>|<span data-ttu-id="91f4b-239">String</span><span class="sxs-lookup"><span data-stu-id="91f4b-239">String</span></span>|<span data-ttu-id="91f4b-p109">O sobrenome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="91f4b-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="91f4b-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="91f4b-242">Response</span></span>

<span data-ttu-id="91f4b-243">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91f4b-243">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91f4b-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91f4b-244">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91f4b-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91f4b-245">Request</span></span>
<span data-ttu-id="91f4b-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91f4b-246">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="91f4b-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="91f4b-247">Response</span></span>
<span data-ttu-id="91f4b-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91f4b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
