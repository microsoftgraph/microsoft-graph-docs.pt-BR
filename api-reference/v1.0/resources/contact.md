---
title: tipo de recurso contact
description: Um contato é um item no Outlook no qual você pode organizar e salvar informações sobre as pessoas e organizações com quem se comunica. Os contatos estão contidos em pastas de contatos.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ab0236f92075398f2131b40f14c45bfe215b6ea0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029656"
---
# <a name="contact-resource-type"></a><span data-ttu-id="f353f-104">tipo de recurso contact</span><span class="sxs-lookup"><span data-stu-id="f353f-104">contact resource type</span></span>

<span data-ttu-id="f353f-p102">Um contato é um item no Outlook no qual você pode organizar e salvar informações sobre as pessoas e organizações com quem se comunica. Os contatos estão contidos em pastas de contatos.</span><span class="sxs-lookup"><span data-stu-id="f353f-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="f353f-107">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="f353f-107">This resource supports:</span></span>

- <span data-ttu-id="f353f-108">Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="f353f-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="f353f-109">Assinar as [notificações de alteração](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="f353f-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="f353f-110">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contact-delta.md).</span><span class="sxs-lookup"><span data-stu-id="f353f-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="f353f-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="f353f-111">Methods</span></span>

| <span data-ttu-id="f353f-112">Método</span><span class="sxs-lookup"><span data-stu-id="f353f-112">Method</span></span>       | <span data-ttu-id="f353f-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f353f-113">Return Type</span></span>  |<span data-ttu-id="f353f-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f353f-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f353f-115">Obter contato</span><span class="sxs-lookup"><span data-stu-id="f353f-115">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="f353f-116">contact</span><span class="sxs-lookup"><span data-stu-id="f353f-116">contact</span></span>](contact.md) |<span data-ttu-id="f353f-117">Leia as propriedades e as relações do objeto contact.</span><span class="sxs-lookup"><span data-stu-id="f353f-117">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="f353f-118">Create</span><span class="sxs-lookup"><span data-stu-id="f353f-118">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="f353f-119">contact</span><span class="sxs-lookup"><span data-stu-id="f353f-119">contact</span></span>](contact.md) |<span data-ttu-id="f353f-120">Adicione um contato na pasta de Contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="f353f-120">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="f353f-121">Update</span><span class="sxs-lookup"><span data-stu-id="f353f-121">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="f353f-122">contact</span><span class="sxs-lookup"><span data-stu-id="f353f-122">contact</span></span>](contact.md) |<span data-ttu-id="f353f-123">Atualize o objeto contact.</span><span class="sxs-lookup"><span data-stu-id="f353f-123">Update contact object.</span></span> |
|[<span data-ttu-id="f353f-124">Delete</span><span class="sxs-lookup"><span data-stu-id="f353f-124">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="f353f-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f353f-125">None</span></span> |<span data-ttu-id="f353f-126">Exclua um objeto contact.</span><span class="sxs-lookup"><span data-stu-id="f353f-126">Delete contact object.</span></span> |
|[<span data-ttu-id="f353f-127">delta</span><span class="sxs-lookup"><span data-stu-id="f353f-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="f353f-128">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="f353f-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="f353f-129">Obtenha um conjunto de contatos que foram adicionados, excluídos ou atualizados em uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="f353f-129">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="f353f-130">**Extensões abertas**</span><span class="sxs-lookup"><span data-stu-id="f353f-130">**Open extensions**</span></span>| | |
|[<span data-ttu-id="f353f-131">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="f353f-131">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="f353f-132">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="f353f-132">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="f353f-133">Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="f353f-133">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="f353f-134">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="f353f-134">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="f353f-135">Coleção [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="f353f-135">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="f353f-136">Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="f353f-136">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="f353f-137">**Extensões de esquema**</span><span class="sxs-lookup"><span data-stu-id="f353f-137">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="f353f-138">Adicionar valores de extensões de esquema</span><span class="sxs-lookup"><span data-stu-id="f353f-138">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="f353f-139">Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.</span><span class="sxs-lookup"><span data-stu-id="f353f-139">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="f353f-140">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="f353f-140">**Extended properties**</span></span>| | |
|[<span data-ttu-id="f353f-141">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="f353f-141">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="f353f-142">contact</span><span class="sxs-lookup"><span data-stu-id="f353f-142">contact</span></span>](contact.md)  |<span data-ttu-id="f353f-143">Criar uma ou mais propriedades estendidas de valor único em um contato novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="f353f-143">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="f353f-144">Obter contato com propriedade estendida com valor único</span><span class="sxs-lookup"><span data-stu-id="f353f-144">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="f353f-145">contact</span><span class="sxs-lookup"><span data-stu-id="f353f-145">contact</span></span>](contact.md) | <span data-ttu-id="f353f-146">Obter contatos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f353f-146">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="f353f-147">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="f353f-147">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="f353f-148">contact</span><span class="sxs-lookup"><span data-stu-id="f353f-148">contact</span></span>](contact.md) | <span data-ttu-id="f353f-149">Criar uma ou mais propriedades estendidas de vários valores em um contato novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="f353f-149">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="f353f-150">Obter contato com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="f353f-150">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="f353f-151">contact</span><span class="sxs-lookup"><span data-stu-id="f353f-151">contact</span></span>](contact.md) | <span data-ttu-id="f353f-152">Obter um contato que contenha uma propriedade estendida de vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="f353f-152">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="f353f-153">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f353f-153">Properties</span></span>
| <span data-ttu-id="f353f-154">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f353f-154">Property</span></span>     | <span data-ttu-id="f353f-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="f353f-155">Type</span></span>   |<span data-ttu-id="f353f-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="f353f-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f353f-157">assistantName</span><span class="sxs-lookup"><span data-stu-id="f353f-157">assistantName</span></span>|<span data-ttu-id="f353f-158">String</span><span class="sxs-lookup"><span data-stu-id="f353f-158">String</span></span>|<span data-ttu-id="f353f-159">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-159">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="f353f-160">birthday</span><span class="sxs-lookup"><span data-stu-id="f353f-160">birthday</span></span>|<span data-ttu-id="f353f-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f353f-161">DateTimeOffset</span></span>|<span data-ttu-id="f353f-p103">O aniversário do contato. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f353f-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f353f-165">businessAddress</span><span class="sxs-lookup"><span data-stu-id="f353f-165">businessAddress</span></span>|[<span data-ttu-id="f353f-166">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="f353f-166">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="f353f-167">O endereço comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-167">The contact's business address.</span></span>|
|<span data-ttu-id="f353f-168">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="f353f-168">businessHomePage</span></span>|<span data-ttu-id="f353f-169">String</span><span class="sxs-lookup"><span data-stu-id="f353f-169">String</span></span>|<span data-ttu-id="f353f-170">A home page comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-170">The business home page of the contact.</span></span>|
|<span data-ttu-id="f353f-171">businessPhones</span><span class="sxs-lookup"><span data-stu-id="f353f-171">businessPhones</span></span>|<span data-ttu-id="f353f-172">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f353f-172">String collection</span></span>|<span data-ttu-id="f353f-173">Os números de telefone comerciais do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-173">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="f353f-174">categories</span><span class="sxs-lookup"><span data-stu-id="f353f-174">categories</span></span>|<span data-ttu-id="f353f-175">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f353f-175">String collection</span></span>|<span data-ttu-id="f353f-176">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-176">The categories associated with the contact.</span></span>|
|<span data-ttu-id="f353f-177">changeKey</span><span class="sxs-lookup"><span data-stu-id="f353f-177">changeKey</span></span>|<span data-ttu-id="f353f-178">String</span><span class="sxs-lookup"><span data-stu-id="f353f-178">String</span></span>|<span data-ttu-id="f353f-p104">Identifica a versão do contato. Toda vez que o contato muda, a ChangeKey também muda. Isso permite que o Exchange aplique alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="f353f-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="f353f-182">children</span><span class="sxs-lookup"><span data-stu-id="f353f-182">children</span></span>|<span data-ttu-id="f353f-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f353f-183">String collection</span></span>|<span data-ttu-id="f353f-184">Os nomes dos filhos do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-184">The names of the contact's children.</span></span>|
|<span data-ttu-id="f353f-185">nomeDaEmpresa</span><span class="sxs-lookup"><span data-stu-id="f353f-185">companyName</span></span>|<span data-ttu-id="f353f-186">String</span><span class="sxs-lookup"><span data-stu-id="f353f-186">String</span></span>|<span data-ttu-id="f353f-187">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-187">The name of the contact's company.</span></span>|
|<span data-ttu-id="f353f-188">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f353f-188">createdDateTime</span></span>|<span data-ttu-id="f353f-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f353f-189">DateTimeOffset</span></span>|<span data-ttu-id="f353f-p105">A hora em que o contato foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f353f-p105">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f353f-193">department</span><span class="sxs-lookup"><span data-stu-id="f353f-193">department</span></span>|<span data-ttu-id="f353f-194">String</span><span class="sxs-lookup"><span data-stu-id="f353f-194">String</span></span>|<span data-ttu-id="f353f-195">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-195">The contact's department.</span></span>|
|<span data-ttu-id="f353f-196">displayName</span><span class="sxs-lookup"><span data-stu-id="f353f-196">displayName</span></span>|<span data-ttu-id="f353f-197">String</span><span class="sxs-lookup"><span data-stu-id="f353f-197">String</span></span>|<span data-ttu-id="f353f-198">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-198">The contact's display name.</span></span> <span data-ttu-id="f353f-199">Você pode especificar o nome de exibição em uma operação [criar](../api/user-post-contacts.md) ou [atualizar](../api/contact-update.md).</span><span class="sxs-lookup"><span data-stu-id="f353f-199">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="f353f-200">Observe que atualizações posteriores em outras propriedades podem fazer com que um valor gerado automaticamente sobrescreva o valor de displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="f353f-200">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="f353f-201">Para preservar a um valor preexistente, inclua-o como o displayName na operação [atualizar](../api/contact-update.md).</span><span class="sxs-lookup"><span data-stu-id="f353f-201">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="f353f-202">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="f353f-202">emailAddresses</span></span>|<span data-ttu-id="f353f-203">Coleção [EmailAddress](emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="f353f-203">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="f353f-204">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-204">The contact's email addresses.</span></span>|
|<span data-ttu-id="f353f-205">fileAs</span><span class="sxs-lookup"><span data-stu-id="f353f-205">fileAs</span></span>|<span data-ttu-id="f353f-206">String</span><span class="sxs-lookup"><span data-stu-id="f353f-206">String</span></span>|<span data-ttu-id="f353f-207">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="f353f-207">The name the contact is filed under.</span></span>|
|<span data-ttu-id="f353f-208">generation</span><span class="sxs-lookup"><span data-stu-id="f353f-208">generation</span></span>|<span data-ttu-id="f353f-209">String</span><span class="sxs-lookup"><span data-stu-id="f353f-209">String</span></span>|<span data-ttu-id="f353f-210">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-210">The contact's generation.</span></span>|
|<span data-ttu-id="f353f-211">givenName</span><span class="sxs-lookup"><span data-stu-id="f353f-211">givenName</span></span>|<span data-ttu-id="f353f-212">String</span><span class="sxs-lookup"><span data-stu-id="f353f-212">String</span></span>|<span data-ttu-id="f353f-213">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-213">The contact's given name.</span></span>|
|<span data-ttu-id="f353f-214">homeAddress</span><span class="sxs-lookup"><span data-stu-id="f353f-214">homeAddress</span></span>|[<span data-ttu-id="f353f-215">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="f353f-215">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="f353f-216">O endereço residencial do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-216">The contact's home address.</span></span>|
|<span data-ttu-id="f353f-217">homePhones</span><span class="sxs-lookup"><span data-stu-id="f353f-217">homePhones</span></span>|<span data-ttu-id="f353f-218">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f353f-218">String collection</span></span>|<span data-ttu-id="f353f-219">Os números de telefone residenciais do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-219">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="f353f-220">id</span><span class="sxs-lookup"><span data-stu-id="f353f-220">id</span></span>|<span data-ttu-id="f353f-221">String</span><span class="sxs-lookup"><span data-stu-id="f353f-221">String</span></span>|<span data-ttu-id="f353f-p107">O identificador exclusivo do contato. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f353f-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="f353f-224">imAddresses</span><span class="sxs-lookup"><span data-stu-id="f353f-224">imAddresses</span></span>|<span data-ttu-id="f353f-225">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f353f-225">String collection</span></span>|<span data-ttu-id="f353f-226">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-226">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="f353f-227">initials</span><span class="sxs-lookup"><span data-stu-id="f353f-227">initials</span></span>|<span data-ttu-id="f353f-228">String</span><span class="sxs-lookup"><span data-stu-id="f353f-228">String</span></span>|<span data-ttu-id="f353f-229">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-229">The contact's initials.</span></span>|
|<span data-ttu-id="f353f-230">jobTitle</span><span class="sxs-lookup"><span data-stu-id="f353f-230">jobTitle</span></span>|<span data-ttu-id="f353f-231">String</span><span class="sxs-lookup"><span data-stu-id="f353f-231">String</span></span>|<span data-ttu-id="f353f-232">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-232">The contact’s job title.</span></span>|
|<span data-ttu-id="f353f-233">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f353f-233">lastModifiedDateTime</span></span>|<span data-ttu-id="f353f-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f353f-234">DateTimeOffset</span></span>|<span data-ttu-id="f353f-p108">A hora em que o contato foi modificado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f353f-p108">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f353f-238">manager</span><span class="sxs-lookup"><span data-stu-id="f353f-238">manager</span></span>|<span data-ttu-id="f353f-239">String</span><span class="sxs-lookup"><span data-stu-id="f353f-239">String</span></span>|<span data-ttu-id="f353f-240">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-240">The name of the contact's manager.</span></span>
|<span data-ttu-id="f353f-241">middleName</span><span class="sxs-lookup"><span data-stu-id="f353f-241">middleName</span></span>|<span data-ttu-id="f353f-242">String</span><span class="sxs-lookup"><span data-stu-id="f353f-242">String</span></span>|<span data-ttu-id="f353f-243">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-243">The contact's middle name.</span></span>|
|<span data-ttu-id="f353f-244">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="f353f-244">mobilePhone</span></span>|<span data-ttu-id="f353f-245">String</span><span class="sxs-lookup"><span data-stu-id="f353f-245">String</span></span>|<span data-ttu-id="f353f-246">O número de celular do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-246">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="f353f-247">nickName</span><span class="sxs-lookup"><span data-stu-id="f353f-247">nickName</span></span>|<span data-ttu-id="f353f-248">String</span><span class="sxs-lookup"><span data-stu-id="f353f-248">String</span></span>|<span data-ttu-id="f353f-249">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-249">The contact's nickname.</span></span>|
|<span data-ttu-id="f353f-250">officeLocation</span><span class="sxs-lookup"><span data-stu-id="f353f-250">officeLocation</span></span>|<span data-ttu-id="f353f-251">String</span><span class="sxs-lookup"><span data-stu-id="f353f-251">String</span></span>|<span data-ttu-id="f353f-252">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-252">The location of the contact's office.</span></span>|
|<span data-ttu-id="f353f-253">otherAddress</span><span class="sxs-lookup"><span data-stu-id="f353f-253">otherAddress</span></span>|[<span data-ttu-id="f353f-254">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="f353f-254">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="f353f-255">Outros endereços do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-255">Other addresses for the contact.</span></span>|
|<span data-ttu-id="f353f-256">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="f353f-256">parentFolderId</span></span>|<span data-ttu-id="f353f-257">String</span><span class="sxs-lookup"><span data-stu-id="f353f-257">String</span></span>|<span data-ttu-id="f353f-258">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-258">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="f353f-259">personalNotes</span><span class="sxs-lookup"><span data-stu-id="f353f-259">personalNotes</span></span>|<span data-ttu-id="f353f-260">String</span><span class="sxs-lookup"><span data-stu-id="f353f-260">String</span></span>|<span data-ttu-id="f353f-261">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-261">The user's notes about the contact.</span></span>|
|<span data-ttu-id="f353f-262">profession</span><span class="sxs-lookup"><span data-stu-id="f353f-262">profession</span></span>|<span data-ttu-id="f353f-263">String</span><span class="sxs-lookup"><span data-stu-id="f353f-263">String</span></span>|<span data-ttu-id="f353f-264">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-264">The contact's profession.</span></span>|
|<span data-ttu-id="f353f-265">spouseName</span><span class="sxs-lookup"><span data-stu-id="f353f-265">spouseName</span></span>|<span data-ttu-id="f353f-266">String</span><span class="sxs-lookup"><span data-stu-id="f353f-266">String</span></span>|<span data-ttu-id="f353f-267">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-267">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="f353f-268">surname</span><span class="sxs-lookup"><span data-stu-id="f353f-268">surname</span></span>|<span data-ttu-id="f353f-269">String</span><span class="sxs-lookup"><span data-stu-id="f353f-269">String</span></span>|<span data-ttu-id="f353f-270">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-270">The contact's surname.</span></span>|
|<span data-ttu-id="f353f-271">title</span><span class="sxs-lookup"><span data-stu-id="f353f-271">title</span></span>|<span data-ttu-id="f353f-272">String</span><span class="sxs-lookup"><span data-stu-id="f353f-272">String</span></span>|<span data-ttu-id="f353f-273">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-273">The contact's title.</span></span>|
|<span data-ttu-id="f353f-274">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="f353f-274">yomiCompanyName</span></span>|<span data-ttu-id="f353f-275">String</span><span class="sxs-lookup"><span data-stu-id="f353f-275">String</span></span>|<span data-ttu-id="f353f-276">O nome de empresa japonês fonético do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-276">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="f353f-277">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="f353f-277">yomiGivenName</span></span>|<span data-ttu-id="f353f-278">String</span><span class="sxs-lookup"><span data-stu-id="f353f-278">String</span></span>|<span data-ttu-id="f353f-279">O nome japonês fonético do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-279">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="f353f-280">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="f353f-280">yomiSurname</span></span>|<span data-ttu-id="f353f-281">String</span><span class="sxs-lookup"><span data-stu-id="f353f-281">String</span></span>|<span data-ttu-id="f353f-282">O sobrenome japonês fonético do contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-282">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f353f-283">Relações</span><span class="sxs-lookup"><span data-stu-id="f353f-283">Relationships</span></span>
| <span data-ttu-id="f353f-284">Relação</span><span class="sxs-lookup"><span data-stu-id="f353f-284">Relationship</span></span> | <span data-ttu-id="f353f-285">Tipo</span><span class="sxs-lookup"><span data-stu-id="f353f-285">Type</span></span>   |<span data-ttu-id="f353f-286">Descrição</span><span class="sxs-lookup"><span data-stu-id="f353f-286">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f353f-287">extensions</span><span class="sxs-lookup"><span data-stu-id="f353f-287">extensions</span></span>|<span data-ttu-id="f353f-288">Coleção [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="f353f-288">[extension](extension.md) collection</span></span>|<span data-ttu-id="f353f-p109">A coleção de extensões abertas definidas para o contato. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="f353f-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="f353f-292">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="f353f-292">multiValueExtendedProperties</span></span>|<span data-ttu-id="f353f-293">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f353f-293">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="f353f-p110">A coleção de propriedades estendidas de vários valores definidas para o contato. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="f353f-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="f353f-297">Foto</span><span class="sxs-lookup"><span data-stu-id="f353f-297">photo</span></span>|[<span data-ttu-id="f353f-298">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="f353f-298">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="f353f-p111">Imagem de contato opcional. Você pode obter ou definir uma foto de um contato.</span><span class="sxs-lookup"><span data-stu-id="f353f-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="f353f-301">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="f353f-301">singleValueExtendedProperties</span></span>|<span data-ttu-id="f353f-302">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f353f-302">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="f353f-p112">A coleção de propriedades estendidas de valor único definidas para o contato. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="f353f-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f353f-306">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f353f-306">JSON representation</span></span>

<span data-ttu-id="f353f-307">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f353f-307">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="f353f-308">Confira também</span><span class="sxs-lookup"><span data-stu-id="f353f-308">See also</span></span>

- [<span data-ttu-id="f353f-309">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f353f-309">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="f353f-310">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="f353f-310">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="f353f-311">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="f353f-311">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f353f-312">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="f353f-312">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f353f-313">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="f353f-313">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
