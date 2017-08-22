# <a name="update-contact"></a><span data-ttu-id="b7d82-101">Atualizar contato</span><span class="sxs-lookup"><span data-stu-id="b7d82-101">Update contact</span></span>

<span data-ttu-id="b7d82-102">Atualize as propriedades de um objeto contact.</span><span class="sxs-lookup"><span data-stu-id="b7d82-102">Update the properties of a contact object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b7d82-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7d82-103">Prerequisites</span></span>
<span data-ttu-id="b7d82-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="b7d82-104">One of the following **scopes** is required to execute this API: *Contacts.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="b7d82-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7d82-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b7d82-106">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="b7d82-106">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="b7d82-107">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="b7d82-107">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="b7d82-p101">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="b7d82-p101">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b7d82-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7d82-110">Request headers</span></span>
| <span data-ttu-id="b7d82-111">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7d82-111">Header</span></span>       | <span data-ttu-id="b7d82-112">Valor</span><span class="sxs-lookup"><span data-stu-id="b7d82-112">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7d82-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7d82-113">Authorization</span></span>  | <span data-ttu-id="b7d82-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7d82-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b7d82-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7d82-116">Content-Type</span></span>  | <span data-ttu-id="b7d82-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7d82-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7d82-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7d82-119">Request body</span></span>
<span data-ttu-id="b7d82-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b7d82-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b7d82-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7d82-123">Property</span></span>     | <span data-ttu-id="b7d82-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7d82-124">Type</span></span>   |<span data-ttu-id="b7d82-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7d82-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7d82-126">assistantName</span><span class="sxs-lookup"><span data-stu-id="b7d82-126">assistantName</span></span>|<span data-ttu-id="b7d82-127">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-127">String</span></span>|<span data-ttu-id="b7d82-128">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-128">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="b7d82-129">birthday</span><span class="sxs-lookup"><span data-stu-id="b7d82-129">birthday</span></span>|<span data-ttu-id="b7d82-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7d82-130">DateTimeOffset</span></span>|<span data-ttu-id="b7d82-131">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-131">The contact's birthday.</span></span>|
|<span data-ttu-id="b7d82-132">businessAddress</span><span class="sxs-lookup"><span data-stu-id="b7d82-132">businessAddress</span></span>|[<span data-ttu-id="b7d82-133">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b7d82-133">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="b7d82-134">O endereço comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-134">The contact's business address.</span></span>|
|<span data-ttu-id="b7d82-135">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="b7d82-135">businessHomePage</span></span>|<span data-ttu-id="b7d82-136">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-136">String</span></span>|<span data-ttu-id="b7d82-137">A home page comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-137">The business home page of the contact.</span></span>|
|<span data-ttu-id="b7d82-138">businessPhones</span><span class="sxs-lookup"><span data-stu-id="b7d82-138">businessPhones</span></span>|<span data-ttu-id="b7d82-139">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-139">String</span></span>|<span data-ttu-id="b7d82-140">Os números de telefone comerciais do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-140">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="b7d82-141">categories</span><span class="sxs-lookup"><span data-stu-id="b7d82-141">categories</span></span>|<span data-ttu-id="b7d82-142">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-142">String</span></span>|<span data-ttu-id="b7d82-143">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-143">The categories associated with the contact.</span></span>|
|<span data-ttu-id="b7d82-144">children</span><span class="sxs-lookup"><span data-stu-id="b7d82-144">children</span></span>|<span data-ttu-id="b7d82-145">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-145">String</span></span>|<span data-ttu-id="b7d82-146">Os nomes dos filhos do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-146">The names of the contact's children.</span></span>|
|<span data-ttu-id="b7d82-147">nomeDaEmpresa</span><span class="sxs-lookup"><span data-stu-id="b7d82-147">companyName</span></span>|<span data-ttu-id="b7d82-148">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-148">String</span></span>|<span data-ttu-id="b7d82-149">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-149">The name of the contact's company.</span></span>|
|<span data-ttu-id="b7d82-150">departamento</span><span class="sxs-lookup"><span data-stu-id="b7d82-150">department</span></span>|<span data-ttu-id="b7d82-151">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-151">String</span></span>|<span data-ttu-id="b7d82-152">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-152">The contact's department.</span></span>|
|<span data-ttu-id="b7d82-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b7d82-153">displayName</span></span>|<span data-ttu-id="b7d82-154">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-154">String</span></span>|<span data-ttu-id="b7d82-155">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-155">The contact's display name.</span></span>|
|<span data-ttu-id="b7d82-156">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="b7d82-156">emailAddresses</span></span>|<span data-ttu-id="b7d82-157">Coleção [EmailAddress](../resources/emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="b7d82-157">[EmailAddress](../resources/emailaddress.md) collection</span></span>|<span data-ttu-id="b7d82-158">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-158">The contact's email addresses.</span></span>|
|<span data-ttu-id="b7d82-159">fileAs</span><span class="sxs-lookup"><span data-stu-id="b7d82-159">fileAs</span></span>|<span data-ttu-id="b7d82-160">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-160">String</span></span>|<span data-ttu-id="b7d82-161">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="b7d82-161">The name the contact is filed under.</span></span>|
|<span data-ttu-id="b7d82-162">generation</span><span class="sxs-lookup"><span data-stu-id="b7d82-162">generation</span></span>|<span data-ttu-id="b7d82-163">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-163">String</span></span>|<span data-ttu-id="b7d82-164">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-164">The contact's generation.</span></span>|
|<span data-ttu-id="b7d82-165">givenName</span><span class="sxs-lookup"><span data-stu-id="b7d82-165">givenName</span></span>|<span data-ttu-id="b7d82-166">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-166">String</span></span>|<span data-ttu-id="b7d82-167">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-167">The contact's given name.</span></span>|
|<span data-ttu-id="b7d82-168">homeAddress</span><span class="sxs-lookup"><span data-stu-id="b7d82-168">homeAddress</span></span>|[<span data-ttu-id="b7d82-169">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b7d82-169">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="b7d82-170">O endereço residencial do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-170">The contact's home address.</span></span>|
|<span data-ttu-id="b7d82-171">homePhones</span><span class="sxs-lookup"><span data-stu-id="b7d82-171">homePhones</span></span>|<span data-ttu-id="b7d82-172">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7d82-172">String collection</span></span>|<span data-ttu-id="b7d82-173">Os números de telefone residenciais do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-173">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="b7d82-174">imAddresses</span><span class="sxs-lookup"><span data-stu-id="b7d82-174">imAddresses</span></span>|<span data-ttu-id="b7d82-175">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-175">String</span></span>|<span data-ttu-id="b7d82-176">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-176">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="b7d82-177">initials</span><span class="sxs-lookup"><span data-stu-id="b7d82-177">initials</span></span>|<span data-ttu-id="b7d82-178">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-178">String</span></span>|<span data-ttu-id="b7d82-179">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-179">The contact's initials.</span></span>|
|<span data-ttu-id="b7d82-180">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b7d82-180">jobTitle</span></span>|<span data-ttu-id="b7d82-181">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-181">String</span></span>|<span data-ttu-id="b7d82-182">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-182">The contact’s job title.</span></span>|
|<span data-ttu-id="b7d82-183">manager</span><span class="sxs-lookup"><span data-stu-id="b7d82-183">manager</span></span>|<span data-ttu-id="b7d82-184">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-184">String</span></span>|<span data-ttu-id="b7d82-185">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-185">The name of the contact's manager.</span></span>
|<span data-ttu-id="b7d82-186">middleName</span><span class="sxs-lookup"><span data-stu-id="b7d82-186">middleName</span></span>|<span data-ttu-id="b7d82-187">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-187">String</span></span>|<span data-ttu-id="b7d82-188">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-188">The contact's middle name.</span></span>|
|<span data-ttu-id="b7d82-189">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b7d82-189">mobilePhone</span></span>|<span data-ttu-id="b7d82-190">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-190">String</span></span>|<span data-ttu-id="b7d82-191">O número de celular do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-191">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="b7d82-192">nickName</span><span class="sxs-lookup"><span data-stu-id="b7d82-192">nickName</span></span>|<span data-ttu-id="b7d82-193">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-193">String</span></span>|<span data-ttu-id="b7d82-194">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-194">The contact's nickname.</span></span>|
|<span data-ttu-id="b7d82-195">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b7d82-195">officeLocation</span></span>|<span data-ttu-id="b7d82-196">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-196">String</span></span>|<span data-ttu-id="b7d82-197">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-197">The location of the contact's office.</span></span>|
|<span data-ttu-id="b7d82-198">otherAddress</span><span class="sxs-lookup"><span data-stu-id="b7d82-198">otherAddress</span></span>|[<span data-ttu-id="b7d82-199">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b7d82-199">PhysicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="b7d82-200">Outros endereços do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-200">Other addresses for the contact.</span></span>|
|<span data-ttu-id="b7d82-201">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="b7d82-201">parentFolderId</span></span>|<span data-ttu-id="b7d82-202">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-202">String</span></span>|<span data-ttu-id="b7d82-203">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-203">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="b7d82-204">personalNotes</span><span class="sxs-lookup"><span data-stu-id="b7d82-204">personalNotes</span></span>|<span data-ttu-id="b7d82-205">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-205">String</span></span>|<span data-ttu-id="b7d82-206">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-206">The user's notes about the contact.</span></span>|
|<span data-ttu-id="b7d82-207">profession</span><span class="sxs-lookup"><span data-stu-id="b7d82-207">profession</span></span>|<span data-ttu-id="b7d82-208">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-208">String</span></span>|<span data-ttu-id="b7d82-209">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-209">The contact's profession.</span></span>|
|<span data-ttu-id="b7d82-210">spouseName</span><span class="sxs-lookup"><span data-stu-id="b7d82-210">spouseName</span></span>|<span data-ttu-id="b7d82-211">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-211">String</span></span>|<span data-ttu-id="b7d82-212">O nome do cônjuge do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-212">The name of the contact's spouse.</span></span>|
|<span data-ttu-id="b7d82-213">surname</span><span class="sxs-lookup"><span data-stu-id="b7d82-213">surname</span></span>|<span data-ttu-id="b7d82-214">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-214">String</span></span>|<span data-ttu-id="b7d82-215">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-215">The contact's surname.</span></span>|
|<span data-ttu-id="b7d82-216">title</span><span class="sxs-lookup"><span data-stu-id="b7d82-216">title</span></span>|<span data-ttu-id="b7d82-217">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-217">String</span></span>|<span data-ttu-id="b7d82-218">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="b7d82-218">The contact's title.</span></span>|
|<span data-ttu-id="b7d82-219">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="b7d82-219">yomiCompanyName</span></span>|<span data-ttu-id="b7d82-220">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-220">String</span></span>|<span data-ttu-id="b7d82-p105">O nome de empresa japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="b7d82-p105">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="b7d82-223">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="b7d82-223">yomiGivenName</span></span>|<span data-ttu-id="b7d82-224">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-224">String</span></span>|<span data-ttu-id="b7d82-p106">O nome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="b7d82-p106">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="b7d82-227">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="b7d82-227">yomiSurname</span></span>|<span data-ttu-id="b7d82-228">String</span><span class="sxs-lookup"><span data-stu-id="b7d82-228">String</span></span>|<span data-ttu-id="b7d82-p107">O sobrenome japonês fonético do contato. Essa propriedade é opcional.</span><span class="sxs-lookup"><span data-stu-id="b7d82-p107">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

## <a name="response"></a><span data-ttu-id="b7d82-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7d82-231">Response</span></span>

<span data-ttu-id="b7d82-232">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contact](../resources/contact.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7d82-232">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7d82-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7d82-233">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7d82-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7d82-234">Request</span></span>
<span data-ttu-id="b7d82-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7d82-235">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b7d82-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7d82-236">Response</span></span>
<span data-ttu-id="b7d82-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7d82-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
