---
title: Tipo de recurso person
description: Uma agregação de informações sobre uma pessoa através de email, contatos e redes sociais. As pessoas podem ser contatos locais, contatos de redes sociais, diretório da sua organização e pessoas de comunicações recentes (como email e Skype).
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: cc63a75af497a2402955c39a2bcfc8efe370c782
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998037"
---
# <a name="person-resource-type"></a><span data-ttu-id="7b8b5-104">Tipo de recurso person</span><span class="sxs-lookup"><span data-stu-id="7b8b5-104">person resource type</span></span>

<span data-ttu-id="7b8b5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b8b5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b8b5-p102">Uma agregação de informações sobre uma pessoa através de email, contatos e redes sociais. As pessoas podem ser contatos locais, contatos de redes sociais, diretório da sua organização e pessoas de comunicações recentes (como email e Skype).</span><span class="sxs-lookup"><span data-stu-id="7b8b5-p102">An aggregation of information about a person from across mail, contacts and social networks. People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="7b8b5-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7b8b5-108">Methods</span></span>

| <span data-ttu-id="7b8b5-109">Método</span><span class="sxs-lookup"><span data-stu-id="7b8b5-109">Method</span></span> | <span data-ttu-id="7b8b5-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b8b5-110">Return Type</span></span> | <span data-ttu-id="7b8b5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b8b5-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b8b5-112">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="7b8b5-112">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="7b8b5-113">**person**</span><span class="sxs-lookup"><span data-stu-id="7b8b5-113">**person**</span></span> |<span data-ttu-id="7b8b5-114">Obtém uma coleção de objetos person ordenados por relevância para o [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="7b8b5-114">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="7b8b5-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b8b5-115">Properties</span></span>

| <span data-ttu-id="7b8b5-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b8b5-116">Property</span></span> | <span data-ttu-id="7b8b5-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b8b5-117">Type</span></span> | <span data-ttu-id="7b8b5-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b8b5-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7b8b5-119">birthday</span><span class="sxs-lookup"><span data-stu-id="7b8b5-119">birthday</span></span>|<span data-ttu-id="7b8b5-120">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-120">string</span></span>|<span data-ttu-id="7b8b5-121">O aniversário da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-121">The person's birthday.</span></span>|
|<span data-ttu-id="7b8b5-122">companyName</span><span class="sxs-lookup"><span data-stu-id="7b8b5-122">companyName</span></span>|<span data-ttu-id="7b8b5-123">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-123">string</span></span>|<span data-ttu-id="7b8b5-124">O nome da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-124">The name of the person's company.</span></span>|
|<span data-ttu-id="7b8b5-125">departamento</span><span class="sxs-lookup"><span data-stu-id="7b8b5-125">department</span></span>|<span data-ttu-id="7b8b5-126">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-126">string</span></span>|<span data-ttu-id="7b8b5-127">O departamento da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-127">The person's department.</span></span>|
|<span data-ttu-id="7b8b5-128">displayName</span><span class="sxs-lookup"><span data-stu-id="7b8b5-128">displayName</span></span>|<span data-ttu-id="7b8b5-129">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-129">string</span></span>|<span data-ttu-id="7b8b5-130">O nome de exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-130">The person's display name.</span></span>|
|<span data-ttu-id="7b8b5-131">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="7b8b5-131">emailAddresses</span></span>|<span data-ttu-id="7b8b5-132">coleção [rankedEmailAddress](rankedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="7b8b5-132">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="7b8b5-133">Os endereços de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-133">The person's email addresses.</span></span>|
|<span data-ttu-id="7b8b5-134">givenName</span><span class="sxs-lookup"><span data-stu-id="7b8b5-134">givenName</span></span>|<span data-ttu-id="7b8b5-135">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-135">string</span></span>|<span data-ttu-id="7b8b5-136">O nome fornecido da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-136">The person's given name.</span></span>|
|<span data-ttu-id="7b8b5-137">id</span><span class="sxs-lookup"><span data-stu-id="7b8b5-137">id</span></span>|<span data-ttu-id="7b8b5-138">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-138">string</span></span>|<span data-ttu-id="7b8b5-p103">O identificador exclusivo da pessoa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="7b8b5-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="7b8b5-141">isFavorite</span></span>|<span data-ttu-id="7b8b5-142">booliano</span><span class="sxs-lookup"><span data-stu-id="7b8b5-142">boolean</span></span>|<span data-ttu-id="7b8b5-143">`true` se o usuário tiver sinalizado essa pessoa como um favorito.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="7b8b5-144">mailboxType</span><span class="sxs-lookup"><span data-stu-id="7b8b5-144">mailboxType</span></span>|<span data-ttu-id="7b8b5-145">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-145">string</span></span>|<span data-ttu-id="7b8b5-146">O tipo de caixa de correio que é representado pelo endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-146">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="7b8b5-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="7b8b5-147">officeLocation</span></span>|<span data-ttu-id="7b8b5-148">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-148">string</span></span>|<span data-ttu-id="7b8b5-149">O local do escritório da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-149">The location of the person's office.</span></span>|
|<span data-ttu-id="7b8b5-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="7b8b5-150">personNotes</span></span>|<span data-ttu-id="7b8b5-151">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-151">string</span></span>|<span data-ttu-id="7b8b5-152">As anotações de forma livre que o usuário fez sobre essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="7b8b5-153">personType</span><span class="sxs-lookup"><span data-stu-id="7b8b5-153">personType</span></span>|<span data-ttu-id="7b8b5-154">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-154">string</span></span>|<span data-ttu-id="7b8b5-155">O tipo de pessoa, por exemplo, lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-155">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="7b8b5-156">telefones</span><span class="sxs-lookup"><span data-stu-id="7b8b5-156">phones</span></span>|<span data-ttu-id="7b8b5-157">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="7b8b5-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="7b8b5-158">Os números de telefone da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="7b8b5-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="7b8b5-159">postalAddresses</span></span>|<span data-ttu-id="7b8b5-160">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="7b8b5-160">[location](location.md) collection</span></span>|<span data-ttu-id="7b8b5-161">Os endereços da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-161">The person's addresses.</span></span>|
|<span data-ttu-id="7b8b5-162">profession</span><span class="sxs-lookup"><span data-stu-id="7b8b5-162">profession</span></span>|<span data-ttu-id="7b8b5-163">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-163">string</span></span>|<span data-ttu-id="7b8b5-164">A profissão da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-164">The person's profession.</span></span>|
|<span data-ttu-id="7b8b5-165">fontes</span><span class="sxs-lookup"><span data-stu-id="7b8b5-165">sources</span></span>|<span data-ttu-id="7b8b5-166">coleção [personDataSource](persondatasource.md)</span><span class="sxs-lookup"><span data-stu-id="7b8b5-166">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="7b8b5-167">As fontes das quais os dados do usuário são provenientes, por exemplo, contatos do Outlook ou do Outlook.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-167">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="7b8b5-168">surname</span><span class="sxs-lookup"><span data-stu-id="7b8b5-168">surname</span></span>|<span data-ttu-id="7b8b5-169">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-169">string</span></span>|<span data-ttu-id="7b8b5-170">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-170">The person's surname.</span></span>|
|<span data-ttu-id="7b8b5-171">title</span><span class="sxs-lookup"><span data-stu-id="7b8b5-171">title</span></span>|<span data-ttu-id="7b8b5-172">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-172">string</span></span>|<span data-ttu-id="7b8b5-173">O título da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-173">The person's title.</span></span>|
|<span data-ttu-id="7b8b5-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7b8b5-174">userPrincipalName</span></span>|<span data-ttu-id="7b8b5-175">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-175">string</span></span>|<span data-ttu-id="7b8b5-p104">O nome UPN da pessoa. O UPN é um nome de logon para a pessoa ao estilo da Internet com base na [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email da pessoa. O formato geral é alias@domínio.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="7b8b5-180">websites</span><span class="sxs-lookup"><span data-stu-id="7b8b5-180">websites</span></span>|<span data-ttu-id="7b8b5-181">Coleção [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="7b8b5-181">[website](website.md) collection</span></span>|<span data-ttu-id="7b8b5-182">Os sites da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-182">The person's websites.</span></span>|
|<span data-ttu-id="7b8b5-183">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="7b8b5-183">yomiCompany</span></span>|<span data-ttu-id="7b8b5-184">string</span><span class="sxs-lookup"><span data-stu-id="7b8b5-184">string</span></span>|<span data-ttu-id="7b8b5-185">O nome japonês fonético da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-185">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b8b5-186">Relações</span><span class="sxs-lookup"><span data-stu-id="7b8b5-186">Relationships</span></span>

<span data-ttu-id="7b8b5-187">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b8b5-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b8b5-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b8b5-188">JSON representation</span></span>

<span data-ttu-id="7b8b5-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b8b5-189">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


