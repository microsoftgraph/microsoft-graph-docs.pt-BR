---
title: tipo de recurso contact
description: Um contato é um item no Outlook no qual você pode organizar e salvar informações sobre as pessoas e organizações com quem se comunica. Os contatos estão contidos em pastas de contatos.
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 91ce5d0c21d0b9dc700e2669efe881488d79257d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721996"
---
# <a name="contact-resource-type"></a><span data-ttu-id="b5f50-104">tipo de recurso contact</span><span class="sxs-lookup"><span data-stu-id="b5f50-104">contact resource type</span></span>

<span data-ttu-id="b5f50-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5f50-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5f50-p102">Um contato é um item no Outlook no qual você pode organizar e salvar informações sobre as pessoas e organizações com quem se comunica. Os contatos estão contidos em pastas de contatos.</span><span class="sxs-lookup"><span data-stu-id="b5f50-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="b5f50-108">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="b5f50-108">This resource supports:</span></span>

- <span data-ttu-id="b5f50-109">Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="b5f50-109">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="b5f50-110">Assinar as [notificações de alteração](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="b5f50-110">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="b5f50-111">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contact-delta.md).</span><span class="sxs-lookup"><span data-stu-id="b5f50-111">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="b5f50-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="b5f50-112">Methods</span></span>

