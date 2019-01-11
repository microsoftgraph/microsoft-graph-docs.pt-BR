---
title: tipo de recurso contact
description: Um contato é um item no Outlook no qual você pode organizar e salvar informações sobre as pessoas e organizações com quem se comunica. Os contatos estão contidos em pastas de contatos.
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 6ff19278e6cf120404b892bb95881326ce281a72
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854373"
---
# <a name="contact-resource-type"></a><span data-ttu-id="eeb12-104">tipo de recurso contact</span><span class="sxs-lookup"><span data-stu-id="eeb12-104">contact resource type</span></span>

<span data-ttu-id="eeb12-p102">Um contato é um item no Outlook no qual você pode organizar e salvar informações sobre as pessoas e organizações com quem se comunica. Os contatos estão contidos em pastas de contatos.</span><span class="sxs-lookup"><span data-stu-id="eeb12-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="eeb12-107">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="eeb12-107">This resource supports:</span></span>

- <span data-ttu-id="eeb12-108">Adicionar seus próprios dados às propriedades personalizadas como [extensões](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="eeb12-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="eeb12-109">Assinatura de [notificações de alteração](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="eeb12-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="eeb12-110">Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contact-delta.md).</span><span class="sxs-lookup"><span data-stu-id="eeb12-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="eeb12-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="eeb12-111">Methods</span></span>

