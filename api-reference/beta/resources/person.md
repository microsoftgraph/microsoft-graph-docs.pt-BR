---
title: Tipo de recurso person
description: Uma agregação de informações sobre uma pessoa através de email, contatos e redes sociais. As pessoas podem ser contatos locais, contatos de redes sociais, diretório da sua organização e pessoas de comunicações recentes (como email e Skype).
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4df5f82bd14ba56969c26facef82b59f3ac7e3f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521936"
---
# <a name="person-resource-type"></a><span data-ttu-id="c908c-104">Tipo de recurso person</span><span class="sxs-lookup"><span data-stu-id="c908c-104">person resource type</span></span>

<span data-ttu-id="c908c-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c908c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c908c-106">Uma agregação de informações sobre uma pessoa através de email, contatos e redes sociais.</span><span class="sxs-lookup"><span data-stu-id="c908c-106">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="c908c-107">As pessoas podem ser contatos locais, contatos de redes sociais, diretório da sua organização e pessoas de comunicações recentes (como email e Skype).</span><span class="sxs-lookup"><span data-stu-id="c908c-107">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="c908c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c908c-108">Methods</span></span>

| <span data-ttu-id="c908c-109">Método</span><span class="sxs-lookup"><span data-stu-id="c908c-109">Method</span></span> | <span data-ttu-id="c908c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c908c-110">Return Type</span></span> | <span data-ttu-id="c908c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c908c-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="c908c-112">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="c908c-112">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="c908c-113">**person**</span><span class="sxs-lookup"><span data-stu-id="c908c-113">**person**</span></span> |<span data-ttu-id="c908c-114">Obtém uma coleção de objetos person ordenados por relevância para o [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="c908c-114">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="c908c-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c908c-115">Properties</span></span>