| <span data-ttu-id="b5f50-113">Método</span><span class="sxs-lookup"><span data-stu-id="b5f50-113">Method</span></span>       | <span data-ttu-id="b5f50-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b5f50-114">Return Type</span></span>  |<span data-ttu-id="b5f50-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5f50-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b5f50-116">Obter contato</span><span class="sxs-lookup"><span data-stu-id="b5f50-116">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="b5f50-117">contact</span><span class="sxs-lookup"><span data-stu-id="b5f50-117">contact</span></span>](contact.md) |<span data-ttu-id="b5f50-118">Leia as propriedades e as relações do objeto contact.</span><span class="sxs-lookup"><span data-stu-id="b5f50-118">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="b5f50-119">Create</span><span class="sxs-lookup"><span data-stu-id="b5f50-119">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="b5f50-120">contact</span><span class="sxs-lookup"><span data-stu-id="b5f50-120">contact</span></span>](contact.md) |<span data-ttu-id="b5f50-121">Adicione um contato na pasta de Contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="b5f50-121">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="b5f50-122">Update</span><span class="sxs-lookup"><span data-stu-id="b5f50-122">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="b5f50-123">contact</span><span class="sxs-lookup"><span data-stu-id="b5f50-123">contact</span></span>](contact.md) |<span data-ttu-id="b5f50-124">Atualize o objeto contact.</span><span class="sxs-lookup"><span data-stu-id="b5f50-124">Update contact object.</span></span> |
|[<span data-ttu-id="b5f50-125">Delete</span><span class="sxs-lookup"><span data-stu-id="b5f50-125">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="b5f50-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b5f50-126">None</span></span> |<span data-ttu-id="b5f50-127">Exclua um objeto contact.</span><span class="sxs-lookup"><span data-stu-id="b5f50-127">Delete contact object.</span></span> |
|[<span data-ttu-id="b5f50-128">delta</span><span class="sxs-lookup"><span data-stu-id="b5f50-128">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="b5f50-129">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="b5f50-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="b5f50-130">Obtenha um conjunto de contatos que foram adicionados, excluídos ou atualizados em uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="b5f50-130">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="b5f50-131">**Extensões abertas**</span><span class="sxs-lookup"><span data-stu-id="b5f50-131">**Open extensions**</span></span>| | |
|[<span data-ttu-id="b5f50-132">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="b5f50-132">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="b5f50-133">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="b5f50-133">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="b5f50-134">Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="b5f50-134">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="b5f50-135">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="b5f50-135">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="b5f50-136">Coleção [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="b5f50-136">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="b5f50-137">Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="b5f50-137">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="b5f50-138">**Extensões de esquema**</span><span class="sxs-lookup"><span data-stu-id="b5f50-138">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="b5f50-139">Adicionar valores de extensões de esquema</span><span class="sxs-lookup"><span data-stu-id="b5f50-139">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="b5f50-140">Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.</span><span class="sxs-lookup"><span data-stu-id="b5f50-140">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="b5f50-141">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="b5f50-141">**Extended properties**</span></span>| | |
|[<span data-ttu-id="b5f50-142">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="b5f50-142">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="b5f50-143">contact</span><span class="sxs-lookup"><span data-stu-id="b5f50-143">contact</span></span>](contact.md)  |<span data-ttu-id="b5f50-144">Criar uma ou mais propriedades estendidas de valor único em um contato novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="b5f50-144">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="b5f50-145">Obter contato com propriedade estendida com valor único</span><span class="sxs-lookup"><span data-stu-id="b5f50-145">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b5f50-146">contact</span><span class="sxs-lookup"><span data-stu-id="b5f50-146">contact</span></span>](contact.md) | <span data-ttu-id="b5f50-147">Obter contatos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b5f50-147">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="b5f50-148">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="b5f50-148">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="b5f50-149">contact</span><span class="sxs-lookup"><span data-stu-id="b5f50-149">contact</span></span>](contact.md) | <span data-ttu-id="b5f50-150">Criar uma ou mais propriedades estendidas de vários valores em um contato novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="b5f50-150">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="b5f50-151">Obter contato com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="b5f50-151">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="b5f50-152">contact</span><span class="sxs-lookup"><span data-stu-id="b5f50-152">contact</span></span>](contact.md) | <span data-ttu-id="b5f50-153">Obter um contato que contenha uma propriedade estendida de vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="b5f50-153">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="b5f50-154">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5f50-154">Properties</span></span>
| <span data-ttu-id="b5f50-155">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5f50-155">Property</span></span>     | <span data-ttu-id="b5f50-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5f50-156">Type</span></span>   |<span data-ttu-id="b5f50-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5f50-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5f50-158">assistantName</span><span class="sxs-lookup"><span data-stu-id="b5f50-158">assistantName</span></span>|<span data-ttu-id="b5f50-159">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-159">String</span></span>|<span data-ttu-id="b5f50-160">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-160">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="b5f50-161">birthday</span><span class="sxs-lookup"><span data-stu-id="b5f50-161">birthday</span></span>|<span data-ttu-id="b5f50-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5f50-162">DateTimeOffset</span></span>|<span data-ttu-id="b5f50-163">O aniversário do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-163">The contact's birthday.</span></span> <span data-ttu-id="b5f50-164">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b5f50-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b5f50-165">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b5f50-165">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b5f50-166">businessAddress</span><span class="sxs-lookup"><span data-stu-id="b5f50-166">businessAddress</span></span>|[<span data-ttu-id="b5f50-167">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b5f50-167">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="b5f50-168">O endereço comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-168">The contact's business address.</span></span>|
|<span data-ttu-id="b5f50-169">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="b5f50-169">businessHomePage</span></span>|<span data-ttu-id="b5f50-170">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-170">String</span></span>|<span data-ttu-id="b5f50-171">A home page comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-171">The business home page of the contact.</span></span>|
|<span data-ttu-id="b5f50-172">businessPhones</span><span class="sxs-lookup"><span data-stu-id="b5f50-172">businessPhones</span></span>|<span data-ttu-id="b5f50-173">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f50-173">String collection</span></span>|<span data-ttu-id="b5f50-174">Os números de telefone comerciais do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-174">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="b5f50-175">categories</span><span class="sxs-lookup"><span data-stu-id="b5f50-175">categories</span></span>|<span data-ttu-id="b5f50-176">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f50-176">String collection</span></span>|<span data-ttu-id="b5f50-177">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-177">The categories associated with the contact.</span></span>|
|<span data-ttu-id="b5f50-178">changeKey</span><span class="sxs-lookup"><span data-stu-id="b5f50-178">changeKey</span></span>|<span data-ttu-id="b5f50-179">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-179">String</span></span>|<span data-ttu-id="b5f50-p104">Identifica a versão do contato. Toda vez que o contato muda, a ChangeKey também muda. Isso permite que o Exchange aplique alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="b5f50-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="b5f50-183">children</span><span class="sxs-lookup"><span data-stu-id="b5f50-183">children</span></span>|<span data-ttu-id="b5f50-184">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f50-184">String collection</span></span>|<span data-ttu-id="b5f50-185">Os nomes dos filhos do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-185">The names of the contact's children.</span></span>|
|<span data-ttu-id="b5f50-186">nomeDaEmpresa</span><span class="sxs-lookup"><span data-stu-id="b5f50-186">companyName</span></span>|<span data-ttu-id="b5f50-187">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-187">String</span></span>|<span data-ttu-id="b5f50-188">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-188">The name of the contact's company.</span></span>|
|<span data-ttu-id="b5f50-189">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5f50-189">createdDateTime</span></span>|<span data-ttu-id="b5f50-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5f50-190">DateTimeOffset</span></span>|<span data-ttu-id="b5f50-191">A hora em que o contato foi criado.</span><span class="sxs-lookup"><span data-stu-id="b5f50-191">The time the contact was created.</span></span> <span data-ttu-id="b5f50-192">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b5f50-192">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b5f50-193">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b5f50-193">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b5f50-194">department</span><span class="sxs-lookup"><span data-stu-id="b5f50-194">department</span></span>|<span data-ttu-id="b5f50-195">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-195">String</span></span>|<span data-ttu-id="b5f50-196">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-196">The contact's department.</span></span>|
|<span data-ttu-id="b5f50-197">displayName</span><span class="sxs-lookup"><span data-stu-id="b5f50-197">displayName</span></span>|<span data-ttu-id="b5f50-198">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-198">String</span></span>|<span data-ttu-id="b5f50-199">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-199">The contact's display name.</span></span> <span data-ttu-id="b5f50-200">Você pode especificar o nome de exibição em uma operação [criar](../api/user-post-contacts.md) ou [atualizar](../api/contact-update.md).</span><span class="sxs-lookup"><span data-stu-id="b5f50-200">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="b5f50-201">Observe que atualizações posteriores em outras propriedades podem fazer com que um valor gerado automaticamente sobrescreva o valor de displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="b5f50-201">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="b5f50-202">Para preservar a um valor preexistente, inclua-o como o displayName na operação [atualizar](../api/contact-update.md).</span><span class="sxs-lookup"><span data-stu-id="b5f50-202">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="b5f50-203">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="b5f50-203">emailAddresses</span></span>|<span data-ttu-id="b5f50-204">Coleção [EmailAddress](emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="b5f50-204">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="b5f50-205">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-205">The contact's email addresses.</span></span>|
|<span data-ttu-id="b5f50-206">fileAs</span><span class="sxs-lookup"><span data-stu-id="b5f50-206">fileAs</span></span>|<span data-ttu-id="b5f50-207">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-207">String</span></span>|<span data-ttu-id="b5f50-208">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="b5f50-208">The name the contact is filed under.</span></span>|
|<span data-ttu-id="b5f50-209">generation</span><span class="sxs-lookup"><span data-stu-id="b5f50-209">generation</span></span>|<span data-ttu-id="b5f50-210">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-210">String</span></span>|<span data-ttu-id="b5f50-211">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-211">The contact's generation.</span></span>|
|<span data-ttu-id="b5f50-212">givenName</span><span class="sxs-lookup"><span data-stu-id="b5f50-212">givenName</span></span>|<span data-ttu-id="b5f50-213">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-213">String</span></span>|<span data-ttu-id="b5f50-214">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-214">The contact's given name.</span></span>|
|<span data-ttu-id="b5f50-215">homeAddress</span><span class="sxs-lookup"><span data-stu-id="b5f50-215">homeAddress</span></span>|[<span data-ttu-id="b5f50-216">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b5f50-216">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="b5f50-217">O endereço residencial do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-217">The contact's home address.</span></span>|
|<span data-ttu-id="b5f50-218">homePhones</span><span class="sxs-lookup"><span data-stu-id="b5f50-218">homePhones</span></span>|<span data-ttu-id="b5f50-219">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f50-219">String collection</span></span>|<span data-ttu-id="b5f50-220">Os números de telefone residenciais do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-220">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="b5f50-221">id</span><span class="sxs-lookup"><span data-stu-id="b5f50-221">id</span></span>|<span data-ttu-id="b5f50-222">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-222">String</span></span>|<span data-ttu-id="b5f50-p107">O identificador exclusivo do contato. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5f50-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="b5f50-225">imAddresses</span><span class="sxs-lookup"><span data-stu-id="b5f50-225">imAddresses</span></span>|<span data-ttu-id="b5f50-226">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f50-226">String collection</span></span>|<span data-ttu-id="b5f50-227">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-227">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="b5f50-228">initials</span><span class="sxs-lookup"><span data-stu-id="b5f50-228">initials</span></span>|<span data-ttu-id="b5f50-229">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-229">String</span></span>|<span data-ttu-id="b5f50-230">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-230">The contact's initials.</span></span>|
|<span data-ttu-id="b5f50-231">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b5f50-231">jobTitle</span></span>|<span data-ttu-id="b5f50-232">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-232">String</span></span>|<span data-ttu-id="b5f50-233">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-233">The contact’s job title.</span></span>|
|<span data-ttu-id="b5f50-234">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5f50-234">lastModifiedDateTime</span></span>|<span data-ttu-id="b5f50-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5f50-235">DateTimeOffset</span></span>|<span data-ttu-id="b5f50-236">A hora em que o contato foi modificado.</span><span class="sxs-lookup"><span data-stu-id="b5f50-236">The time the contact was modified.</span></span> <span data-ttu-id="b5f50-237">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b5f50-237">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b5f50-238">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b5f50-238">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b5f50-239">manager</span><span class="sxs-lookup"><span data-stu-id="b5f50-239">manager</span></span>|<span data-ttu-id="b5f50-240">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-240">String</span></span>|<span data-ttu-id="b5f50-241">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-241">The name of the contact's manager.</span></span>
|<span data-ttu-id="b5f50-242">middleName</span><span class="sxs-lookup"><span data-stu-id="b5f50-242">middleName</span></span>|<span data-ttu-id="b5f50-243">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-243">String</span></span>|<span data-ttu-id="b5f50-244">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-244">The contact's middle name.</span></span>|
|<span data-ttu-id="b5f50-245">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b5f50-245">mobilePhone</span></span>|<span data-ttu-id="b5f50-246">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-246">String</span></span>|<span data-ttu-id="b5f50-247">O número de celular do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-247">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="b5f50-248">nickName</span><span class="sxs-lookup"><span data-stu-id="b5f50-248">nickName</span></span>|<span data-ttu-id="b5f50-249">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-249">String</span></span>|<span data-ttu-id="b5f50-250">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-250">The contact's nickname.</span></span>|
|<span data-ttu-id="b5f50-251">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b5f50-251">officeLocation</span></span>|<span data-ttu-id="b5f50-252">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-252">String</span></span>|<span data-ttu-id="b5f50-253">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-253">The location of the contact's office.</span></span>|
|<span data-ttu-id="b5f50-254">otherAddress</span><span class="sxs-lookup"><span data-stu-id="b5f50-254">otherAddress</span></span>|[<span data-ttu-id="b5f50-255">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="b5f50-255">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="b5f50-256">Outros endereços do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-256">Other addresses for the contact.</span></span>|
|<span data-ttu-id="b5f50-257">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="b5f50-257">parentFolderId</span></span>|<span data-ttu-id="b5f50-258">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-258">String</span></span>|<span data-ttu-id="b5f50-259">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-259">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="b5f50-260">personalNotes</span><span class="sxs-lookup"><span data-stu-id="b5f50-260">personalNotes</span></span>|<span data-ttu-id="b5f50-261">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-261">String</span></span>|<span data-ttu-id="b5f50-262">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-262">The user's notes about the contact.</span></span>|
|<span data-ttu-id="b5f50-263">profession</span><span class="sxs-lookup"><span data-stu-id="b5f50-263">profession</span></span>|<span data-ttu-id="b5f50-264">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-264">String</span></span>|<span data-ttu-id="b5f50-265">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-265">The contact's profession.</span></span>|
|<span data-ttu-id="b5f50-266">spouseName</span><span class="sxs-lookup"><span data-stu-id="b5f50-266">spouseName</span></span>|<span data-ttu-id="b5f50-267">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-267">String</span></span>|<span data-ttu-id="b5f50-268">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-268">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="b5f50-269">surname</span><span class="sxs-lookup"><span data-stu-id="b5f50-269">surname</span></span>|<span data-ttu-id="b5f50-270">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-270">String</span></span>|<span data-ttu-id="b5f50-271">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-271">The contact's surname.</span></span>|
|<span data-ttu-id="b5f50-272">title</span><span class="sxs-lookup"><span data-stu-id="b5f50-272">title</span></span>|<span data-ttu-id="b5f50-273">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-273">String</span></span>|<span data-ttu-id="b5f50-274">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-274">The contact's title.</span></span>|
|<span data-ttu-id="b5f50-275">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="b5f50-275">yomiCompanyName</span></span>|<span data-ttu-id="b5f50-276">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-276">String</span></span>|<span data-ttu-id="b5f50-277">O nome de empresa japonês fonético do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-277">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="b5f50-278">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="b5f50-278">yomiGivenName</span></span>|<span data-ttu-id="b5f50-279">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-279">String</span></span>|<span data-ttu-id="b5f50-280">O nome japonês fonético do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-280">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="b5f50-281">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="b5f50-281">yomiSurname</span></span>|<span data-ttu-id="b5f50-282">String</span><span class="sxs-lookup"><span data-stu-id="b5f50-282">String</span></span>|<span data-ttu-id="b5f50-283">O sobrenome japonês fonético do contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-283">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5f50-284">Relações</span><span class="sxs-lookup"><span data-stu-id="b5f50-284">Relationships</span></span>
| <span data-ttu-id="b5f50-285">Relação</span><span class="sxs-lookup"><span data-stu-id="b5f50-285">Relationship</span></span> | <span data-ttu-id="b5f50-286">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5f50-286">Type</span></span>   |<span data-ttu-id="b5f50-287">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5f50-287">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5f50-288">extensions</span><span class="sxs-lookup"><span data-stu-id="b5f50-288">extensions</span></span>|<span data-ttu-id="b5f50-289">Coleção [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="b5f50-289">[extension](extension.md) collection</span></span>|<span data-ttu-id="b5f50-p109">A coleção de extensões abertas definidas para o contato. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b5f50-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b5f50-293">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b5f50-293">multiValueExtendedProperties</span></span>|<span data-ttu-id="b5f50-294">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b5f50-294">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b5f50-p110">A coleção de propriedades estendidas de vários valores definidas para o contato. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b5f50-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b5f50-298">Foto</span><span class="sxs-lookup"><span data-stu-id="b5f50-298">photo</span></span>|[<span data-ttu-id="b5f50-299">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="b5f50-299">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="b5f50-p111">Imagem de contato opcional. Você pode obter ou definir uma foto de um contato.</span><span class="sxs-lookup"><span data-stu-id="b5f50-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="b5f50-302">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b5f50-302">singleValueExtendedProperties</span></span>|<span data-ttu-id="b5f50-303">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b5f50-303">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b5f50-p112">A coleção de propriedades estendidas de valor único definidas para o contato. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b5f50-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5f50-307">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5f50-307">JSON representation</span></span>

<span data-ttu-id="b5f50-308">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b5f50-308">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact",
  "@odata.annotations": [
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "businessAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHomePage": "string",
  "businessPhones": ["string"],
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.emailAddress"}],
  "fileAs": "string",
  "generation": "string",
  "givenName": "string",
  "homeAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "homePhones": ["string"],
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "mobilePhone": "string",
  "nickName": "string",
  "officeLocation": "string",
  "otherAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "parentFolderId": "string",
  "personalNotes": "string",
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string",

  "photo": { "@odata.type": "microsoft.graph.profilePhoto" }
}

```

## <a name="see-also"></a><span data-ttu-id="b5f50-309">Confira também</span><span class="sxs-lookup"><span data-stu-id="b5f50-309">See also</span></span>

- [<span data-ttu-id="b5f50-310">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b5f50-310">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="b5f50-311">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="b5f50-311">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="b5f50-312">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="b5f50-312">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b5f50-313">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="b5f50-313">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b5f50-314">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="b5f50-314">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