| <span data-ttu-id="eeb12-112">Método</span><span class="sxs-lookup"><span data-stu-id="eeb12-112">Method</span></span>       | <span data-ttu-id="eeb12-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eeb12-113">Return Type</span></span>  |<span data-ttu-id="eeb12-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb12-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eeb12-115">Obter contato</span><span class="sxs-lookup"><span data-stu-id="eeb12-115">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="eeb12-116">contact</span><span class="sxs-lookup"><span data-stu-id="eeb12-116">contact</span></span>](contact.md) |<span data-ttu-id="eeb12-117">Leia as propriedades e as relações do objeto contact.</span><span class="sxs-lookup"><span data-stu-id="eeb12-117">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="eeb12-118">Create</span><span class="sxs-lookup"><span data-stu-id="eeb12-118">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="eeb12-119">contact</span><span class="sxs-lookup"><span data-stu-id="eeb12-119">contact</span></span>](contact.md) |<span data-ttu-id="eeb12-120">Adicione um contato na pasta de Contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="eeb12-120">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="eeb12-121">Update</span><span class="sxs-lookup"><span data-stu-id="eeb12-121">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="eeb12-122">contact</span><span class="sxs-lookup"><span data-stu-id="eeb12-122">contact</span></span>](contact.md) |<span data-ttu-id="eeb12-123">Atualize o objeto contact.</span><span class="sxs-lookup"><span data-stu-id="eeb12-123">Update contact object.</span></span> |
|[<span data-ttu-id="eeb12-124">Delete</span><span class="sxs-lookup"><span data-stu-id="eeb12-124">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="eeb12-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="eeb12-125">None</span></span> |<span data-ttu-id="eeb12-126">Exclua um objeto contact.</span><span class="sxs-lookup"><span data-stu-id="eeb12-126">Delete contact object.</span></span> |
|[<span data-ttu-id="eeb12-127">delta</span><span class="sxs-lookup"><span data-stu-id="eeb12-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="eeb12-128">Coleção [Contact](contact.md)</span><span class="sxs-lookup"><span data-stu-id="eeb12-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="eeb12-129">Obtenha um conjunto de contatos que foram adicionados, excluídos ou atualizados em uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="eeb12-129">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="eeb12-130">**Extensões abertas**</span><span class="sxs-lookup"><span data-stu-id="eeb12-130">**Open extensions**</span></span>| | |
|[<span data-ttu-id="eeb12-131">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="eeb12-131">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="eeb12-132">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="eeb12-132">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="eeb12-133">Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="eeb12-133">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="eeb12-134">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="eeb12-134">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="eeb12-135">Coleção [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="eeb12-135">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="eeb12-136">Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="eeb12-136">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="eeb12-137">**Extensões de esquema**</span><span class="sxs-lookup"><span data-stu-id="eeb12-137">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="eeb12-138">Adicionar valores de extensões de esquema</span><span class="sxs-lookup"><span data-stu-id="eeb12-138">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="eeb12-139">Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.</span><span class="sxs-lookup"><span data-stu-id="eeb12-139">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="eeb12-140">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="eeb12-140">**Extended properties**</span></span>| | |
|[<span data-ttu-id="eeb12-141">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="eeb12-141">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="eeb12-142">contact</span><span class="sxs-lookup"><span data-stu-id="eeb12-142">contact</span></span>](contact.md)  |<span data-ttu-id="eeb12-143">Criar uma ou mais propriedades estendidas de valor único em um contato novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="eeb12-143">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="eeb12-144">Obter contato com propriedade estendida com valor único</span><span class="sxs-lookup"><span data-stu-id="eeb12-144">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="eeb12-145">contact</span><span class="sxs-lookup"><span data-stu-id="eeb12-145">contact</span></span>](contact.md) | <span data-ttu-id="eeb12-146">Obter contatos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="eeb12-146">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="eeb12-147">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="eeb12-147">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="eeb12-148">contact</span><span class="sxs-lookup"><span data-stu-id="eeb12-148">contact</span></span>](contact.md) | <span data-ttu-id="eeb12-149">Criar uma ou mais propriedades estendidas de vários valores em um contato novo ou existente.</span><span class="sxs-lookup"><span data-stu-id="eeb12-149">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="eeb12-150">Obter contato com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="eeb12-150">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="eeb12-151">contact</span><span class="sxs-lookup"><span data-stu-id="eeb12-151">contact</span></span>](contact.md) | <span data-ttu-id="eeb12-152">Obter um contato que contenha uma propriedade estendida de vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="eeb12-152">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="eeb12-153">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eeb12-153">Properties</span></span>
| <span data-ttu-id="eeb12-154">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eeb12-154">Property</span></span>     | <span data-ttu-id="eeb12-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeb12-155">Type</span></span>   |<span data-ttu-id="eeb12-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb12-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eeb12-157">assistantName</span><span class="sxs-lookup"><span data-stu-id="eeb12-157">assistantName</span></span>|<span data-ttu-id="eeb12-158">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-158">String</span></span>|<span data-ttu-id="eeb12-159">O nome do assistente do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-159">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="eeb12-160">birthday</span><span class="sxs-lookup"><span data-stu-id="eeb12-160">birthday</span></span>|<span data-ttu-id="eeb12-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeb12-161">DateTimeOffset</span></span>|<span data-ttu-id="eeb12-p103">O aniversário do contato. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eeb12-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="eeb12-165">businessAddress</span><span class="sxs-lookup"><span data-stu-id="eeb12-165">businessAddress</span></span>|[<span data-ttu-id="eeb12-166">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="eeb12-166">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="eeb12-167">O endereço comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-167">The contact's business address.</span></span>|
|<span data-ttu-id="eeb12-168">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="eeb12-168">businessHomePage</span></span>|<span data-ttu-id="eeb12-169">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-169">String</span></span>|<span data-ttu-id="eeb12-170">A home page comercial do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-170">The business home page of the contact.</span></span>|
|<span data-ttu-id="eeb12-171">businessPhones</span><span class="sxs-lookup"><span data-stu-id="eeb12-171">businessPhones</span></span>|<span data-ttu-id="eeb12-172">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eeb12-172">String collection</span></span>|<span data-ttu-id="eeb12-173">Os números de telefone comerciais do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-173">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="eeb12-174">categories</span><span class="sxs-lookup"><span data-stu-id="eeb12-174">categories</span></span>|<span data-ttu-id="eeb12-175">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eeb12-175">String collection</span></span>|<span data-ttu-id="eeb12-176">As categorias associadas ao contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-176">The categories associated with the contact.</span></span>|
|<span data-ttu-id="eeb12-177">changeKey</span><span class="sxs-lookup"><span data-stu-id="eeb12-177">changeKey</span></span>|<span data-ttu-id="eeb12-178">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-178">String</span></span>|<span data-ttu-id="eeb12-p104">Identifica a versão do contato. Toda vez que o contato muda, a ChangeKey também muda. Isso permite que o Exchange aplique alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="eeb12-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="eeb12-182">children</span><span class="sxs-lookup"><span data-stu-id="eeb12-182">children</span></span>|<span data-ttu-id="eeb12-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eeb12-183">String collection</span></span>|<span data-ttu-id="eeb12-184">Os nomes dos filhos do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-184">The names of the contact's children.</span></span>|
|<span data-ttu-id="eeb12-185">nomeDaEmpresa</span><span class="sxs-lookup"><span data-stu-id="eeb12-185">companyName</span></span>|<span data-ttu-id="eeb12-186">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-186">String</span></span>|<span data-ttu-id="eeb12-187">O nome da empresa do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-187">The name of the contact's company.</span></span>|
|<span data-ttu-id="eeb12-188">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eeb12-188">createdDateTime</span></span>|<span data-ttu-id="eeb12-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeb12-189">DateTimeOffset</span></span>|<span data-ttu-id="eeb12-p105">A hora em que o contato foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eeb12-p105">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="eeb12-193">department</span><span class="sxs-lookup"><span data-stu-id="eeb12-193">department</span></span>|<span data-ttu-id="eeb12-194">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-194">String</span></span>|<span data-ttu-id="eeb12-195">O departamento do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-195">The contact's department.</span></span>|
|<span data-ttu-id="eeb12-196">displayName</span><span class="sxs-lookup"><span data-stu-id="eeb12-196">displayName</span></span>|<span data-ttu-id="eeb12-197">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-197">String</span></span>|<span data-ttu-id="eeb12-198">O nome para exibição do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-198">The contact's display name.</span></span> <span data-ttu-id="eeb12-199">Você pode especificar o nome para exibição em uma operação de [criar](../api/user-post-contacts.md) ou [Atualizar](../api/contact-update.md) .</span><span class="sxs-lookup"><span data-stu-id="eeb12-199">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="eeb12-200">Observe que as atualizações posteriores a outras propriedades podem causar um valor gerado automaticamente substituir o valor displayName que você especificou.</span><span class="sxs-lookup"><span data-stu-id="eeb12-200">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="eeb12-201">Para preservar a um valor pré-existente, sempre incluí-lo como displayName em uma operação de [atualização](../api/contact-update.md) .</span><span class="sxs-lookup"><span data-stu-id="eeb12-201">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="eeb12-202">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="eeb12-202">emailAddresses</span></span>|<span data-ttu-id="eeb12-203">Coleção [EmailAddress](emailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="eeb12-203">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="eeb12-204">Os endereços de email do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-204">The contact's email addresses.</span></span>|
|<span data-ttu-id="eeb12-205">fileAs</span><span class="sxs-lookup"><span data-stu-id="eeb12-205">fileAs</span></span>|<span data-ttu-id="eeb12-206">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-206">String</span></span>|<span data-ttu-id="eeb12-207">O nome com o qual o contato está arquivado.</span><span class="sxs-lookup"><span data-stu-id="eeb12-207">The name the contact is filed under.</span></span>|
|<span data-ttu-id="eeb12-208">generation</span><span class="sxs-lookup"><span data-stu-id="eeb12-208">generation</span></span>|<span data-ttu-id="eeb12-209">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-209">String</span></span>|<span data-ttu-id="eeb12-210">A geração do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-210">The contact's generation.</span></span>|
|<span data-ttu-id="eeb12-211">givenName</span><span class="sxs-lookup"><span data-stu-id="eeb12-211">givenName</span></span>|<span data-ttu-id="eeb12-212">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-212">String</span></span>|<span data-ttu-id="eeb12-213">O nome do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-213">The contact's given name.</span></span>|
|<span data-ttu-id="eeb12-214">homeAddress</span><span class="sxs-lookup"><span data-stu-id="eeb12-214">homeAddress</span></span>|[<span data-ttu-id="eeb12-215">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="eeb12-215">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="eeb12-216">O endereço residencial do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-216">The contact's home address.</span></span>|
|<span data-ttu-id="eeb12-217">homePhones</span><span class="sxs-lookup"><span data-stu-id="eeb12-217">homePhones</span></span>|<span data-ttu-id="eeb12-218">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eeb12-218">String collection</span></span>|<span data-ttu-id="eeb12-219">Os números de telefone residenciais do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-219">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="eeb12-220">id</span><span class="sxs-lookup"><span data-stu-id="eeb12-220">id</span></span>|<span data-ttu-id="eeb12-221">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-221">String</span></span>|<span data-ttu-id="eeb12-p107">O identificador exclusivo do contato. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eeb12-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="eeb12-224">imAddresses</span><span class="sxs-lookup"><span data-stu-id="eeb12-224">imAddresses</span></span>|<span data-ttu-id="eeb12-225">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eeb12-225">String collection</span></span>|<span data-ttu-id="eeb12-226">Os endereços de mensagens instantâneas do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-226">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="eeb12-227">initials</span><span class="sxs-lookup"><span data-stu-id="eeb12-227">initials</span></span>|<span data-ttu-id="eeb12-228">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-228">String</span></span>|<span data-ttu-id="eeb12-229">As iniciais do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-229">The contact's initials.</span></span>|
|<span data-ttu-id="eeb12-230">jobTitle</span><span class="sxs-lookup"><span data-stu-id="eeb12-230">jobTitle</span></span>|<span data-ttu-id="eeb12-231">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-231">String</span></span>|<span data-ttu-id="eeb12-232">O cargo do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-232">The contact’s job title.</span></span>|
|<span data-ttu-id="eeb12-233">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eeb12-233">lastModifiedDateTime</span></span>|<span data-ttu-id="eeb12-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeb12-234">DateTimeOffset</span></span>|<span data-ttu-id="eeb12-p108">A hora em que o contato foi modificado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eeb12-p108">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="eeb12-238">manager</span><span class="sxs-lookup"><span data-stu-id="eeb12-238">manager</span></span>|<span data-ttu-id="eeb12-239">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-239">String</span></span>|<span data-ttu-id="eeb12-240">O nome do gerente do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-240">The name of the contact's manager.</span></span>
|<span data-ttu-id="eeb12-241">middleName</span><span class="sxs-lookup"><span data-stu-id="eeb12-241">middleName</span></span>|<span data-ttu-id="eeb12-242">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-242">String</span></span>|<span data-ttu-id="eeb12-243">O nome do meio do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-243">The contact's middle name.</span></span>|
|<span data-ttu-id="eeb12-244">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="eeb12-244">mobilePhone</span></span>|<span data-ttu-id="eeb12-245">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-245">String</span></span>|<span data-ttu-id="eeb12-246">O número de celular do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-246">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="eeb12-247">nickName</span><span class="sxs-lookup"><span data-stu-id="eeb12-247">nickName</span></span>|<span data-ttu-id="eeb12-248">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-248">String</span></span>|<span data-ttu-id="eeb12-249">O apelido do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-249">The contact's nickname.</span></span>|
|<span data-ttu-id="eeb12-250">officeLocation</span><span class="sxs-lookup"><span data-stu-id="eeb12-250">officeLocation</span></span>|<span data-ttu-id="eeb12-251">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-251">String</span></span>|<span data-ttu-id="eeb12-252">O local do escritório do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-252">The location of the contact's office.</span></span>|
|<span data-ttu-id="eeb12-253">otherAddress</span><span class="sxs-lookup"><span data-stu-id="eeb12-253">otherAddress</span></span>|[<span data-ttu-id="eeb12-254">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="eeb12-254">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="eeb12-255">Outros endereços do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-255">Other addresses for the contact.</span></span>|
|<span data-ttu-id="eeb12-256">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="eeb12-256">parentFolderId</span></span>|<span data-ttu-id="eeb12-257">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-257">String</span></span>|<span data-ttu-id="eeb12-258">A ID da pasta pai do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-258">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="eeb12-259">personalNotes</span><span class="sxs-lookup"><span data-stu-id="eeb12-259">personalNotes</span></span>|<span data-ttu-id="eeb12-260">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-260">String</span></span>|<span data-ttu-id="eeb12-261">As anotações do usuário sobre o contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-261">The user's notes about the contact.</span></span>|
|<span data-ttu-id="eeb12-262">profession</span><span class="sxs-lookup"><span data-stu-id="eeb12-262">profession</span></span>|<span data-ttu-id="eeb12-263">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-263">String</span></span>|<span data-ttu-id="eeb12-264">A profissão do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-264">The contact's profession.</span></span>|
|<span data-ttu-id="eeb12-265">spouseName</span><span class="sxs-lookup"><span data-stu-id="eeb12-265">spouseName</span></span>|<span data-ttu-id="eeb12-266">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-266">String</span></span>|<span data-ttu-id="eeb12-267">O nome do cônjuge/parceiro do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-267">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="eeb12-268">surname</span><span class="sxs-lookup"><span data-stu-id="eeb12-268">surname</span></span>|<span data-ttu-id="eeb12-269">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-269">String</span></span>|<span data-ttu-id="eeb12-270">O sobrenome do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-270">The contact's surname.</span></span>|
|<span data-ttu-id="eeb12-271">title</span><span class="sxs-lookup"><span data-stu-id="eeb12-271">title</span></span>|<span data-ttu-id="eeb12-272">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-272">String</span></span>|<span data-ttu-id="eeb12-273">O título do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-273">The contact's title.</span></span>|
|<span data-ttu-id="eeb12-274">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="eeb12-274">yomiCompanyName</span></span>|<span data-ttu-id="eeb12-275">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-275">String</span></span>|<span data-ttu-id="eeb12-276">O nome de empresa japonês fonético do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-276">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="eeb12-277">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="eeb12-277">yomiGivenName</span></span>|<span data-ttu-id="eeb12-278">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-278">String</span></span>|<span data-ttu-id="eeb12-279">O nome japonês fonético do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-279">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="eeb12-280">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="eeb12-280">yomiSurname</span></span>|<span data-ttu-id="eeb12-281">String</span><span class="sxs-lookup"><span data-stu-id="eeb12-281">String</span></span>|<span data-ttu-id="eeb12-282">O sobrenome japonês fonético do contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-282">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eeb12-283">Relações</span><span class="sxs-lookup"><span data-stu-id="eeb12-283">Relationships</span></span>
| <span data-ttu-id="eeb12-284">Relação</span><span class="sxs-lookup"><span data-stu-id="eeb12-284">Relationship</span></span> | <span data-ttu-id="eeb12-285">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeb12-285">Type</span></span>   |<span data-ttu-id="eeb12-286">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb12-286">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eeb12-287">extensions</span><span class="sxs-lookup"><span data-stu-id="eeb12-287">extensions</span></span>|<span data-ttu-id="eeb12-288">Coleção [extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="eeb12-288">[extension](extension.md) collection</span></span>|<span data-ttu-id="eeb12-p109">A coleção de extensões abertas definidas para o contato. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="eeb12-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="eeb12-292">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="eeb12-292">multiValueExtendedProperties</span></span>|<span data-ttu-id="eeb12-293">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="eeb12-293">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="eeb12-p110">A coleção de propriedades estendidas de vários valores definidas para o contato. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="eeb12-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="eeb12-297">Foto</span><span class="sxs-lookup"><span data-stu-id="eeb12-297">photo</span></span>|[<span data-ttu-id="eeb12-298">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="eeb12-298">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="eeb12-p111">Imagem de contato opcional. Você pode obter ou definir uma foto de um contato.</span><span class="sxs-lookup"><span data-stu-id="eeb12-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="eeb12-301">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="eeb12-301">singleValueExtendedProperties</span></span>|<span data-ttu-id="eeb12-302">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="eeb12-302">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="eeb12-p112">A coleção de propriedades estendidas de valor único definidas para o contato. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="eeb12-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eeb12-306">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eeb12-306">JSON representation</span></span>

<span data-ttu-id="eeb12-307">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="eeb12-307">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="eeb12-308">Confira também</span><span class="sxs-lookup"><span data-stu-id="eeb12-308">See also</span></span>

- [<span data-ttu-id="eeb12-309">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="eeb12-309">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="eeb12-310">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="eeb12-310">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="eeb12-311">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="eeb12-311">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="eeb12-312">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="eeb12-312">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="eeb12-313">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="eeb12-313">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