| <span data-ttu-id="c908c-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c908c-116">Property</span></span> | <span data-ttu-id="c908c-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="c908c-117">Type</span></span> | <span data-ttu-id="c908c-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="c908c-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c908c-119">birthday</span><span class="sxs-lookup"><span data-stu-id="c908c-119">birthday</span></span>|<span data-ttu-id="c908c-120">string</span><span class="sxs-lookup"><span data-stu-id="c908c-120">string</span></span>|<span data-ttu-id="c908c-121">O aniversário da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-121">The person's birthday.</span></span>|
|<span data-ttu-id="c908c-122">companyName</span><span class="sxs-lookup"><span data-stu-id="c908c-122">companyName</span></span>|<span data-ttu-id="c908c-123">string</span><span class="sxs-lookup"><span data-stu-id="c908c-123">string</span></span>|<span data-ttu-id="c908c-124">O nome da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-124">The name of the person's company.</span></span>|
|<span data-ttu-id="c908c-125">departamento</span><span class="sxs-lookup"><span data-stu-id="c908c-125">department</span></span>|<span data-ttu-id="c908c-126">string</span><span class="sxs-lookup"><span data-stu-id="c908c-126">string</span></span>|<span data-ttu-id="c908c-127">O departamento da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-127">The person's department.</span></span>|
|<span data-ttu-id="c908c-128">displayName</span><span class="sxs-lookup"><span data-stu-id="c908c-128">displayName</span></span>|<span data-ttu-id="c908c-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c908c-129">string</span></span>|<span data-ttu-id="c908c-130">O nome de exibição da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-130">The person's display name.</span></span>|
|<span data-ttu-id="c908c-131">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="c908c-131">emailAddresses</span></span>|<span data-ttu-id="c908c-132">coleção [rankedEmailAddress](rankedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="c908c-132">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="c908c-133">Os endereços de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-133">The person's email addresses.</span></span>|
|<span data-ttu-id="c908c-134">givenName</span><span class="sxs-lookup"><span data-stu-id="c908c-134">givenName</span></span>|<span data-ttu-id="c908c-135">string</span><span class="sxs-lookup"><span data-stu-id="c908c-135">string</span></span>|<span data-ttu-id="c908c-136">O nome fornecido da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-136">The person's given name.</span></span>|
|<span data-ttu-id="c908c-137">id</span><span class="sxs-lookup"><span data-stu-id="c908c-137">id</span></span>|<span data-ttu-id="c908c-138">string</span><span class="sxs-lookup"><span data-stu-id="c908c-138">string</span></span>|<span data-ttu-id="c908c-139">O identificador exclusivo da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-139">The person's unique identifier.</span></span> <span data-ttu-id="c908c-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c908c-140">Read-only.</span></span>|
|<span data-ttu-id="c908c-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="c908c-141">isFavorite</span></span>|<span data-ttu-id="c908c-142">booliano</span><span class="sxs-lookup"><span data-stu-id="c908c-142">boolean</span></span>|<span data-ttu-id="c908c-143">`true` se o usuário tiver sinalizado essa pessoa como um favorito.</span><span class="sxs-lookup"><span data-stu-id="c908c-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="c908c-144">mailboxType</span><span class="sxs-lookup"><span data-stu-id="c908c-144">mailboxType</span></span>|<span data-ttu-id="c908c-145">string</span><span class="sxs-lookup"><span data-stu-id="c908c-145">string</span></span>|<span data-ttu-id="c908c-146">O tipo de caixa de correio que é representado pelo endereço de email da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-146">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="c908c-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="c908c-147">officeLocation</span></span>|<span data-ttu-id="c908c-148">string</span><span class="sxs-lookup"><span data-stu-id="c908c-148">string</span></span>|<span data-ttu-id="c908c-149">O local do escritório da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-149">The location of the person's office.</span></span>|
|<span data-ttu-id="c908c-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="c908c-150">personNotes</span></span>|<span data-ttu-id="c908c-151">string</span><span class="sxs-lookup"><span data-stu-id="c908c-151">string</span></span>|<span data-ttu-id="c908c-152">As anotações de forma livre que o usuário fez sobre essa pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="c908c-153">personType</span><span class="sxs-lookup"><span data-stu-id="c908c-153">personType</span></span>|<span data-ttu-id="c908c-154">string</span><span class="sxs-lookup"><span data-stu-id="c908c-154">string</span></span>|<span data-ttu-id="c908c-155">O tipo de pessoa, por exemplo, lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="c908c-155">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="c908c-156">telefones</span><span class="sxs-lookup"><span data-stu-id="c908c-156">phones</span></span>|<span data-ttu-id="c908c-157">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="c908c-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="c908c-158">Os números de telefone da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="c908c-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="c908c-159">postalAddresses</span></span>|<span data-ttu-id="c908c-160">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="c908c-160">[location](location.md) collection</span></span>|<span data-ttu-id="c908c-161">Os endereços da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-161">The person's addresses.</span></span>|
|<span data-ttu-id="c908c-162">profession</span><span class="sxs-lookup"><span data-stu-id="c908c-162">profession</span></span>|<span data-ttu-id="c908c-163">string</span><span class="sxs-lookup"><span data-stu-id="c908c-163">string</span></span>|<span data-ttu-id="c908c-164">A profissão da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-164">The person's profession.</span></span>|
|<span data-ttu-id="c908c-165">fontes</span><span class="sxs-lookup"><span data-stu-id="c908c-165">sources</span></span>|<span data-ttu-id="c908c-166">coleção [personDataSource](persondatasource.md)</span><span class="sxs-lookup"><span data-stu-id="c908c-166">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="c908c-167">As fontes das quais os dados do usuário são provenientes, por exemplo, contatos do Outlook ou do Outlook.</span><span class="sxs-lookup"><span data-stu-id="c908c-167">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="c908c-168">surname</span><span class="sxs-lookup"><span data-stu-id="c908c-168">surname</span></span>|<span data-ttu-id="c908c-169">string</span><span class="sxs-lookup"><span data-stu-id="c908c-169">string</span></span>|<span data-ttu-id="c908c-170">O sobrenome da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-170">The person's surname.</span></span>|
|<span data-ttu-id="c908c-171">title</span><span class="sxs-lookup"><span data-stu-id="c908c-171">title</span></span>|<span data-ttu-id="c908c-172">string</span><span class="sxs-lookup"><span data-stu-id="c908c-172">string</span></span>|<span data-ttu-id="c908c-173">O título da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-173">The person's title.</span></span>|
|<span data-ttu-id="c908c-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c908c-174">userPrincipalName</span></span>|<span data-ttu-id="c908c-175">string</span><span class="sxs-lookup"><span data-stu-id="c908c-175">string</span></span>|<span data-ttu-id="c908c-p104">O nome UPN da pessoa. O UPN é um nome de logon para a pessoa ao estilo da Internet com base na [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email da pessoa. O formato geral é alias@domínio.</span><span class="sxs-lookup"><span data-stu-id="c908c-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="c908c-180">websites</span><span class="sxs-lookup"><span data-stu-id="c908c-180">websites</span></span>|<span data-ttu-id="c908c-181">Coleção [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="c908c-181">[website](website.md) collection</span></span>|<span data-ttu-id="c908c-182">Os sites da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-182">The person's websites.</span></span>|
|<span data-ttu-id="c908c-183">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="c908c-183">yomiCompany</span></span>|<span data-ttu-id="c908c-184">string</span><span class="sxs-lookup"><span data-stu-id="c908c-184">string</span></span>|<span data-ttu-id="c908c-185">O nome japonês fonético da empresa da pessoa.</span><span class="sxs-lookup"><span data-stu-id="c908c-185">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c908c-186">Relações</span><span class="sxs-lookup"><span data-stu-id="c908c-186">Relationships</span></span>

<span data-ttu-id="c908c-187">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c908c-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c908c-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c908c-188">JSON representation</span></span>

<span data-ttu-id="c908c-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c908c-189">Here is a JSON representation of the resource.</span></span>

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
